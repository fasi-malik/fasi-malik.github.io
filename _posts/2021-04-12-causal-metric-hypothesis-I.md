---
layout: distill
title: "Causal Metric Hypothesis–I"
description: "Exploring the causal metric hypothesis, its philosophical roots, and its role in defining the discrete structure of spacetime within causal set theory."
tags: physics quantum-gravity causal-set-theory spacetime metric-recovery
date: 2021-04-12
giscus_comments: false
authors:
  - name: Muhammad Bilal Azam
    url: "https://mbilalazam.github.io"
    affiliations:
      name: Lahore University of Management Sciences
thumbnail: /assets/img/posts/2021-04-12-causal-metric-hypothesis-I/cover.png

bibliography: 2021-04-12-causal-metric-hypothesis-I.bib

toc:
  - name: General Version of Hypothesis
    subsections:
      - name: Background
      - name: Roots of the Causal Metric Hypothesis and Emergent Spacetime
      - name: Restatement of the General Version
      - name: Technical Implementation
  - name: Previous Blog Posts
---

📄 A printable version of this article is available [Causal Metric Hypothesis–I (PDF)](https://github.com/mbilalazam/mbilalazam.github.io/blob/main/assets/pdf/posts/2021-04-12-causal-metric-hypothesis-I/3_Causal_Metric_Hypothesis_CST_Blog.pdf)

---


## General Version of Hypothesis

### Background

It can be safely stated the whole idea of the discrete causal theories relies on the question: “How to and up to which level, one can recover the continuum from the discrete spacetime?” Answer circles around a very important concept of metric recovery theorems. To refer to these theorems in a more broad sense, we will stick to the term, *causal metric hypothesis*, adopted by Dribus <d-cite key="Dribus2017"></d-cite>. In general, it can be stated as follows.

> *“The properties of the physical universe are manifestations of causal structure.”*

This hypothesis relies upon the metric recovery theorems proposed and proven by Hawking <d-cite key="Hawking1975a"></d-cite> and Malament <d-cite key="Malament1976"></d-cite> in the late 1970s. However, it received a remarkable share in the research community when Rafael Sorkin proposed this as an explicit structural ansatz for the causal set theory <d-cite key="Sorkin2009"></d-cite>. He states:

> *“Order plus number equals geometry.”*

This gives an entirely new meaning to the scope of metric recovery theorems and proposes the *discrete and directed structure* for spacetime at the most fundamental (or quantum) levels. The causal set idea, one of the most prominent proponents of discrete spacetime, is based upon Sorkin's version of the causal metric hypothesis.

Although the causal metric hypothesis is studied in the context of discrete spacetime, yet it does not require a strict assumption of discreteness. Causal metric hypothesis is needed to recover the geometry from the underlying spacetime, and in case of continuum spacetime, at least under the relativistic assumption, metric recovery theorems will not be quite sufficient and contains enough information to recover the geometry. However, there are versions of the causal metric hypothesis, which are neither discrete nor continuous. It is important to note, in causal set theory, Sorkin's version is applied at the classical level<d-footnote>There is no fully-developed quantum causal set dynamics yet.</d-footnote> but is explicitly discrete. Such a discrete notion of spacetime invokes *counting*; count atoms, count volume, count everything, and it requires the condition of local finiteness.

---

### Roots of the Causal Metric Hypothesis and Emergent Spacetime

There is a whole lot of debates on the idea of causal metric hypothesis, from its philosophical aspects to its connection to modern exploration to nature. Roots of this hypothesis can be traced back to the ancient Greeks; a famous example would be Zeno's paradox. In the modern era of science, from Leibniz to Riemann, Einstein to Finkelstein, and Hawking to Sorkin, everyone contributed. Despite all the popular and ambitious fantasy of philosophical and scientific aspects of the hypothesis and the technical results, it is still concerned whether this hypothesis is “true” or “almost true”? This hypothesis is such a great deal in itself that metric recovery theorems suggest that, at the very least, this should have been “almost true” in nature and the aspects of the geometrical structure of spacetime, which prevents the hypothesis from being exactly “true” does not actually exist but only in case of emergent spacetime. Moreover, as the concept of directed sets relies upon causality, so we may extend the scope of this causal structure even beyond the spacetime fabric, and it can include all sorts of physical interactions being observed in nature. It links the hypothesis to the modern attempts of unification.

Before proceeding further, let us briefly discuss the ideas of *emergence* and *emergent spacetime*. In *reductionist philosophy*, one breaks down the “true” laws of nature into the most fundamental form. However, it remains a challenging task, how to construct and explain the exact (or even approximate) descriptions of macroscopic objects from these microscopic ideas. For example, in high school, we develop a structural model and dissect the frog to understand the individual parts, and it works well there. Nevertheless, still, there are complicated biological processes that cannot be understood with the same model. If one tries to explain, it is nearly impossible to get some adequate results to understand *all* the processes. Even in physics, any macroscopic system can be viewed as a verily large collection (ensemble) of microscopic states. Here, emergence describes those properties of the system, which occurs at the macroscopic scale but not on the microscopic level. For example, quantum properties are more fundamental than their classical counterparts, but the quantum structure cannot be observed at a macroscopic level. So, classical mechanics can be thought of as an emergent description of quantum mechanics under some limitations. Similarly, in condensed-matter systems, a large ensemble of fermions on the surface of metal forms a Fermi surface. It ultimately leads to the idea of Fermi liquid theory, which is an emergent phenomenon and does not require us to construct the individual excitation of fermions in a quantum field to model their behavior. However, it must be noted, in a philosophical sense, emergence may or may not contrast to the reductionist approach.

On the same grounds, many phenomena and observational measurements compel to think that spacetime is not fundamental but is an effective description of nature, and there is some more fundamental theory whose degrees of freedom are quantum mechanical in nature. The dynamics of such a system emerge out the particles and fields living in a spacetime. Here comes an important point. The standard model of particle physics requires a fixed background spacetime to define causality and locality. All the interactions of particles appear on this fixed spacetime, and the features of causality and locality have been tested successfully millions of times in particle accelerators, and these accelerators work on TeV scales. It signifies, if such an emergent spacetime exists, it is much beyond the reach of present particle accelerators, that is, somewhere between the present TeV and Planck scale. Let us elaborate on the last point in the context of discrete causal theories. Einstein's field equation is:

$$
R_{\mu\nu} - \frac{1}{2} R g_{\mu\nu} + \Lambda g_{\mu\nu} = \frac{8\pi G}{c^4} T_{\mu\nu}.
$$

where $ R_{\mu\nu} $ is the Ricci curvature tensor, $ R $ is the Ricci scalar, $ g_{\mu\nu} $ is the metric tensor, $ \Lambda $ is the cosmological constant and $ T_{\mu\nu} $ is the stress-energy tensor. This equation applies to the classical spacetime, as depicted in the left-hand diagram in the figure below. Warped dark gray triangles represent the set of events that could be causally connected to event $ x $. Middle diagram is a magnified view of a region near to the event $ x $, and according to causal set theory, at such a small scale, discreteness or granularity of spacetime starts appearing, so Einstein's field equations will start losing their precision. However, this is an intermediate scale, and it can still be approximated to the continuum spacetime. Despite the intermediate scales, these are still very much larger than the probing ability of present accelerators, raising some important issues to worry about:

1. Up to which order, such an approximation can produce consistent and effective results?
2. These deviations are quite noticeable, how they will manifest themselves experimentally?

To handle these issues, people suggested the systematic violations of Lorentz invariance, but we will explore the technical details and reasoning behind its proposition in future blog posts. The right-hand diagram in the figure is a highly magnified version of spacetime region around the event $ x $ and represents the hypothesized granularity of spacetime. Discreteness is quite evident at this level, geometry is no more smooth, and Einstein's field equation becomes essentially irrelevant. It should not be surprising that $ x $ could have been connected to a very large number of spacetime atoms (or satoms<d-footnote>This term is coined by Maqbool Ahmed.</d-footnote>) say $ 10^{50} $ or more. Black nodes are the events causally connected to $ x $, while light gray nodes are causally not related to $ x $.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0 text-center">
    {% include figure.liquid 
       path="assets/img/posts/2021-04-12-causal-metric-hypothesis-I/blog_cstheory_3_figure_1.jpg" 
       title="Classical spacetime according to discrete causal theory (Benjamin Dribus 2017)." 
       class="img-fluid rounded z-depth-1" %}
    <div class="caption">
      Classical spacetime according to discrete causal theory (<d-cite key="Dribus2017"></d-cite>).
    </div>
  </div>
</div>

---

### Restatement of the General Version of Causal Metric Hypothesis

In the start, we present the general statement, proposed by <d-cite key="Dribus2017"></d-cite>, as:

> *“The properties of the physical universe are manifestations of causal structure.”*

This statement takes the cause-and-effect relationship as a primary tenet to the physical phenomena and invokes that “physics is *essentially structured* in nature.” However, the scope of this tenet as a fundamental building block of nature is questionable in its extent. So, the hypothesis is interpreted differently in its comprehensiveness. For a conservationist, properties of *physical universe* are the mere descriptions of the *spacetime*. So we can redefine the above statement as:

> *“The properties of the spacetime are manifestations of causal structure.”*

Such a feature is possessed by theories that have a limited degree of background independence, such as the discrete quantum field theories and some theories of gravity too. This is somewhat a *weak interpretation* of the causal metric hypothesis. In a *strong interpretation* sense, one thinks of *all* the properties of the physical universe being emerged out from the deep underlying causal structure. It is stated as:

> *“All the properties of the physical universe are manifestations of causal structure.”*

This statement is quite radical in itself and requires and enables a doorway to *perfect background independence*. At this point, it seems necessary to discuss background independence briefly. It always remains a subtle question of interest in theoretical physics, whether a theory of quantum gravity would be background dependent or independent. This condition asserts that background spacetime is not fixed; instead, this results from the dynamical equations. A background independent theory is said to be *coordinate-free* theory, as Einstein's theory of general relativity is. In such a theory, the results can be inferred from the *first principles*. Newton's law of gravitation is:

$$
F = G \frac{m_1 m_2}{r^2}.
$$

Remaining in the Newtonian context, one always has to perform experiments to see a $ r $-squared term in the denominator. It is impossible to figure out from the first principles, what power $ r $ will take? So, we can say, the Newtonian theory is background dependent. However, in GR, one can get this $ r $-squared term comes from the first principles. It comes naturally. So, Einstein's theory confirms that gravity is a background independent theory. Similarly, the action functional of the electromagnetic field $ S[A] $ is also background dependent, but when it is coupled to gravity, $ S[A,g] $ becomes background independent. The Maxwell and Einstein-Hilbert action functionals are given as <d-cite key="Blau2019"></d-cite>:

$$
\begin{align*}
S_\text{EM}[A] &= -\frac{1}{4} \int F_{\mu\nu} F^{\mu\nu} \sqrt{-g} d^4 x, \\
S_\text{EH}[g] &= \frac{1}{16\pi G} \int_M R_{\mu\nu} g^{\mu\nu} \sqrt{-g} d^4 x. 
\end{align*}
$$

Such a background independent treatment of a physical theory is the corollary of the principle of general covariance. Upon seeing the actions of both fields, one can get confused, but it is always important to keep in mind that “diffeomorphism invariance is not the same as background independence.” We will dedicate a blog in the future to elaborate this difference in detail, but let us turn our attention back to the causal metric hypothesis.

Relativistic understanding and causal metric hypothesis are more or less way to look at the same thing. In Einstein's relativity, one may prescribe which events may influence $ x $ or which events, $ x $ may influence (see the figure above). This is the “prescription of possible behavior.” On the other hand, the causal metric hypothesis gives an approximate<d-footnote>Here, the word “approximation” is of extreme importance. It is linked with the question we posed earlier, up to which conformal factor, the macroscopic world can be recovered from the underlying spacetime. Quantitatively, we will discuss this in future blog posts.</d-footnote> way to describe, in actual, which events influence $ x $ and which events are influenced by $ x $. This is the “description of actual behavior.” So, we can describe Wheeler's famous statement <d-cite key="Wheeler2010Geons"></d-cite>:

> *“Spacetime tells matter how to move; matter tells spacetime how to curve,”*

in the context of discrete causal theories as <d-cite key="Dribus2017"></d-cite>:

> *“Things happen; ‘spacetime’ and ‘matter’ are ways of describing them.”*

This, somewhat, seems to have a philosophical connection. However, it is equally important in discrete causal theories as it directly relates to the concept of perfect background independence.

---

### Technical Implementation of Causal Metric Hypothesis

The technical implementation of CMH has its own meaning in the classical and quantum world. It is a matter of a great deal, what is the mathematical definition of the causal structure? Or what is the meaning of causal structure mathematically? Or how to identify causal structure in mathematical terms? In the following posts, we will stick to the classical causal metric hypothesis (CCMH), which models classical spacetime via a directed set. To make theory capable of giving the quantitative description of nature, some conditions or the *axioms* are imposed on it, for instance, the partially ordered sets in causal set theory. Usually, these axioms are applied to the hypothesis based on the physical intuition, but experimental and observational results also play their role, whenever it seems adequately necessary. In the next episode on CMH, we will study the quantitative and qualitative treatment of the classical causal metric hypothesis.

---

## Previous Blog Posts

- [What do we need Quantum Gravity?](https://mbilalazam.github.io/blog/2021/why-do-we-need-quantum-gravity/)
- [A Picture and an Equation](https://mbilalazam.github.io/blog/2021/a-picture-and-an-equation/)
