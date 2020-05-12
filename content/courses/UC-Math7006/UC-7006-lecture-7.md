---
title: Energy Methods for Poisson's Equation
linktitle: Lecture 7
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  Math7006:
    parent: Lecture Notes
    weight: 7

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 7
---
In this lecture we cover **energy methods** for the boundary-value problem (BVP)
$$
\left\\{
\begin{alignedat}{2}
-\Delta u &= f\quad &&\text{in}~U\\\ u&=g\quad&&\text{on}~\partial U
\end{alignedat}
\right.
$$
We define the **energy functional**
$$
I[w]:= \int\limits_U \frac{1}{2} |D w(y)|^2 - w(y)f(y) \\, \mathrm{d}y
$$
for $w$ belonging to the admissible set
$$
\mathcal{A}:= \left\\{w\in C^2(\overline{U})~\vert~ w=g~\text{on}~\partial U\right\\}.
$$
and among other things, cover **Dirichlet's Principle**:

$u\in C^2(\overline{U})$ solves (BVP) if and only if $I[u]=\min_{w\in\mathcal{A}} I[w]$.

## Full Set of Lecture Notes

[The notes for this lecture are available here (6 pages).](https://www.dropbox.com/s/ws0phrmzo3ocjjx/uc-7006-Lec-7-Energy-Methods-Poisson.pdf?dl=0)

## Homework
[Homework 4 is posted.](https://www.dropbox.com/s/p8oeih2zg88fd9j/Math-7006-Sp20-HW4.pdf?dl=0)
