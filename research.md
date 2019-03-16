---
layout: page
title: Research 1
permalink: /research/
---

Current research interests: time reversal symmetry breaking in statistical field theory, active droplets, chiral liquid crystals, glasses, _etc_.

I use lattice Boltzmann simulation for fluid dynamics.

## Time reversal symmetry breaking

In statistical physics we often say this system is in equilibrium and that system is out-of-equilibrium _et cetera_. But what is equilibrium? and what is out-of-equilibrium?

We say that a system is in equilibrium if it respects time reversal symmetry (TRS) at steady state and out-of-equilibrium if it violates TRS at steady state. For example, consider the pedestrations on Champs Elysee. They clearly constitute a non-equilibrium system because if we watch the movie backwards they will appear to walk backwards. 

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/people1.png" alt="drawing" width="800"/>

But now suppose we pay half the people 5€ each to walk backwards. They now become an equilibrium system because if we watch the movie backwards they look exactly the same

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/people2.png" alt="drawing" width="800"/>

## Active field theories

So we are already familiar with the Cahn-Hiliard equation:

<img src="http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7B%5Cpartial%5Cphi%7D%7B%5Cpartial%20t%7D%20%2B%20%5Cnabla%5Ccdot%5Cleft%28%20-%5Cnabla%5Cfrac%7B%5Cdelta%20F%7D%7B%5Cdelta%5Cphi%7D%20%2B%20%5Cboldsymbol%7B%5CLambda%7D%20%5Cright%29%20%3D%200&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="\frac{\partial\phi}{\partial t} + \nabla\cdot\left( -\nabla\frac{\delta F}{\delta\phi} + \boldsymbol{\Lambda} \right) = 0" width="210" height="47" />

This equation describes full phase separation into low density (vapour) and high density phase (liquid). For example, suppose initially at time _t = 0_, the density is uniform everywhere. Then as time increases, liquid droplets are nucleated and coarsen with time. In steady state _t = ∞_, we end up with a single big drop of liquid.

For example, non-equilibrium Cahn-Hiliard equation can give rise to a perpetual boiling droplet.

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/boiling-droplet.jpg" alt="drawing" width="1200"/>



