---
title: "Statistical Physics of Soft Condensed Matter"
collection: teaching
type: "Graduate Course"
permalink: /teaching/soft-matter
venue: "The Open University"
date: 2023-01-01
location: "Milton Keynes, United Kingdom"
---

This is a graduate course in Statistical Physics and Soft Condensed Matter. This course is aimed at PhD students and postdocs who are going to do research in Theoretical Soft Condensed Matter Physics and Statistical Physics. 

## 0. Introduction

This course is an evolution of the Part III course in Cambridge of the same name, given by Prof. Cates, but with the added computational aspects. This course assumes some knowledge of Python (see [Python Crash Course] for reference). Entire course is written in Jupyter notebook.

## 1. Brownian motion

Brownian motion is the jittery motion of micron-sized particles in a fluid. These particles do not sit still and instead they are being bombarded by even smaller fluid molecules. These random kicks from the fluid molecules can be approximated as random force, which we will model below mathematically as a stochastic process.

### 1.1. Langevin equation

(Work in progress.)

## 2. Binary fluid

In this section, we will start with the Cahn-Hilliard equation, which is a model for phase-separation in a binary fluid, _e.g._ water/oil phase separation, liquid/gas phase separation, and so on. 
Then we will extend the Cahn-Hiliard equation to include momentum conservation (Cahn-Hilliard-Navier-Stokes equation) and noise (model B equation) to model droplet dynamics, droplet evaporation, microfluidics, and so on.

### 2.1. Cahn-Hiliard equation

In this tutorial, we will introduce the order parameter, the coarse-grained free energy and the time evolution of the order parameter. 
We will also look at the equilibrium phase diagram and the linear stability analysis of the homogenous phase. 
The link to the jupyter notebook is here: [Cahn-Hiliard notebook]. The PDF version is here: [Cahn-Hiliard pdf]. 

<img src="https://elsentjhung.github.io/images/coarsening.jpg" alt="drawing" width="800"/>

### 2.2. Droplet

In this tutorial, we will derive the macroscopic properties of a droplet, such as surface tension, pressure, contact angle _etc_, from the free energy. 
The link to the jupyter notebook is here: [droplet notebook]. The PDF version is here: [droplet pdf]. If one is interested, a short note about Noether's theorem can be found here: [Noether's Theorem pdf].

<img src="https://elsentjhung.github.io/images/affine-deformation.jpg" alt="drawing" width="800"/>

### 2.3. Adding noise (equilibrium model B)

When the droplets are very small (~microns), thermal fluctuations become important. For instance, the droplet might undergo a Brownian motion like the colloidal particle described in the previous section. In this tutorial, we will add thermal noise to the Cahn-Hiliard equation and study the statistics of this noisy dynamics.
The link to the jupyter notebook is here: [model B notebook]. The PDF version is here: [model B pdf]. 

<img src="https://elsentjhung.github.io/images/structure-factor.jpg" alt="drawing" width="800"/>


[Cahn-Hiliard notebook]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-coarsening/blob/master/coarsening.ipynb

[Cahn-Hiliard pdf]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-coarsening/blob/master/coarsening.pdf

[droplet notebook]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-droplet/blob/master/droplet.ipynb

[droplet pdf]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-droplet/blob/master/droplet.pdf

[Noether's Theorem pdf]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-coarsening/blob/master/Noether-Theorem.pdf

[model B notebook]: https://nbviewer.org/github/elsentjhung/equilibrium-model-B/blob/master/model_B.ipynb

[model B pdf]: https://nbviewer.org/github/elsentjhung/equilibrium-model-B/blob/master/model_B.pdf

[Python Crash Course]: https://www.amazon.co.uk/Python-Crash-Course-Hands-Project-Based/dp/1593276036/ref=sr_1_3?crid=3PW3644NJJAFI&keywords=Eric+Matthes+python&qid=1668365923&sprefix=eric+matthes+python%2Caps%2C153&sr=8-3

[C Programming Absolute Beginner's Guide]: https://www.amazon.co.uk/Programming-Absolute-Beginners-Guide-Guides/dp/0789751984/ref=sr_1_1?keywords=c+programming+absolute+beginner%27s+guide&qid=1668365982&sprefix=c+programming+abso%2Caps%2C160&sr=8-1
