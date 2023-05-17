---
layout: page
title: Tutorial
---

This tutorial is aimed at PhD students and postdocs who are going to do research in Theoretical Soft Condensed Matter Physics and Statistical Physics.
(This page is work in progress and will be updated periodically.)

---

### 0. Programming languages

You should learn at least one high level programming language _e.g._ Python, and one low level programming language, _e.g._ C or C++. 
This tutorial assumes knowledge of Python.

#### 0.1. Python

Python is a modern object-oriented programming language and widely used in scientific research and other industry such as data science, banking, machine learning, _etc_. Python also has a vast library to do numerical computation and plotting. Reference: [Python Crash Course].

#### 0.2. C or C++

Programs written in C usually run 10 times faster compared to the same programs written in Python.
C also gives users more low-level control, such as memory management. Reference: [C Programming Absolute Beginner's Guide].

---

### 1. Essential mathematics

This section contains several concepts in mathematical methods that might be useful.

#### 1.1. Fourier series, Fourier transform, and fast Fourier transform

Do you play a musical instrument? do you want to refresh your Python? do you want to learn Fourier transform? Then this jupyter notebook will teach you all of the above [sound wave and Fourier transform notebook].

<img src="https://elsentjhung.github.io/figures/Fourier-transform.jpg" alt="drawing" width="800"/>

---

### 2. Brownian motion

Brownian motion is the jittery motion of micron-sized particles in a fluid.
These particles do not sit still and instead they are being bombarded by even smaller fluid molecules.
These random kicks from the fluid molecules can be approximated as random force, which we will model below mathematically as a stochastic process.

#### 2.1. Langevin equation

(Work in progress.)

---

### 3. Binary fluid

In this section, we will start with the Cahn-Hilliard equation, which is a model for phase-separation in a binary fluid, _e.g._ water/oil phase separation, liquid/gas phase separation, and so on. 
Then we will extend the Cahn-Hiliard equation to include momentum conservation (Cahn-Hilliard-Navier-Stokes equation) and noise (model B equation).

#### 3.1. Cahn-Hiliard equation

In this tutorial, we will introduce the order parameter, the coarse-grained free energy and the time evolution of the order parameter. 
We will also look at the equilibrium phase diagram and the linear stability analysis of the homogenous phase. 
The link to the jupyter notebook is here [Cahn-Hiliard notebook].

<img src="https://elsentjhung.github.io/figures/coarsening.jpg" alt="drawing" width="800"/>

#### 3.2. Droplet

In this tutorial, we will derive the macroscopic properties of a droplet, such as surface tension, pressure, contact angle _etc_, from the free energy. 
The link to the jupyter notebook is here [droplet notebook].

<img src="https://elsentjhung.github.io/figures/affine-deformation.jpg" alt="drawing" width="800"/>

#### 3.3. Adding noise (equilibrium model B)

When the droplets are very small (~microns), thermal fluctuations become important. For instance, the droplet might undergo a Brownian motion like the colloidal particle described in the previous section. In this tutorial, we will add thermal noise to the Cahn-Hiliard equation and study the statistics of this noisy dynamics.
The link to the jupyter notebook is here [model B notebook].

<img src="https://elsentjhung.github.io/figures/structure-factor.jpg" alt="drawing" width="800"/>

---

[sound wave and Fourier transform notebook]: https://nbviewer.org/github/elsentjhung/sound-wave-analyser/blob/master/sound_analyser.ipynb

[Cahn-Hiliard notebook]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-coarsening/blob/master/coarsening.ipynb

[droplet notebook]: https://nbviewer.org/github/elsentjhung/cahn-hilliard-droplet/blob/master/droplet.ipynb

[model B notebook]: https://nbviewer.org/github/elsentjhung/equilibrium-model-B/blob/master/model_B.ipynb

[Python Crash Course]: https://www.amazon.co.uk/Python-Crash-Course-Hands-Project-Based/dp/1593276036/ref=sr_1_3?crid=3PW3644NJJAFI&keywords=Eric+Matthes+python&qid=1668365923&sprefix=eric+matthes+python%2Caps%2C153&sr=8-3

[C Programming Absolute Beginner's Guide]: https://www.amazon.co.uk/Programming-Absolute-Beginners-Guide-Guides/dp/0789751984/ref=sr_1_1?keywords=c+programming+absolute+beginner%27s+guide&qid=1668365982&sprefix=c+programming+abso%2Caps%2C160&sr=8-1
