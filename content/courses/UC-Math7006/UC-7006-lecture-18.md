---
title: "Riemann's Problem & Applications"
linktitle: Lecture 18
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false

menu:
  Math7006:
    parent: Lecture Notes
    weight: 18

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 18
---
We continue our discussion with **Riemann's problem**, the initial value problem
$$
\left\\{
\begin{alignedat}{2}
u_t + (F(u))_x &= 0 \quad&&\text{in}~\mathbb{R}\times(0,\infty)\\\ u&=g \quad &&\text{on}~\mathbb{R}\times\\{t=0\\}
\end{alignedat}
\right.
$$
where $g$ is a piecewise-constant function
$$
g(x)=\begin{cases} u_L,& x<0 \\\ u_R,& x>0 \end{cases}
$$
with $u_L\neq u_R$. Assuming that $F$ is uniformly convex and $C^2$, we give the unique entropy solution of Riemann's problem for the cases $u_L < u_R$ and $u_L > u_R$.

We then give several examples with more general, piecewise-constant initial data.

## Full Set of Lecture Notes

[The notes for this lecture are available here (14 pages).](https://www.dropbox.com/s/kt7aoi04fb9xqhs/uc-7006-Lec-18-Riemann-prob-Applications.pdf?dl=0)

## Homework
[Homework 8 is posted.](https://www.dropbox.com/s/aitiuj0c85hyv3j/Math-7006-Sp20-HW8.pdf?dl=0)
