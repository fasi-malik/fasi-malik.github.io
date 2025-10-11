---
layout: distill
title: "How Machines Learn to Rebuild Particle Showers"
description: "An intuitive explainer on how AI models evaluate reconstruction quality — using ARI, Purity, and Efficiency."
date: 2025-10-06
featured: true
giscus_comments: false
authors:
  - name: Muhammad Bilal Azam
    url: "https://mbilalazam.github.io"
    affiliations:
      name: Illinois Institute of Technology
tags: AI DUNE particle-physics machine-learning
thumbnail: /assets/img/posts/2025-10-06-ai-reconstructs-particle-showers/cover.png
---

> *When physicists teach machines to recognize the footprints of invisible particles, how do they know the machine has truly understood what it’s seeing?*

---

### Understanding the invisible

In high-energy physics, detectors record tiny **fragments** of a particle’s energy trail — a bit like scattered puzzle pieces. When we train a deep-learning model to **reconstruct electromagnetic (EM) showers**, we want to know how well it has learned to assemble those pieces back into the right physical picture.

To measure that, physicists use a family of **clustering and learning metrics** — mathematical scorecards that tell us how "physicist-like" the machine’s reconstruction really is. Let’s unpack some of these metrics in plain language.

---

## 1. Adjusted Rand Index (ARI)

Imagine you and your friend both try to sort puzzle pieces into their correct pictures. The Adjusted Rand Index (ARI) checks **how similar your sorting is**, while correcting for the chance that you might agree just by luck.

If both of you consistently group the same pairs of pieces together, ARI will be close to **1.0** — perfect agreement.  If your grouping is random, it hovers near **0**. Negative values mean you are actively disagreeing (rare, but interesting).

Formally, scientists measure it as:

$$
\text{ARI} = \frac{\text{RI} - E(\text{RI})}{\max(\text{RI}) - E(\text{RI})}
$$

where the **Rand Index (RI)** measures how consistently pairs are grouped in both the true and predicted clusters:

$$
\text{RI} = \frac{a + b}{a + b + c + d}
$$

Here:
- $$a$$: pairs in the same group in both truth and prediction  
- $$b$$: pairs in different groups in both  
- $$c$$: pairs in the same group in truth but different in prediction  
- $$d$$: pairs in the same group in prediction but different in truth  

### Example: Step-by-step RI calculation

Let us go through a small example to see where the numbers come from. We have **six fragments** labeled $$F1–F6$$. The Ground truth groups are:

$$
\{F1, F2\}, \{F3, F4\}, \{F5, F6\}  
$$

and the predicted groups are:  

$$
\{F1, F2\}, \{F3, F5\}, \{F4, F6\}  
$$

There are  

$$
\binom{6}{2} = 15
$$

unique fragment pairs to compare.  
For each pair, we check whether the two fragments are in the **same group** in truth and prediction.

| Pair | Same in Truth? | Same in Prediction? | Agreement |
|:-----|:---------------:|:-------------------:|:-----------:|
| F1–F2 | ✅ Yes | ✅ Yes | ✅ Agree |
| F1–F3 | ❌ No | ❌ No | ✅ Agree |
| F1–F4 | ❌ No | ❌ No | ✅ Agree |
| F1–F5 | ❌ No | ❌ No | ✅ Agree |
| F1–F6 | ❌ No | ❌ No | ✅ Agree |
| F2–F3 | ❌ No | ❌ No | ✅ Agree |
| F2–F4 | ❌ No | ❌ No | ✅ Agree |
| F2–F5 | ❌ No | ❌ No | ✅ Agree |
| F2–F6 | ❌ No | ❌ No | ✅ Agree |
| F3–F4 | ✅ Yes | ❌ No | ❌ Disagree |
| F3–F5 | ❌ No | ✅ Yes | ❌ Disagree |
| F3–F6 | ❌ No | ❌ No | ✅ Agree |
| F4–F5 | ❌ No | ❌ No | ✅ Agree |
| F4–F6 | ❌ No | ✅ Yes | ❌ Disagree |
| F5–F6 | ✅ Yes | ❌ No | ❌ Disagree |

Out of 15 total pairs:
- 11 pairs agree (same grouping judgment in both truth and prediction)  
- 4 pairs disagree  

Hence,

$$
\text{RI} = \frac{11}{15} \approx 0.733
$$

ARI then adjusts this value by subtracting the expected agreement due to random chance, giving a final score closer to **0.7** for this example.

---

