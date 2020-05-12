---
title: Heat Equation
linktitle: Lecture 8
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  Math7006:
    parent: Lecture Notes
    weight: 8

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 8
---
In this lecture we begin our treatment of the **heat equation**
$$
u_t - \Delta u = 0,
$$
where the unknown function is $u=u(x,t)$ with $u\colon \mathbb{R}^n\times(0,\infty)$. We construct the fundamental solution using dilation symmetry of the heat operator and then give a representation for solutions of the initial-value problem (IVP)
$$
\left\\{
\begin{alignedat}{2}
u_t -\Delta u &= 0\quad &&\text{in}~\mathbb{R}^n \times(0,\infty)\\\ u&=g\quad&&\text{on}~\mathbb{R}^n \times \\{t=0\\}
\end{alignedat}
\right.
$$
that is, we show that
$$
u(x,t):=(\Phi * g)(x,t)
$$
satisfies (IVP) and that $u \in C^{\infty}\left(\mathbb{R}^{n} \times(0, \infty)\right)$ provided $g\in C\left(\mathbb{R}^{n}\right) \cap L^{\infty}\left(\mathbb{R}^{n}\right)$.

We then move on to the treatment of the inhomogeneous problem and cover **Duhamel's principle**.

## Full Set of Lecture Notes

[The notes for this lecture are available here (16 pages).](https://www.dropbox.com/s/4t05seqduxa25k2/uc-7006-Lec-8-Heat-Eqn-Basics.pdf?dl=0)
