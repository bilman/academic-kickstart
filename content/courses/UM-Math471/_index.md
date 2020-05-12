---
# Course title, summary, and position.
linktitle: Introduction to Numerical Analysis (Math 471 at U. Michigan)
summary: An course on numerical analysis for seniors and Master's students which is a survey of the basic numerical methods which are used to solve scientific problems. Taught at the University of Michigan in Winter 2019. Accuracy, stability, and efficiency of the some of the basic methods are studied. The emphasis is evenly divided between the analysis of the methods and their practical applications. Some convergence theorems and error bounds are proved.
weight: 4

# Page metadata.
title: "Introduction to Numerical Analysis"
date: "2018-09-09T00:00:00Z"
lastmod: "2018-09-09T00:00:00Z"
draft: false  # Is this a draft? true/false
toc: true  # Show table of contents? true/false
type: docs  # Do not modify.

# Add menu entry to sidebar.
# - name: Declare this menu item as a parent with ID `name`.
# - weight: Position of link in menu.


menu:
  Math471:
    name: Overview
    weight: 1
---
{{< figure src="eniac.jpg" title="" lightbox="true" caption="ENIAC. Image Source: Wikipedia" >}}

This is a survey of the basic numerical methods which are used to solve scientific problems. A numerical method is an algorithm, or a sequence of steps, for solving a set of equations. These can be linear equations, nonlinear equations, or differential equations. We will study the accuracy, stability, and efficiency of the some of the basic methods. The emphasis is evenly divided between the analysis of the methods and their practical applications. Some convergence theorems and error bounds are proved. Scientific problems were traditionally investigated by theory and experiment, but now computer simulations are also being used in problems such as airplane design, weather prediction, modeling the spread of an epidemic, and improving the efficiency of solar cells, to cite just a few examples. There are software packages that can be used as a black box, but in this course we will look under the hood and see how the methods work.

The course also provides an introduction to MATLAB, an interactive program for numerical linear algebra, as well as practice in computer programming. One goal of the course is to show how calculus and linear algebra are used in numerical analysis.

## Textbook

A Friendly Introduction to Numerical Analysis, by _Brian Bradie_, Pearson, 2006, ISBN-13:978-0130130549

## Topics Covered
A tentative list of topics to cover are (the indicated chapters are from the textbook by Bradie):

* Chapter 1: Floating Point Arithmetic and Error Propagation (1.2–1.4)
* Chapter 2: Rootfinding (2.1–2.7)
* Chapter 3: Systems of Equations & Numerical Linear Algebra (3.1–3.10)
* Chapter 5: Interpolation (5.1–5.8)
* Chapter 6: Numerical Integration (6.3–6.7)
* Chapter 7: Numerical Methods for Differential Equations (7.1–7.6)
* Chapter 8: Two-Point Boundary Value Problems (time-permitting)

## Advice for Students

Questions are encouraged --- if something is unclear during class, please ask, ask, ask, ask. Review your the notes after each class and make a list of points that are unclear. Ask me about these points either in class or office hours. **Do not postpone understanding something**.

Be in full control of your work. When a code you wrote works (i.e. gives you the “desired answer”) for example, make sure you understand completely why it worked instead of abandoning it immediately.

Make the point above a habit. If you do not understand why a method, an algorithm, a piece of code works, you do not know know when it will fail. The consequences of such failures are known to be catastrophic:

* [Disasters Attributable to Bad Computing, by Doug Arnold](http://www-users.math.umn.edu/~arnold//disasters/disasters.html)

* [Collection of Software Bugs, by Thomas Huckle](https://www5.in.tum.de/~huckle/bugse.html)

## Homework Assignments

* [Homework 1](https://www.dropbox.com/s/v3upx9d4wwtssmv/M471-W19-HW1.pdf?dl=0)
* [Homework 2](https://www.dropbox.com/s/vm4putnuh5e41g1/M471-W19-HW2.pdf?dl=0)
* [Homework 3](https://www.dropbox.com/s/ggsk7dk81qpesm0/M471-W19-HW3.pdf?dl=0)
* [Homework 4](https://www.dropbox.com/s/c40spb0imbxw15u/M471-W19-HW4.pdf?dl=0)
* [Homework 5](https://www.dropbox.com/s/961tsasi49ads99/M471-W19-HW5.pdf?dl=0)
* [Homework 6](https://www.dropbox.com/s/cdmchohgtfa64ho/M471-W19-HW6.pdf?dl=0)
* [Homework 7](https://www.dropbox.com/s/wcb936ui2mxlkvn/M471-W19-HW7.pdf?dl=0)
* [Homework 8](https://www.dropbox.com/s/zrziuueix73bm62/M471-W19-HW8.pdf?dl=0)
* [Homework 9](https://www.dropbox.com/s/zrziuueix73bm62/M471-W19-HW9.pdf?dl=0)
* [Homework 10](https://www.dropbox.com/s/zrziuueix73bm62/M471-W19-HW10.pdf?dl=0)

## Lecture Notes

From the menu on the left, you may find a (n incomplete) set of lecture notes written using Jupyter (see Jupyter) notebooks. The scientific computing software used in Math 471 was _MATLAB_. The notes provided here are just a proper subset of what is covered in class and they are meant to be supplementary only. The interactive features (if any) work with web browsers Safari, Firefox, and Google Chrome as of now. Other browsers were not tested.


{{% staticref "files/courses/um-471/471IVPs.html" "newtab" %}}Download my CV{{% /staticref %}}
