---
title: Poisson's Equation
linktitle: Lecture 4
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  Math7006:
    parent: Lecture Notes
    weight: 4

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 4
---
This lecture considers Poisson's equation
$$
-\Delta u = f\quad \text{in}~ \mathbb{R}^n,
$$
where $f\colon \mathbb{R}^n \to \mathbb{R}$ is a given function. We cover some essential identities and theorems from calculus such as **Gauss' (Divergence) Theorem** and **Green's identities**. We prove the following. Let
$$
u(x):= \int\limits_{\mathbb{R}^n} \Phi(x-y) f(y)\\,\mathrm{d}y,
$$
where $\Phi$ is the fundamental solution of Laplace's equation constructed in [Lecture 3]({{< ref "/courses/UC-Math7006/UC-7006-lecture-3.md" >}}) and $f\in C^2_\mathrm{c}(\mathbb{R}^n)$. Then

1. $u\in C^2(\mathbb{R}^n)$.

2. $-\Delta u = f$ in $\mathbb{R}^n$


## Full Set of Lecture Notes

[The notes for this lecture are available here (21 pages).](https://www.dropbox.com/s/8u0f5xu8iiqvbmi/uc-MATH7006-Lec-4-Poissons-Equation.pdf?dl=0)
