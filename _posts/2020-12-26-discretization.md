---
title: 'Numerical discretization for active scalar field theory'
date: 2020-12-26
permalink: /posts/2020/12/discretization/
tags:
  - active matter
---

In this blog post, we will discuss the numerical implementation of active scalar field theory, in particular Active Model B+. Various discretization scheme for spatial derivatives will be discussed.

## Active model B+

Here we will consider the active model B+, which is a model for phase-separation in active matter (see [previous post]).
We consider a scalar order parameter $\phi(\mathbf{r},t)$. The free energy is given by:

$$ F[\phi] = \int dV\left\{ - \frac{A}{2}\phi^{2} + \frac{A}{4}\phi^{4} + \frac{K}{2}|\nabla\phi|^{2} \right\} $$

The dynamics for active model B+, is given by (see [Tjhung, Nardini, Cates, _PRX_, (2018)]):

$$ \frac{\partial\phi}{\partial t} = \underbrace{\nabla^{2}}_{(3)}(-A\phi+A\phi^{3}-K\underbrace{\nabla^{2}\phi}_{(2)})+\sqrt{2D}\underbrace{\nabla\cdot}_{(1)}\boldsymbol{\Lambda} \underbrace{\nabla\cdot}_{(4)}(\zeta\underbrace{(\nabla^{2}\phi)}_{(2)}\underbrace{\nabla}_{(4)}\phi - \underbrace{\nabla}_{(4)}(\lambda|\underbrace{\nabla}_{(4)}\phi|^{2})) $$

where $\lambda$ and $\zeta$ are the activity parameters. ($\lambda=\zeta=0$) corresponds to the passive/equilibrium limit.) The last two terms (proportional to $\lambda$ and $\zeta$) above are the non-equilibrium terms. $\boldsymbol{\Lambda}$ is Gaussian white noise with zero mean and delta-function correlation:

$$ \left<\Lambda_\alpha(\mathbf{r},t)\Lambda_\beta(\mathbf{r}',t')\right> = \delta_{\alpha\beta}\delta(\mathbf{r}-\mathbf{r}')\delta(t-t') $$

Numerically, we have to discretize the Laplacian and gradient operator in the $\phi$-dynamics. First, for derivatives in (1), we must use higher order derivatives. This is because the noise is of order $\sqrt{\Delta t/\Delta x\Delta y}$ so we need to be accurate in the derivatives:

$$ \partial_{x}\phi = \frac{\frac{1}{280}\phi_{i-4,j} - \frac{4}{105}\phi_{i-3,j}+\frac{1}{5}\phi_{i-2,j} - \frac{4}{5}\phi_{i-1,j} +\frac{4}{5}\phi_{i+1,j} - \frac{1}{5}\phi_{i+2,j} + \frac{4}{105}\phi_{i+3,j} - \frac{1}{280}\phi_{i+4,j}}{\Delta x} $$

For derivative in (3), we apply (1) twice to ensure detailed balance exactly on the lattice.

For Laplacian in (2) and the gradients in (4), we use the isotropic form of the numerical Laplacian and gradients because we nucleate small bubbles, which is bad for _∇<sup>2</sup>ϕ_ (see [Pooley, Furtado, _PRE_, (2007)]):

$$ \nabla^{2}\phi=\frac{1}{\Delta x\Delta y}\left[\begin{array}{ccc}
-\frac{1}{2} & 2 & -\frac{1}{2}\\
2 & -6 & 2\\
-\frac{1}{2} & 2 & -\frac{1}{2}
\end{array}\right]\phi_{ij} $$

$$ \partial_x\phi=\frac{1}{\Delta x}\left[\begin{array}{ccc}
-\frac{1}{10} & 0 & \frac{1}{10}\\
-\frac{3}{10} & 0 & \frac{3}{10}\\
-\frac{1}{10} & 0 & \frac{1}{10}
\end{array}\right]\phi_{ij} $$

Source code is available here [source code].

[previous post]: https://elsentjhung.github.io/posts/2019/04/active/
[Tjhung, Nardini, Cates, _PRX_, (2018)]: https://journals.aps.org/prx/abstract/10.1103/PhysRevX.8.031080
[Pooley, Furtado, _PRE_, (2007)]: https://journals.aps.org/pre/abstract/10.1103/PhysRevE.77.046702
[source code]: https://github.com/elsentjhung/active-model-B-plus
