---
title: Introduction
linktitle: Lecture 1
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
menu:
  Math7006:
    parent: Lecture Notes
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---
## Basic Definitions and Notation

Let $u$ be a function of several variables $u(x_1,x_2,\ldots,x_n)$. We say $u$ is _smooth_ provided $u$ is infinitely differentiable with respect to all of the variables. We denote partial derivative of $u$ with respect to $x_k$ by
$$
u_{x_k} := \frac{\partial u}{\partial x_k}
$$
We sometimes also write $\partial_{x_k}$ to denote the differential operator $\frac{\partial}{\partial x_k}$. With this notation, we may express mixed partial derivatives as
$$
u_{x_j x_k} = \frac{\partial^2 u}{\partial x_k \partial x_j} = \partial_{x_k} \partial_{x_j} u.
$$
We will for the most part be working with functions that have continuous partial derivatives and hence (by Clairaut-Schwarz's Theorem) assume that the partial derivatives commute:
$$
u_{x_j x_k}=u_{x_k x_j}.
$$
This assumption also provides us with a well-defined notation to express high-order derivatives. The _multi-index notation_ due to L. Schwartz.

### Multi-index Notation
A **multi-index** is a vector $\alpha=(\alpha_1,\ldots, \alpha_n)$ where each component $\alpha_j$ is a nonnegative integer. The **order of a multi-index** $\alpha$ is denoted by $|\alpha|$ and is defined by:
$$
|\alpha|:= \alpha_1 + \cdots + \alpha_n.
$$

Given a multi-index $\alpha$, we define
$$
D^{\alpha} u:=\frac{\partial^{|\alpha|} u}{\partial x_{1}^{\alpha_{1}} \cdots \partial x_{n}^{\alpha_{n}}}=\partial_{x_{1}}^{\alpha_{1}} \cdots \partial_{x_{n}}^{\alpha_{n}} u
$$

#### Example
Let $u$ be a function of 3 variables $(x,y,z)$ and $\alpha=(1,3,2)$. Then
$$
D^{\alpha} u= \partial_{x}\partial_{y}^3\partial_{z}^2 u = u_{xyyyzz}
$$
where both of the equalities uses the commutativity of the partial derivatives.

#### Example
If $u=u\left(x_{1}, \ldots, x_{n}\right)$, then $D^1u=\left\\{u_{x_{i}}\colon i=1, \ldots, n \right\\}$.

In practice, for $k$ non-negative integer, $D^k u$ denotes the set of all partial derivatives of $u$ of order $k$. Assigning a certain ordering we can regard $D^k u(x)$ for $x\in\mathbb{R}^n$ as a point in $\mathbb{R}^{n^k}$.

#### Special Cases
Let $x=(x_1,\ldots,x_n)\in\mathbb{R}^n$.
* $k=1$: In this case we have:
$$
D^1 u(x)=D u(x) =:(u_{x_1}(x),u_{x_2}(x),\ldots,u_{x_n}(x)),
$$
which is the gradient vector $\nabla u(x)$, hence $Du(x)\in\mathbb{R}^n$.

* $k=2$: In this case we regard the elements of $D^2u(x)$ as they are arranged in an $n\times n$ matrix:
$$
D^2u(x):=
\begin{bmatrix}
u_{x_1 x_1}(x) & &\cdots& & u_{x_1 x_n}(x) \\\ u_{x_2 x_1}(x) & &\cdots& & u_{x_2 x_n}(x)\\\ & &\cdots& & \\\ \vdots & &\cdots& & \vdots \\\ & &\cdots& & \\\ u_{x_n x_1}(x) & &\cdots& & u_{x_n x_n}(x)
\end{bmatrix}
$$
which is the Hessian matrix of $u$ at $x$, and hence $D^2u(x)\in S(n)$, the space of real symmetric $n\times n$ matrices. Note that in this case $\mathrm{tr}(D^2u(x))$ gives the Laplacian of $u$ at $x$ (in rectangular coordinates).

### Partial Differential Equations

A **partial differential equation** (PDE) is an equation involving a(n unknown) function $u$ of several variables and its partial derivatives. The **order** of a PDE is the order of the highest-order derivative in the PDE.

#### Examples

* Transport equation: $u_t + b\cdot Du = 0$, $b\in\mathbb{R}^n$; first order.

* Laplace's equation: $u_{xx}+ u_{yy} =0$; second order.

* Poisson's equation: $u_{xx}+ u_{yy} =f(x,y)$; second order.

* Heat equation: $u_t - u_{xx} =0$; second order.

* Wave equation: $u_{tt} - u_{xx} =0$; second order.

* Airy's equation: $u_t + u_{xxx} = 0$; third order.

* Korteweg-de Vries equation: $u_t + u u_x + u_{xxx} = 0$; third order.

* Eikonal equation: $u_x^2 +u_y^2 = c^2$; first order.


## Homework
[Homework 1 is posted.](https://www.dropbox.com/s/8qq67sf0l4jyuef/Math-7006-Sp20-HW1.pdf?dl=0)
