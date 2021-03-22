---
title: "Plane Waves, Traveling Waves, and Solitons"
linktitle: Lecture 19
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false

menu:
  Math7006:
    parent: Lecture Notes
    weight: 19

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 19
---
We end the semester with some **basic linear wave theory** and **solitons**.

![KdV Solitons](../img/kdvsolitons2.png)

We obtain linear dispersion relation for the plane wave solutions of several PDEs:

* heat equation
* wave equation
* Klein-Gordon equation
* Airy's equation

and introduce notions of **dispersion** and **dissipation**. Inline with this, we cover **phase velocity** for plane waves.

We then discuss what a **soliton** is along with a brief history of integrability in context of nonlinear wave equations, from John Scott Russell's observation of **the great wave of translation** in 1984 to the FPU recurrence at Los Alamos in 1950s, followed by Zabusky and Kruskal's discovery of a soliton in 1964, and the seminal paper of Gardner, Greene, Kruskal, and Miura in 1967.

We end the semester with calculating the famous $1$-soliton solution
$$
u(x,t)=\frac{\sigma}{2}\mathrm{sech}\left( \frac{\sqrt{\sigma}}{2}(x-\sigma t - c)\right)^2,
$$
$\sigma>0$, $c\in\mathbb{R}$, of the Korteweg-de Vries equation
$$
u_t + 6 u u_x + u_{xxx}=0.
$$

{{< figure src="../img/kdvsolitons.gif" title="" lightbox="true" >}}

## Full Set of Lecture Notes

[The notes for this lecture are available here (20 pages).](https://www.dropbox.com/s/hrzm29ngifhquoz/uc-7006-Lec-19-Similarity-Solutions.pdf?dl=0)