**Intuition:**  
ARI asks: *for every pair of fragments, did the AI make the same grouping decision that nature did?* By comparing all fragment pairs, it captures both correct associations and subtle mis-groupings across the whole event.


ARI is powerful because it considers **every possible fragment pair** — a complete measure of how coherently the AI has “understood” an event.

---

## 2. Purity — “How clean are the predicted groups?”

Purity examines each **predicted cluster** the model creates. It asks whether all fragments in that cluster truly belong to the same physical shower. A perfectly pure cluster means the model did not mix fragments from different particles. If fragments from two showers end up together, purity drops.

$$
\text{Purity} = \frac{1}{N} \sum_{i=1}^{N_p} \max_j |c_i \cap t_j|
$$

where:
- $$N$$: total number of fragments  
- $$c_i$$: fragments in predicted cluster $$i$$  
- $$t_j$$: fragments in true cluster $$j$$  

Think of it like this: each cluster is a jar, and each particle’s fragments are colored marbles. Purity measures how many red marbles slipped into a jar meant for blue ones.

High purity = clean clusters, minimal mixing.  
But purity alone does not punish **over-splitting** — if one true shower is divided into many small predictions, purity might still look good. That is why we also track **efficiency**.

---

## 3. Clustering Efficiency — “How complete are the true showers?”

Efficiency flips the question. Instead of asking “Is each prediction clean?”, it asks “Did we recover each true shower completely?”

$$
\text{Efficiency} = \frac{1}{N} \sum_{i=1}^{N_t} \max_j |t_i \cap c_j|
$$

A high efficiency means the AI grouped most of a true particle’s fragments together — a test of **completeness**, not cleanliness.

A good reconstruction strikes a balance:
- **Purity** rewards precision (no contamination).  
- **Efficiency** rewards recall (no fragmentation).

> **Analogy:**  
> Purity is like making sure no wrong puzzle pieces are in your pile.  
> Efficiency is making sure you actually found *all* the right ones.

---

## 4. Edge and Node Accuracy

Inside the model, each event becomes a **graph**:
- Nodes are fragments.  
- Edges represent possible connections — “same shower or not?”

The AI predicts 1 if two fragments belong to the same shower, and 0 otherwise. The **edge accuracy** is simply:

$$
\text{Edge Accuracy} = \frac{\text{Number of correct edge predictions}}{\text{Total edges}}
$$

Similarly, **node accuracy** checks whether each fragment is correctly labeled as a *primary* — the one that started the shower.

> In other words, edge accuracy tests relationships, while node accuracy tests identities. Together, they reveal how well the AI has learned the physics of connectivity.

---

## 5. Loss — “How far are predictions from the truth?”

While accuracy counts how many predictions were right, **loss** tells us *how confident* the model was when it was right or wrong. It is computed with **Binary Cross-Entropy (BCE)** — a function that punishes confident mistakes more heavily than hesitant ones.

$$
\mathcal{L} = \mathcal{L}_e + \mathcal{L}_v
$$

where

$$
\mathcal{L}_e = -\frac{1}{N_e} \sum_{(i,j)} \Big[a_{ij} \ln(s_{ij}^e) + (1 - a_{ij}) \ln(1 - s_{ij}^e)\Big]
$$

and

$$
\mathcal{L}_v = -\frac{1}{N_v} \sum_i \Big[y_i \ln(s_i^v) + (1 - y_i) \ln(1 - s_i^v)\Big]
$$

Here:
- $$s_{ij}^e$$: predicted probability that two fragments belong together  
- $$s_i^v$$: predicted probability that a fragment is primary  
- $$a_{ij}, y_i \in \{0,1\}$$: true labels  

Lower loss = closer alignment between machine predictions and physical truth.

---

## 6. Putting It All Together

These metrics fall into two complementary families:

| Category | Metrics | What They Reveal |
|-----------|----------|------------------|
| **Learning behavior** | Accuracy, Loss | How well the network is learning |
| **Physical reconstruction** | ARI, Purity, Efficiency | How well it is rebuilding reality |

When both sets improve together, it means the AI is not just memorizing data — it is genuinely *learning physics*. Each score tells part of the story, from how fragments pair up to how full showers emerge.

---

### In short:
> ARI judges agreement,  
> Purity measures cleanliness,  
> Efficiency measures completeness,  
> Accuracy tracks correctness,  
> and Loss tells us how confidently wrong (or right) we were.

These metrics do not just evaluate a neural network — they show how close we are to teaching machines to **think like physicists**, rebuilding the invisible patterns of nature one fragment at a time.
