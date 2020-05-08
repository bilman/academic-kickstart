---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Numerical Inverse Scattering Transforms"
summary: "Making solutions of integrable nonlinear dispersive wave equations computationally available to the nonlinear waves community using their Riemann-Hilbert problem representations via developing numerical inverse scattering transform tools. Riemann-Hilbert problems play the role of Fourier-type integral representations we have for solutions of linear problems."
authors: []
tags: []
categories: []
date: 2020-05-07T20:21:52-04:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "A purely dispersive solution of the Toda lattice computed at $t=10000$."
  focal_point: ""
  preview_only: true

header:
  image: "TodaSolution300.png"
  caption: "A purely dispersive solution of the Toda lattice computed at $t=10000$."
# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---
A modern approach is to consider solutions of $(1+1)$-dimensional nonlinear integrable models of wave propagation as **nonlinear special functions** that have their **Riemann-Hilbert problem representations** just as classical special functions (e.g. Airy, Bessel functions) have their integral representations. Riemann-Hilbert problems provide non-commutative analogues of integral representations.

## Goal

To compute physically interesting solutions of various integrable systems available using their Riemann-Hilbert problem representations and make these solutions computationally available to researchers in nonlinear waves community via a [Julia](http://www.julialang.org) package in an asymptotically robust way.

## Background

In 2012, [Sheehan Olver](http://wwwf.imperial.ac.uk/~solver/) developed a numerical framework to solve Riemann-Hilbert problems in context of computation of Painlevé-II transcendents ([RHPACKAGE](https://github.com/dlfivefifty/RHPackage)). Following this development, [Bernard Deconinck](http://depts.washington.edu/bdecon/bernard/)-[Sheehan Olver](http://wwwf.imperial.ac.uk/~solver/)-[Thomas Trogdon](https://www.math.uci.edu/~ttrogdon/) introduced a numerical framework to compute solutions of nonlinear integrable $(1+1)$-dimensional dispersive partial differential equations, starting with the Korteweg-de Vries (KdV) and modified KdV (mKdV) equations in 2014, and then focusing and defocusing nonlinear Schrödinger (NLS) equations. The numerical methodology developed is based on solving the Riemann-Hilbert problem that represents the solution of the PDE for a given $(x,t)$ through the associated inverse scattering transform. With the implementation of the Deift-Zhou method of nonlinear steepest descent, this framework can compute solutions of such dispersive PDEs in the entire $(x,t)$-plane with remarkable accuracy, in particular for arbitrarily large values of $t$, in an asymptotically robust way.  All of these modules are publicly available under the Mathematica package [ISTPACKAGE](https://bitbucket.org/trogdon/istpackage/src) written and maintained by [Thomas Trogdon](https://www.math.uci.edu/~ttrogdon/).

I joined the workforce in 2015 to compute solutions of the initial value problem for the doubly-infinite Toda lattice on the entire $(n,t)$-domain, including long-time asymptotic regions that were not previously studied (see [Numerical Inverse Scattering Transform for the Toda Lattice]({{< ref "/publication/toda-nist.md" >}})) and I am one of the contributors of the [ISTPACKAGE](https://bitbucket.org/trogdon/istpackage/src) since then.

## Advantages of Numerical IST
As variables $(x,t)$ of the PDE (or $(n,t)$ of a P$\Delta$E) appear only as explicit parameters in the Riemann-Hilbert problem,

+ no time-stepping or spatial discretization is necessary to compute the solution of the Cauchy problem under study,
+ presence of high-frequency oscillations in the spatial variable is no longer a numerical challenge; in fact, such aspects become completely irrelevant,
+ the numerical procedure is **immediately parallelizable** (a so-called "embarrassingly parallel" computation).


## Current work
 Current work is on

 + computing dispersive shock wave solutions (resulting from initial data with a step-like boundary values at infinity) of the Korteweg-de Vries (KdV) equation in arbitrarily large time-scales,
 + investigating and computing presence of solitons trapped in a rarefaction fan solution of the KdV equation.

This project involves collaboration with [Thomas Trogdon](https://www.math.uci.edu/~ttrogdon/).
