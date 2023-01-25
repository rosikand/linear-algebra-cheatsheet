---
title: "Linear Algebra Cheatsheet"
format:
  html:
    toc: true
    css: styles.css
    mainfont: sans-serif  # alt: system-ui 
    # minimal: true
  pdf: 
    documentclass: article
---

 
:::{.callout-note collapse='true'}

### Eventual outline 

- **Part 1: Vectors** 
	- Vectors 
	- Plane geometry 
	- Generalizing beyond $\mathbf{R}^3$: vector spaces 
	- Projections 
	- Gram-Schmidt 
	- Applications of projections: linear regression least squares  
- **Part 2: Matrices** 
	- Linear transformations (as matrices)
	- Types of linear transformations (geometric perspective) 
	- Matrix multiplication 
		- Maybe: application: Markov chain/linear dynamical systems 
	- Matrix algebra rules (transpose, various indentities, etc.)
	- Special matrices (symmetric, orthogonal, etc.) 
- **Part 3: Linear systems** 
	- Matrix inverses 
	- Systems of equations as matrices 
	- LU and QR decompositions 
- **Part 4: Further matrix algebra (or name this eigenvalues)** 
	- Eigenvalues and eigenvectors 
	- Spectral theorem (diagonolization) and definiteness of symmetric matrices 
	- Singular value decomposition 
	- The Hessian and the second derivative test 
- **Part 5: Matrix calculus and optimization** 
	- Aside: Lagrange multipliers (constrained optimization) 
	- Calculus with vectors and matrices 
		- Gradient, Jacobian, Hessian, chain rule   
	- Basics of convex functions and optimization 
	- Momentum 
	- Extra: 
		- [Gauss-Newton method](http://ee263.stanford.edu/lectures/gauss_newton.pdf)
		- CS 205L stuff 
:::
 


## I. Vectors 
 
::: {#def-default}

## $\mathbf{R}^2$, $\mathbf{R}^3$, $\mathbb{R}^n$

The set $\mathbf{R}^2$ is the set of all ordered pairs of real numbers ($\mathbf{R}^2=\{(x, y): x, y \in \mathbf{R}\}$). The set itself should be thought of as a plane (i.e. the xy-cartesian plot). The set $\mathbf{R}^3$ is the set of all ordered triples of real numbers ($\mathbf{R}^3=\{(x, y, z): x, y, z \in \mathbf{R}\}$). The set itself should be thought of as ordinary space. This generalizes to higher dimensions ($\mathbf{R}^n$). 

:::