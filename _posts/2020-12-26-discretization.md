---
layout: post
title: Numerical discretization for active scalar field theory
date: 2020-12-26
---

## Active model B+

Here we will consider the active model B+, which is a model for phase-separation in an active matter (see [previous post]).
We consider a scalar order parameter _ϕ(__r__,t)_. The free energy is given by:
<img src="http://latex.codecogs.com/svg.latex?F[\phi]=\int dV\left\{ -\frac{A}{2}\phi^{2}+\frac{A}{4}\phi^{4}+\frac{K}{2}|\nabla\phi|^{2}\right\}" border="0"/>

The dynamics for active model B+, is given by (see [Tjhung, Nardini, Cates, _PRX_, (2018)]):
<img src="http://latex.codecogs.com/svg.latex?\frac{\partial\phi}{\partial t}=\underbrace{\nabla^{2}}_{(3)}(-A\phi+A\phi^{3}-K\underbrace{\nabla^{2}\phi}_{(2)}+\lambda|\underbrace{\nabla}_{(1)}\phi|^{2})-\underbrace{\nabla\cdot}_{(1)}(\zeta\underbrace{(\nabla^{2}\phi)}_{(2)}\underbrace{\nabla}_{(1)}\phi)" border="0"/>
<img src="http://latex.codecogs.com/svg.latex?+\sqrt{2D}\underbrace{\nabla\cdot}_{(1)}\boldsymbol{\Lambda}" border="0"/>,

where _λ_ and _ζ_ are the activity parameters. (_λ=ζ=0_ corresponds to the passive/equilibrium limit.) __Λ__ is Gaussian white noise with zero mean and delta-function correlation:
<img src="http://latex.codecogs.com/svg.latex?\left<\Lambda_\alpha(\mathbf{r},t)\Lambda_\beta(\mathbf{r}',t')\right>=\delta_{\alpha\beta}\delta(\mathbf{r}-\mathbf{r}')\delta(t-t')" border="0"/>.

Numerically, we have to discretize the laplacian and gradient operator in the _ϕ_-dynamics. First, for derivatives in (1), we must use higher order derivatives. This is because the noise is of order <img src="http://latex.codecogs.com/svg.latex?\sqrt{\Delta t/\Delta x\Delta y}"/> so we need to be accurate in the derivatives:
<img src="http://latex.codecogs.com/svg.latex?\partial_{x}\phi & =\frac{\frac{1}{280}\phi_{i-4,j}-\frac{4}{105}\phi_{i-3,j}+\frac{1}{5}\phi_{i-2,j}-\frac{4}{5}\phi_{i-1,j}+\frac{4}{5}\phi_{i+1,j}-\frac{1}{5}\phi_{i+2,j}+\frac{4}{105}\phi_{i+3,j}-\frac{1}{280}\phi_{i+4,j}}{\Delta x}" border="0"/>.


[previous post]: https://elsentjhung.github.io/2019/04/07/active.html
[Tjhung, Nardini, Cates, _PRX_, (2018)]: https://journals.aps.org/prx/abstract/10.1103/PhysRevX.8.031080
