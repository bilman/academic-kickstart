---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Rogue Wave Formation and Asymptotics for Large-Order Coherent Structures"
summary: "Asymptotic properties of large-order coherent structures in nonlinear integrable wave models and dynamical stability properties of rogue waves."
authors: []
tags: []
categories: []
date: 2020-05-07T20:21:13-04:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: true

header:
  image: ""
  caption: ""

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
In the article [A Robust IST for the Focusing NLS Equation]({{< ref "/publication/new-ist.md" >}}), we introduced a **robust** inverse scattering transform (IST) that can handle arbitrary spectral singularities or poles of arbitrary order in a simple and unified way. With this development, we now for the first time have Riemann-Hilbert (RH) problem representations for solutions of the nonlinear Schrödinger equation that may involve coherent structures such as

- **rogue waves**: Peregrine breather and its higher-order generalizations, which are (pseudo-rational) solutions associated with higher-order singularities at the branch points of the continuous spectrum of the associated Zakharov-Shabat operator - see the description of the preceding project [A Robust Inverse Scattering Transform for Arbitrary Spectral Singularities]({{< ref "project/spectral-singularities.md" >}})

![High-order rogue wave](img/nls-n8-rw-density-temp.png)

- **multi-pole solitons**: also reflectionless solutions, which are associated with $N^{\text{th}}$-order ($N\geq 2$, $n\in\mathbb{Z}$) pole singularities in the complement of the continuous spectrum
![Multi-pole soliton](img/nls-n4-soliton.png)

In [Extreme Superposition: Rogue Waves of Infinite Order and the Painlevé-III Hierarchy]({{< ref "/publication/extreme-superposition.md" >}}) we establish the existence of a limiting profile of rogue waves in the limit of large order when the solution is viewed in appropriate rescaled variables capturing the near-field region where the solution has the largest amplitude. The limiting profile is a new particular solution (the $\Psi^{\pm}$ function) of the focusing nonlinear Schrödinger equation in the rescaled variables - **the rogue wave of infinite order** - which also satisfies ordinary differential equations with respect to space and time. The spatial differential equations are identified with certain members of the Painlevé-III hierarchy.

Time evolution of the rogue wave of infinite order $\Psi(X,T)$ can be seen in the video below:

![The rogue wave of infinite order](img/extreme_featured.gif)

In [Extreme Superposition: Rogue Waves of Infinite Order and the Painlevé-III Hierarchy]({{< ref "/publication/extreme-superposition.md" >}}) we also compute the far-field asymptotic behavior of the near-field limit solution and compare the asymptotic formulæ with the exact solution with the help of numerical methods for solving Riemann-Hilbert problems. In a certain transitional region for the asymptotics the near field limit function is described by a specific globally-defined tritronqueé solution of the Painlevé-II equation. These properties lead us to regard the rogue wave of infinite order as **a new special function**, the $\Psi^{\pm}$ function, characterized by its Riemann-Hilbert problem representation given in [Extreme Superposition: Rogue Waves of Infinite Order and the Painlevé-III Hierarchy]({{< ref "/publication/extreme-superposition.md" >}}).

In [Large-order asymptotics for multiple-pole solitons of the focusing nonlinear Schrödinger equation]({{< ref "/publication/multipole-nls.md" >}}) we establish that the very same $\Psi^{\pm}$ function describes the near-field asymptotics coalescing multi-pole solitons (on a zero-background) as the order of the pole becomes large under a certain choice of norming constants. In general, the near-field behavior is again given in terms of certain members of the Painlevé-III hierarchy, albeit with different boundary conditions, having $\Psi^\pm$ as a special case. In this work we also compute the boundary of quiescent regions exactly, and use the nonlinear steepest-descent method to prove the asymptotic limit of the solitons is zero in these regions.
