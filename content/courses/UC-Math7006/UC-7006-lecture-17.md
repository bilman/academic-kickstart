---
title: "Scalar Conservation Laws"
linktitle: Lecture 17
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false

menu:
  Math7006:
    parent: Lecture Notes
    weight: 17

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 17
---
We being our treatment of **scalar conservation laws**:

$$
u_t + (F(u))_x = 0\quad \text{in}~\mathbb{R}^n\times(0,\infty)
$$
for $u=u(x,t)$, $u\colon \mathbb{R}\times(0,\infty)\to \mathbb{R}$. Here $F\colon \mathbb{R}\to \mathbb{R}$ is given. Our focus is the initial-value problem (IVP)

$$
\left\\{
\begin{alignedat}{2}
u_t + (F(u))_x &= 0 \quad&&\text{in}~\mathbb{R}\times(0,\infty)\\\ u&=g \quad &&\text{on}~\mathbb{R}\times\\{t=0\\}
\end{alignedat}
\right.
$$

We first observe that if $(F'\circ g)(\zeta)<0$ for some $\zeta\in\mathbb{R}$, the projected characteristic curves intersect at finite time, which result in formation of discontinuities and gradient catastrophe. We then introduce the notion of a **weak solution** (an integral solution) to allow for discontinuities. We then cover **Rankine-Hugoniot** condition, which imposes restrictions on the behavior of a weak solution at a curve of discontinuity.

We then illustrate non-uniqueness of weak solutions, state the **entropy condition** and provide a _glimpse_ of Lax-Oleinik theory, arriving at the definition of a **shock** and the notion of an **entropy solution**. We provide some examples as well.

## Full Set of Lecture Notes

[The notes for this lecture are available here (44 pages).](https://www.dropbox.com/s/3b7g2by4dmyq4f8/uc-7006-Lec-17-Conservation-Laws.pdf?dl=0)
