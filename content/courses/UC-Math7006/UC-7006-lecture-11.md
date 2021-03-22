---
title: "Wave Equation"
linktitle: Lecture 11
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  Math7006:
    parent: Lecture Notes
    weight: 11

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 11
---
In this lecture we begin the treatment of the wave equation
$$
u_{tt} - \Delta u =0
$$
on $\mathbb{R}^n \times (0,\infty)$. We first consider the case in one spatial dimensions and obtain D'Alembert's solution formula for the solution of the initial-value problem

$$
\left\\{
\begin{alignedat}{2}
u_{tt} -\Delta u &= 0\quad &&\text{in}~\mathbb{R} \times(0,\infty)\\\ u=g\quad u_t&=h&&\text{on}~\mathbb{R} \times \\{t=0\\}
\end{alignedat}
\right.
$$

We then move on to the initial-boundary value problem posed on the half-line, that is,
$$
\left\\{
\begin{alignedat}{2}
u_{tt} -\Delta u &= 0\quad &&\text{in}~\mathbb{R}_+ \times(0,\infty)\\\ u=g\quad u_t&=h&&\text{on}~\mathbb{R}_+ \times \\{t=0\\}\\\ u&=0 \quad &&\text{on}~\\{x=0\\}\times (0,\infty)
\end{alignedat}
\right.
$$
where $\mathbb{R}_+ :=(0,\infty)$, and obtain a representation for its solution.

### Spherical Means

Finally, we introduce the **spherical means**
$$
\begin{aligned}
U(x;r,t)&:=\frac{1}{\mathrm{surf}(\partial B(x;r))}\int\limits_{\partial B(x;r)} u(y,t)\\, \mathrm{d}S_y\\\ G(x;r)&:=\frac{1}{\mathrm{surf}(\partial B(x;r))}\int\limits_{\partial B(x;r)} g(y)\\, \mathrm{d}S_y\\\ H(x;r)&:=\frac{1}{\mathrm{surf}(\partial B(x;r))}\int\limits_{\partial B(x;r)} h(y)\\, \mathrm{d}S_y
\end{aligned}
$$

for the problem (IVP) posed on $\mathbb{R}^n \times (0,\infty)$
$$
\left\\{
\begin{alignedat}{2}
u_{tt} -\Delta u &= 0\quad &&\text{in}~\mathbb{R}^n \times(0,\infty)\\\ u=g\quad u_t&=h&&\text{on}~\mathbb{R}^n \times \\{t=0\\}
\end{alignedat}
\right.
$$
and show that they satisfy Euler-Poisson-Darboux equation:

Fix $x\in\mathbb{R}^n$, let $u\in C^m(\mathbb{R}^n\times[0,\infty])$ satisfy (IVP). Then $U\in C^m\left(\overline{\mathbb{R}}_+\times[0,\infty]\right)$ and

$$
\left\\{
\begin{alignedat}{2}
U_{tt} -U_{rr} -\frac{n-1}{r} U_{r}&= 0\quad &&\text{in}~\mathbb{R}_+ \times(0,\infty)\\\ U=G\quad U_t&=H&&\text{on}~\mathbb{R}_+ \times \\{t=0\\}
\end{alignedat}
\right.
$$

## Full Set of Lecture Notes

[The notes for this lecture are available here (12 pages).](https://www.dropbox.com/s/rftlegrr5mja2gl/uc-MATH7006-Lec-11-Wave-Eqn-Intro.pdf?dl=0)
