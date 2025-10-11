---
layout: distill
title: "Why do we need “Quantum Gravity”?"
description: "Motivation behind quantum gravity and causal sets."
tags: physics quantum-gravity causal-set-theory
date: 2021-01-31
giscus_comments: false
authors:
  - name: Muhammad Bilal Azam
    url: "https://mbilalazam.github.io"
    affiliations:
      name: Lahore University of Management Sciences
thumbnail: /assets/img/posts/2021-01-31-why-do-we-need-quantum-gravity/ch01_fig01_contents.png

bibliography: 2021-01-31-why-do-we-need-quantum-gravity.bib

toc:
  - name: The Basic Idea
  - name: Motivations for Quantum Gravity
  - name: Cut-Off Scales of Quantum Gravity
  - name: Approaches to Quantum Gravity
    subsections:
      - name: Three-and-Half Directions
---


📄 A printable version of this article is available [Why do we need "Quantum Gravity"? (PDF)](https://github.com/mbilalazam/mbilalazam.github.io/blob/main/assets/pdf/posts/2021-01-31-why-do-we-need-quantum-gravity/1_QG_and_CST_v1.pdf)


In the *Proceedings of the Royal Society of London*, in 1929, one of the giants of the twentieth-century scientific community, Paul Dirac narrated <d-cite key="Dirac1929"></d-cite> at a moment:  

> “The underlying physical laws necessary for the mathematical theory of a large part of physics and the whole of chemistry are thus completely known.”


However, the advancements in technology and innovative mathematical theories to study nature at its fundamentals made this statement quite vague, in essence, with the passage of time. People also stated the same when the discovery of the Higgs boson completed the mysterious puzzle of the Standard Model (SM) and made heuristic additions to our understanding of the universe, but then cosmology played its role to change the game and showed that the successful SM explains only around four percent of the universe while the nature and dynamics of the rest of the twenty-six percent dark matter and the seventy percent dark energy cannot be explained under its realm.  

These and some other compelling arguments again convinced the scientists to think of a more fundamental formalism to describe the underlying phenomena of nature — that is, a *theory of quantum gravity* — the merger of classical general relativity and quantum mechanics.


---

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0 text-center">
    {% include figure.liquid 
       path="assets/img/posts/2021-01-31-why-do-we-need-quantum-gravity/ch01_fig01_contents.png" 
       title="Pie Chart of the content of the Universe (Credits: NASA/WMAP Science Team)." 
       class="img-fluid rounded z-depth-1" %}
    <div class="caption">
      Pie chart of the content of the Universe (Credits: NASA/WMAP Science Team).
    </div>
  </div>
</div>

---

## The Basic Idea

Since the formulation of Einstein’s general relativity and quantum mechanics, both theories were (and are) successfully tested millions of times, which depicts how much important these theories are to modern-day science. In their formalism and ideas, both are far apart. General relativity is classical in nature, while quantum mechanics upholds the idea of quantization and interference at the subatomic scale. Quantum (field) theory successfully accommodates all the interactions of nature in its framework but gravity. This framework is called the **Standard Model of Particle Physics**. However, general relativity is the only available tool to study all the manifestations of the gravitational field. Despite all the efforts, we are unable to wed general relativity to quantum theory. Anyhow, some questions instantly pop out regarding their merger:

1. Why do we want to unify these two theories?  
2. Is it not possible that gravity is a classical theory and has no quantum roots?  
3. Is it really challenging to quantize gravity?  

Skip the first two questions for a moment and come to the very last question. The answer is **no** — it is not difficult to quantize gravity. We know how to canonically quantize<d-footnote>Canonical quantization, introduced by Dirac <d-cite key="Dirac1925"></d-cite>, is one of the most direct and simplest ways to quantize classical theories.</d-footnote> fields. People have already done it for non-gravitational fields such as electromagnetic, weak, and strong nuclear. It is exquisite and simple machinery.

1. *Write down* the classical Lagrangian density in terms of fields.  
2. *Calculate* momentum and Hamiltonian densities as fields.  
3. *Treat* these field densities as operators.  
4. *Impose* commutation relations to make them quantum mechanical.  
5. *Expand* the fields in terms of ladder operators.

And that’s it — the classical field has been quantized successfully.

The same trick can also be applied to the gravitational field. So, then? Would not this be the desired theory of quantum gravity? If it is straightforward, why are physicists struggling? To answer this, let us visit the first two questions in the next section.

---

### Motivations for Quantum Gravity

Before proceeding, it would be essential to note that certain *uniqueness theorems* say whatever theory of quantum gravity we develop must approximate Einstein’s GR (or Einstein–Cartan theory<d-footnote>Einstein–Cartan theory is the natural generalization of GR. It is written in the language of tensors and spinors to accommodate fermions and quarks in gravity. (We might discuss it in detail at some later point.)</d-footnote>) in some limit.

General relativity is a remarkably successful theory in its realm. Still, there are some rudimentary observational pieces of evidence that point out discrepancies in theoretical models and suggest a more fundamental viewpoint about gravity. Some of the primary motivations for quantum gravity are:

- **Unification:**  
  Physicists are reductionists. The history of science shows that reductionism has been proven very successful. The Standard Model is one of its prime examples where all the non-gravitational interactions can be studied under a single gauge group, $\mathrm{SU(3)} \times \mathrm{SU(2)} \times \mathrm{U(1)}.$ 
  In the last century, we have seen the unification of the electromagnetic and weak nuclear forces (electroweak). Why would there be a reason gravity cannot be unified with others? It should be.  

  Interestingly, there are also attempts to construct semiclassical frameworks in which all other forces are quantum while gravity remains essentially classical. However, all of these efforts have failed miserably. It indicates that classical and quantum concepts are likely incompatible, as inferred in the early days of quantum mechanics.

- **Universe:**  
  All the attempts of gravity quantization face one severe problem — they are not UV complete. They break at high-energy scales. From the evolution history of the universe<d-footnote><a href="https://mbilalazam.com/1-evolution-history-of-universe-a-story-from-zero-to-ten-seconds/" target="_blank">Evolution History of the Universe — A Story from Zero to Ten Seconds</a></d-footnote>, it is known that the present classical infrastructure of gravity tells us nothing about the initial conditions near the Big Bang or what happens at the sub-Planckian scale and final stages of black hole evolution. I want to discuss one example from cosmology and one from black holes in some detail.

  - **Cosmology:**  
    There are cosmological solutions, in agreement with observations, that successfully predict an accelerated expansion of the universe<d-footnote>We will discuss this problem in detail in the phenomenology of causal set theory.</d-footnote>. From this result, it can be extrapolated that this expansion started, at some zero cosmic time, from a highly dense point (or singularity) with no spatial dimensions. It is where classical GR fails to yield any feasible result(s). This inability to extract any information from this singularity and the subsequent Planck era signifies the need for a theory of quantized gravity.

  - **Black Holes:**  
    Annoyingly mysterious black holes also qualify as a testable region for quantum gravity. In the early seventies, Bekenstein interpreted the entropy of a black hole in terms of the area of its event horizon <d-cite key="Bekenstein1973"></d-cite>, and Hawking conjectured that black holes emit thermal radiation having a black-body spectrum <d-cite key="Hawking1975"></d-cite>. This brings about an identicalness in the thermal behavior of black holes and the conventional laws of thermodynamics. Classical GR fails to explain it well because entropy is described under the notion of discrete states of a quantum system in traditional thermodynamics. It makes black hole entropy phenomenologically important in the search for quantized gravity.

- **Time:**  
  It is one of the most radical issues in the pursuit of QG. Quantum and generally covariant theories (like GR) have drastically different concepts of time — they are incompatible. In quantum theory, time is available as an external parameter. It is not described by an operator; it is kinematical, absolute, and universal. Even in relativistic QFT, external Minkowski spacetime plays the role of absolute time. While in GR, time is a dynamical object. It is relative and non-absolute. It is not available as an external parameter; it needs to be constructed *naturally* by the theory itself. It is quite clear that the definition of time must be modified to develop a fully fledged theory of quantum gravity. We will revisit the problem of time while discussing the role of background structures in quantum gravity.

- **Divergence:**  
  Gravity is non-renormalizable. It breaks at high-energy scales and yields infinities. It is still an open issue how to cure these divergences. There should be no divergences for any quantum version of gravity, as there are none in quantum field theory.

---

## Cut-Off Scales of Quantum Gravity

Length, mass, and time are fundamental — the most basic physical quantities — and the speed of light $(c)$, gravitational constant $(G)$, and quantum of action $(\hbar)$ are the fundamental constants of nature. Can we form these quantities from the constants of general relativity, $c$ and $G$, or the constants of quantum theory, $c$ and $\hbar$? **No!** There is no possible combination of these two sets of universal constants that can produce any of the fundamental quantities.  

But can we derive these quantities using *all* of these constants in any combination? **Yes.** In honor of Max Planck, these units are called *Planck units*<d-footnote>For the sake of completeness — Planck units are defined exclusively in terms of four universal constants. The fourth one is the Boltzmann constant, $k_\text{B}$. Using the four constants, one can also define Planck units of temperature, density, the fine-structure constant of gravity, and charge.</d-footnote>. These units are:

$$
\begin{align*}
\text{Planck length} &= l_\text{P} = \sqrt{\frac{\hbar G}{c^3}} \approx 1.62\times10^{-33}\ \text{cm}, \\
\text{Planck time}   &= t_\text{P} = \frac{l_\text{P}}{c} = \sqrt{\frac{\hbar G}{c^5}} \approx 5.39\times10^{-44}\ \text{s}, \\
\text{Planck mass}   &= m_\text{P} = \frac{\hbar}{l_\text{P} c} = \sqrt{\frac{\hbar c}{G}} \approx 2.18\times10^{-5}\ \text{g}.
\end{align*}
$$

One may be bewildered by noticing that Planck mass is horrendously a larger quantity than Planck length and Planck time. But it is worth noting that $m_\text{P}$ must be concentrated in a linear dimension $l_\text{P}$; otherwise, we will not be able to observe quantum effects of gravity. At this scale, classical properties become an emergent phenomenon of quantum theory. These scales provide the cut-offs to observe quantum gravity.  

We can easily realize that these scales are nearly impossible to detect and observe with the present technology. However, these scales do not provide stringent limits on gravity — these are just the most natural possible cut-offs. The unified theory of forces may also contain other parameters; for instance, in string theory, the fundamental length scale is the string length $l_\text{S}$ rather than the Planck length $l_\text{P}$. Nevertheless, it is an educated guess to set $l_\text{S} = l_\text{P}$.


---

## Approaches to Quantum Gravity

Since the 1930s, there has been no shortage of proposed theories for the quantization of gravitational fields<d-footnote>A list of candidate theories can be found on the following Wikipedia page: <a href="https://en.wikipedia.org/wiki/Quantum_gravity#Candidate_theories" target="_blank">Quantum Gravity — Candidate Theories</a>. However, this is not an exhaustive list.</d-footnote>. No idea is complete; no theory is entirely consistent with quantum fields. No theory provides a way to put it to experimental tests; every approach suffers from conceptual problems. Every theory meets observational discrepancies.  

Issues are there, but even today, the charm of quantum gravity has not faded away — nothing is more fascinating than the problems of gravity. It is challenging to review all the approaches to quantum gravity in just one section; however, I will try to briefly discuss its main research directions. The subsequent sections may contain some *fancy* technical terms which I will intentionally try to oversimplify, and it may cause the text to lose some of its essence (so advanced readers are advised to see <d-cite key="Oriti2009"></d-cite> and <d-cite key="Rovelli2004"></d-cite> and references therein, upon which this section is based).


### Three-and-Half Directions

Research in quantum gravity can be mapped onto three main — and some *neglected* — lines:

- covariant  
- canonical  
- sum-over-histories  
- others  

This list does not qualify to be a precise way to describe research directions since these names are somewhat misleading and sometimes are used interchangeably. Still, they possess specific scientific rationality, developmental logic, and methodological unity. Often, one approach becomes a hot topic, and others get neglected — this has happened repeatedly over the years. However, all of these approaches share some common features, and many ideas cannot fit neatly into any one of these directions.

- **Covariant Approach:**  
  Started in the early thirties by Rosenfeld, Fierz, and Pauli, it is one of the most dominant research directions in the pursuit of quantum gravity. It is an attempt to construct a quantum field theory of gravity. In covariant approaches, fluctuations of the metric element are studied over a four-dimensional Lorentzian flat spacetime or some other appropriate background metric. Rules and equations were established in the sixties by Feynman, Faddeev, and others, while the approach was proved to be non-renormalizable by ’t Hooft and others in the seventies. The search for renormalizability gave birth to string theory in the late eighties — whose sun has not set to date.

- **Canonical Approach:**  
  Initiated by Dirac and pioneered by Wheeler, DeWitt, and Ashtekar, it is the Hamiltonian (or canonical) formulation of general relativity. In this approach, phase-space variables are promoted to quantum operators on a Hilbert space, and these operators correspond to the full metric or some of its functions. The canonical approach started gaining attention when the framework of loop quantum gravity (LQG) was established. LQG remains one of the most significant competitors to string theory.

- **Sum-Over-Histories Approach:**  
  Feynman pioneered the path-integral (SOH) formulation, which proved itself as one of the most successful formalisms of quantum theory. In the quantum world, there are infinite ways (paths) to go from some initial point to a final point, and the probabilities are given by adding contributions from all the possible trajectories (or histories). Similarly, in gravity, this sum is taken over all possible geometries of spacetime. Some discrete causal approaches to quantum gravity are based on different versions of SOH — for instance, the spinfoam formalism or the causal set approach.

- **Other Approaches:**  
  These include effective field theories (such as non-commutative geometry), Penrose’s twistor theory, Regge calculus, causal dynamical triangulation, causal sets, and many more. Some of the alternate approaches have suffered from serious and fundamental crises, while others are too mathematical to describe physical reality. Still, many of these ideas provide astonishing insight into the phenomenology of quantum gravity and bridge the gap between theoretical and observational discrepancies.

It is also important to note that only string theory claims to be the unified version of all fundamental forces — or, loosely speaking, the *theory of everything* — while all other approaches provide different ways to merge quantum theory with general relativity. None of these approaches have matured into fully fledged quantum versions of gravity. All ideas are still in development. Some proposed versions of gravitational theories have an established kinematical side but lack a dynamical framework. For avid history readers, the evolution of research in quantum gravity is summed up in Figure below, taken from <d-cite key="Rovelli2004"></d-cite>.

Lastly, we have briefly reviewed the idea of quantum gravity, its need, present problems, and some of the possible directions. Readers may visit the references (and references therein) for a detailed outlook of the topic. This series is dedicated to *causal set theory*, initiated by Rafael Sorkin in the early eighties, and from the next post, we will try to discuss it from the very basics. We will discuss the need for discrete causal approaches and the causal metric hypothesis, which will lead us to one of the most important theoretical breakthroughs of the last century — *metric recovery theorems*.

---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0 text-center">
    {% include figure.liquid 
       path="assets/img/posts/2021-01-31-why-do-we-need-quantum-gravity/history_of_qg_rovelli.svg" 
       title="The search for a quantum theory of the gravitational field (adapted from Rovelli 2004)." 
       class="img-fluid rounded z-depth-1" %}
    <div class="caption">
      The search for a quantum theory of the gravitational field (adapted from <d-cite key="Rovelli2004"></d-cite>).
    </div>
  </div>
</div>
