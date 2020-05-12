---
title: "Method of Characteristics"
linktitle: Lecture 15
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false

menu:
  Math7006:
    parent: Lecture Notes
    weight: 15

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 15
---
The method of characteristics was already employed to construct the solution of the (constant-coefficient) transport equation in [Lecture 2]({{< ref "/courses/UC-Math7006/UC-7006-lecture-2.md" >}}). We now begin the **general treatment of the method of characteristics** for general first-order PDEs.

We write a first order PDE for an unknown function $u$ as
$$
F(Du,u,x)=0.
$$
Here $x\in U$, where $U \subset \mathbb{R}^{n}$ is open, and $u\colon \overline{U} \to \mathbb{R}$. $F$ is of the form
$$
F\colon \mathbb{R}^n \times \mathbb{R} \times \overline{U} \to \mathbb{R}.
$$
and construct solutions of
$$
\left\\{
\begin{alignedat}{2}
F(Du,u,x) &= 0 &&\text{in}~U \\\ u&=g\quad &&\text{on}~\Gamma
\end{alignedat}
\right.
$$
where $\Gamma \subseteq \partial U$, and $g\colon \Gamma \to \mathbb{R}$ is given. $F$ and $g$ are as smooth as we like and the boundary $\partial U$ is $C^1$. We give several examples before a theoretical treatment.

{{< figure src="/img/characteristics.png" title="" lightbox="true" >}}

## Full Set of Lecture Notes

[The notes for this lecture are available here (24 pages).](https://www.dropbox.com/s/zlb6117r5jkggwm/uc-7006-Lec-15-Characteristics.pdf?dl=0)
