---
layout: distill
title: "A Picture and an Equation"
description: "Exploring the connection between equations and diagrams — from Feynman’s visualization to causal structures in discrete spacetime."
tags: physics quantum-gravity causal-set-theory feynman-diagram penrose-diagram
date: 2021-03-07
giscus_comments: false
authors:
  - name: Muhammad Bilal Azam
    url: "https://mbilalazam.github.io"
    affiliations:
      name: Lahore University of Management Sciences
thumbnail: /assets/img/posts/2021-03-07-a-picture-and-an-equation/Penguin_diagram_01.jpg

bibliography: 2021-03-07-a-picture-and-an-equation.bib

toc:
  - name: An Equation and a Picture
  - name: A Picture and an Equation
  - name: Representation of Structures
  - name: How to Model a Picture with an Equation?
    subsections:
      - name: Causal Schrödinger-Type Equations
---

📄 A printable version of this article is available [A Picture and an Equation (PDF)](https://github.com/mbilalazam/mbilalazam.github.io/blob/main/assets/pdf/posts/2021-03-07-a-picture-and-an-equation/2_A_Picture_and_an_Equation_v1.pdf)

---

In the [previous blog post](https://mbilalazam.github.io/blog/2021/why-do-we-need-quantum-gravity/), we aimed at the questions which compel us to start a pursuit for a quantum theory of gravity. From now on, we will begin paving the path for the discrete versions of spacetime. A famous adage says, “A picture is worth a thousand words,” and this is profoundly true in science. The relation between physics and figures is as old as the history of physics itself. A typical science student becomes familiar with figures (particularly *free-body diagrams*) while solving everyday mechanics problems via Newton’s laws. In the second half of the last century, Feynman elevated diagrams to a new level, using them to study complex quantum interactions and associating equations with different segments of those diagrams. In the next section, we briefly review some notable examples — from quantum field theory to relativity.

---

## An Equation and a Picture

The idea of modeling physical processes — or even equations — through *pictures* dates back to the iconoclastic Richard P. Feynman, who introduced his famous diagrams in 1949 <d-cite key="Feynman1949"></d-cite>. Feynman diagrams provide simple visualizations of abstract mathematical ideas. Imagine electrons represented by solid lines. Arrows pointing forward in time denote particles; those pointing backward represent antiparticles. When two such lines meet and exchange a photon (a wiggly line), the diagram captures the entire interaction. The first published Feynman diagram is shown below. Employing Feynman rules, one can assign mathematical formulas to each part of the diagram — and the computed results match those from the cumbersome mathematics of quantum fields.


<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0 text-center">
    {% include figure.liquid 
       path="assets/img/posts/2021-03-07-a-picture-and-an-equation/feynman_diagram_01.png" 
       title="Exchange of one photon between two electrons (Feynman 1949)." 
       class="img-fluid rounded z-depth-1" %}
    <div class="caption">
      Exchange of one photon between two electrons (<d-cite key="Feynman1949"></d-cite>).
    </div>
  </div>
</div>



Feynman diagrams have proved so useful that they have become integral to quantum field theory. Another famous class, *penguin diagrams*, was inspired by Feynman diagrams. Below is a penguin diagram superimposed on an image of a Gentoo penguin.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid 
       path="assets/img/posts/2021-03-07-a-picture-and-an-equation/Penguin_diagram_01.jpg" 
       title="Penguin diagram (Wikipedia)." 
       class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
A penguin diagram overlaid on an image of a Gentoo penguin.  
<span style="font-size: 0.9em; color: gray;">(Image source: Wikipedia)</span>
</div>

Diagrams are equally central to relativity — from simple Minkowski spacetime diagrams in special relativity to the more complex *Penrose–Carter diagrams*, which represent the causal structure of spacetimes containing black holes. The first Penrose diagram appeared in <d-cite key="Penrose1963"></d-cite>.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid 
       path="assets/img/posts/2021-03-07-a-picture-and-an-equation/penrose_diagram_01.png" 
       title="Penrose diagram (Penrose 1963)." 
       class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Penrose diagram illustrating causal structure of spacetime (<d-cite key="Penrose1963"></d-cite>).
</div>

---

Loosely speaking, the same conceptual idea is also used in discrete causal approaches — but in reverse. Instead of drawing equations from diagrams, we first *construct* spacetime diagrams representing causal relations and then derive the corresponding mathematical expressions from the axioms of the theory. In the next section, we’ll see how we can study the nature of spacetime atoms using such pictures and eventually arrive at the causal analog of the Schrödinger equation.

---

## A Picture and an Equation

Causal theories provide a figurative way to understand and model the universe around us. A glimpse of such a quantum universe is shown below <d-cite key="Dribus2017"></d-cite>.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid 
       path="assets/img/posts/2021-03-07-a-picture-and-an-equation/blog_cstheory_2_figure_1.png" 
       title="Quantum universe in discrete causal theory (Dribus 2017)." 
       class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
Quantum universe in discrete causal theory (<d-cite key="Dribus2017"></d-cite>).
</div>

Two different levels of structural hierarchy in such causal universes are:
- higher-level structures  
- lower-level structures  

In the figure above, the large open nodes and long edges are higher-level structures representing a small portion of the quantum multiverse. Lower-level structures — drawn as filled dots inside these open nodes — connect via lines to other nodes or remain isolated.   This recalls the “ball-and-stick” molecular model. In physics, however, these structures are far simpler yet extremely powerful: they encode *classical universes* or *histories*. Both terms are used interchangeably in causal theories, though “histories” emphasizes an extended process rather than isolated snapshots of spacetime. At this stage, we are not yet concerned with what these histories model or their size. But since they form the most fundamental structural units of spacetime, they must represent local processes such as particle interactions — likely many orders of magnitude smaller than the particles themselves.

---

## Representation of Structures

The “ball-and-stick” (or “node-and-edge”) representation exists at both structural levels. However, the edges are *directed* — each connecting an initial and a terminal node. These nodes are *events*, and the directed edges represent *cause-and-effect* relations. This is where **causality** enters. Such sets of events (or objects) are called *directed sets*<d-footnote>I will explain its technical details in upcoming posts.</d-footnote>. Before proceeding, we label the two structural levels as:

- Higher-level structures → *quantum structures*  
- Lower-level structures → *classical structures*  

Many readers may find this labeling counterintuitive: classical physics usually describes *large-scale* behavior, while quantum theory deals with the *microscopic*. Yet, this labeling becomes natural when viewed through Feynman’s *path-integral* (or *sum-over-histories*) approach <d-cite key="Feynman2005"></d-cite>. Feynman’s 1948 formulation generalizes the classical action principle. In classical mechanics, a particle has a unique trajectory between two points. In Feynman’s framework, it may take *any* of infinitely many paths. Each possible path contributes a phase (or amplitude), and summing all phases yields the observable quantum amplitude. In Feynman’s own words <d-cite key="Herbert1987"></d-cite>:

> “The electron does anything it likes ... It goes in any direction at any speed, forward and backward in time, however it likes, and then you add up the amplitudes and it gives you the wave function.”

---

Another reason to accept this “inverted” labeling is the **supremacy of quantum theory**: the classical world emerges from quantum principles. In our terminology, higher-level (quantum) structures generate lower-level (classical) ones. To clarify what “classical” means, let’s note:

- Technically, it refers to a *specific permissible physical scenario* — for example, a unique trajectory. In discrete causal theories, such scenarios are determined from the axioms rather than from equations of motion. Histories satisfying these axioms are *permissible* and treated equally; those that don’t are excluded.  
- Conventionally, “classical” describes anything measurable at large scales and low energies. Bohr’s correspondence principle formalizes this:  
  > “The predictions of classical and quantum mechanics agree in the limit of large quantum numbers.” <d-cite key="French1979"></d-cite>

Hence, quantum and classical theories are equally fundamental but describe different structural levels. The quantum structure is **more complete**, encompassing all possible scenarios, while the classical structure isolates a single one.

---

## How to Model a Picture with an Equation?

The hierarchical structure we’ve discussed naturally defines a **structured configuration space** — a *kinematic scheme* encoded by sequential evolutionary processes. A configuration space represents all possible states of a system.  

For example, in classical mechanics, a particle’s position is given by coordinates $(x, y, z)$. To describe motion, we use two sets of coordinates $(x_1, y_1, z_1)$ and $(x_2, y_2, z_2)$, forming a function $\psi(x_1, y_1, z_1, x_2, y_2, z_2)$ which lives in a six-dimensional configuration space.  

By generalizing this concept through a *path-summation* approach, any quantum object can be represented in such a space. To “model a picture with an equation,” we sum contributions from all possible paths in this configuration space — after translating structural points into appropriate mathematical objects. This process yields quantum amplitudes and observables, forming a predictive framework that emerges naturally from the underlying causal structure of events. The resulting algebraic framework produces the **dynamical laws** of the theory.

---

### Causal Schrödinger-Type Equations

In non-relativistic quantum mechanics, the time-dependent Schrödinger equation is:

$$
\begin{align*}
\mathrm{i}\hbar \frac{d\psi}{dt} = \hat{H}\psi.
\end{align*}
$$

Here $\psi$ is the state function (an element of Hilbert space) and $\hat{H}$ is the Hamiltonian operator.  

Analogously, the **causal Schrödinger-type equation** <d-cite key="Dribus2017"></d-cite> is:

$$
\begin{align*}
\psi^{-}_{R;\theta} = \theta(r) \sum_{r^{-} \prec r} \psi^{-}_{R;\theta}(r^{-}).
\end{align*}
$$

Here:
- $\psi^{-}_{R;\theta}$ — generalized past-state function  
- $\theta(r)$ — relation function (analogous to the Lagrangian)  
- $R$ — a subobject in configuration space containing *co-relative histories* for elements $r$ and $r^{-}$  
- $r^{-} \prec r$ — denotes that $r^{-}$ precedes $r$ (encodes **causality**)  

This equation can also be viewed as a **discrete heat equation**, for reasons analogous to the Schrödinger equation in conventional quantum theory. If this equation holds, it should in principle contain sufficient information to recover continuum structures — that is, quantum field theory and Einstein’s equations — from the discrete spacetime foundation. We’ll explore this path further in the next few posts, beginning with **metric recovery theorems**.

---