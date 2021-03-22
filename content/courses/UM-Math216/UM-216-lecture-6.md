---
title: Autonomous Equations and Population Dynamics
linktitle: Lecture 6
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  Math216:
    parent: Lecture Notes
    weight: 6

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 6
---
In this lecture we covered autonomous equations and population dynamics, introduced the **logistic equation** along with notions of **saturation capacity** and **threshold**. We also performed qualitative analysis for solutions of initial-value problems for such differential equations.

I most generality, the ODEs are of the form:
$$
\frac{\mathrm{d} y}{\mathrm{d} t}=-r\left(1-\frac{y}{T}\right)\left(1-\frac{y}{K}\right) y
$$
where $r$, $K$, and $T$ are positive constants with $T<K$.

## Jupyter Notebook
Please see the embedded Jupyter notebook below.

<iframe
      src="https://nbviewer.jupyter.org/github/bilman/Math216ODE/blob/master/216Lecture6.ipynb?flush_cache=true"
      width="100%"
      height="1000px"
      style="border:none;">
    </iframe>
