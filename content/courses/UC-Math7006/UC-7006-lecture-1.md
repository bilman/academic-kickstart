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

Let $u$ be a function of several variables $u(x_1,x_2,\ldots,x_n)$. We say $u$ is **smooth** provided $u$ is infinitely differentiable with respect to all of the variables. We denote partial derivative of $u$ with respect to $x_k$ by
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

We express a general $k^{\text{th}}$ order PDE in the form
$$
F(x, u, Du, D^2 u, \ldots, D^k u)=0
$$
for some function $F$.

### Classification

A PDE of order $k$ is **linear** if it is of the form
$$
\sum_{|\alpha|\leq k} a_{\alpha}(x)D^{\alpha} u = 0.
$$
If $u_1$ and $u_2$ are two solutions of a linear PDE, then so is any linear combination $c_1 u + c_2 u_2$, $c_1$ and $c_2$ are constants.

We say a PDE is **nonlinear** if it is not linear.

A nonlinear PDE of order $k$ is **semilinear** if it is linear in the highest-order derivatives. In other words, if it is of the form:
$$
\left(\sum_{|\alpha|=k} a_{\alpha}(x) D^{\alpha} u \right) + a_0 \left(D^{k-1}u, D^{k-2}u,\ldots, Du, u, x \right)=0.
$$
As you can see, the coefficients of the terms with the highest-order derivatives are allowed to depend only on $x$.

A PDE of order $k$ is **quasilinear** if it is of the form

$$
\left(\sum_{|\alpha|=k} a_{\alpha}(D^{k-1}u,D^{k-2}u,\ldots, Du,u,x)D^{\alpha} u \right) + a_0 \left(D^{k-1}u, D^{k-2}u,\ldots, Du, u, x \right)=0
$$
but it is not semilinear. This means that in a quasilinear PDE, the highest-order derivatives $D^\alpha$, $|\alpha|=k$ are allowed to be multiplied by terms involving derivatives of lower orders.

A PDE order $k$ is **fully nonlinear** if it is nonlinear but not quasilinear or semilinear. In this case the highest order derivatives of $u$ themselves appear nonlinearly in the PDE.

#### Examples

* Airy's equation: $u_t + u_{xxx} = 0$; linear.

* Korteweg-de Vries equation: $u_t + u u_x + u_{xxx} = 0$; semilinear.

* Inviscid Burger's equation: $u_t + uu_x=0$; quasilinear.

* Eikonal equation: $u_x^2 +u_y^2 = c^2$; fully nonlinear.

## Main Goals and Motivations in Studying PDEs

Just like ordinary differential equations, a partial differential equation may have no solution, or infinitely many solutions.

#### Example
Consider $u_t - u_x =0$. $u(x,t):=0$ is a solution. So is $u(x,t):=C$ for any constant $C\in \mathbb{R}$. So is $u(x,t):= x+t$, and actually, so is $u(x,t):= C_1(x+t)+C_2$ for any constants $C_1,C_2\in\mathbb{R}$.

We impose auxiliary conditions, e.g. initial conditions and boundary conditions, and pose a problem to pick a particular solution. For example,
$$
\left\\{
  \begin{alignedat}{2}
    u_t - u_x &= 0 \quad&& x\in\mathbb{R},~t>0\\\ u&=g \quad&& x\in\mathbb{R}
  \end{alignedat}
\right.
$$
where $g\colon \mathbb{R}\to \mathbb{R}$ is a given function. This is an initial-value problem.

### Well-Posedness

**Bad news:** Most PDEs cannot be solved in explicit form. Thus, most of the efforts are geared towards understanding existence, properties, and behavior of solutions.

Given a PDE problem such as the initial value-problem above, we focus on three main issues:

1. __Existence:__ the problem in fact has a solution.

2. __Uniqueness:__ this solution is unique.

3. __Continuous dependence on given data:__ the solution depends continuously on the data given under some appropriate norm.

If a PDE problem has all of the properties 1, 2, and 3 above, we say that the problem is **well-posed**.

### Notion of a Solution

What do we mean by solution of a PDE in general? Ideally, a solution to a $k^{\text{th}}$-order PDE is required to have continuous partial derivatives of all orders up to and including order $k$. Such a solution is called a **classical** solution. But it is often the case that one is interested in functions that satisfy a weaker formulation of the PDE, that is, solutions that are not required to be differentiable. Such solutions, loosely speaking, are called **weak solutions**, **distributional solutions**, or **integral solutions**, depending on the context of the treatment. We will give a brief introduction to such solutions and work with them when we cover shock theory for scalar conservation laws.

## Full Set of Lecture Notes

[The notes for this lecture are available here (12 pages).](https://www.dropbox.com/s/feaci3d2vwb8wnb/uc-MATH7006-Lec-1-Introduction.pdf?dl=0)



## Homework
[Homework 1 is posted.](https://www.dropbox.com/s/0h3eal4dvjvcv8r/Math-7006-Sp21-HW1.pdf?dl=0)
