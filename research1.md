---
layout: page
title: Research 1
permalink: /research1/
---

## Time reversal symmetry breaking

In statistical physics we often say this system is in equilibrium and that system is out-of-equilibrium _et cetera_. But what is equilibrium? and what is out-of-equilibrium?

We say that a system is in equilibrium if it respects time reversal symmetry (TRS) at steady state and out-of-equilibrium if it violates TRS at steady state. For example, consider the pedestrations on Champs Elysee. They clearly constitute a non-equilibrium system because if we watch the movie backwards they will appear to walk backwards. 

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/_figures/people1.png" alt="drawing" width="800"/>

But now suppose we pay half the people 5€ each to walk backwards. They now become an equilibrium system because if we watch the movie backwards they look exactly the same

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/_figures/people2.png" alt="drawing" width="800"/>

## Active field theories

Probably we are familiar with the Cahn-Hiliard equation:

<img src="http://latex.codecogs.com/svg.latex?\frac{\partial\phi}{\partial t}+\nabla\cdot\left(-\nabla\frac{\delta F}{\delta\phi}+\boldsymbol{\Lambda}\right)=0" border="0"/>

In the equation above, _ϕ_ is the density of the fluid. If we start from a homogenous density _ϕ = -0.6_, the system will phase-separate into high density _ϕ = +1_ (liquid) and low density _ϕ = -1_ (vapour) phase. In steady state _t = ∞_, we end up with a single big blob of liquid.

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/_figures/MB.png" alt="drawing" width="1200"/>

Introducing the non-equilibrium Cahn-Hiliard equation....

<img src="http://latex.codecogs.com/svg.latex?\frac{\partial\phi}{\partial t}+\nabla\cdot\left( -\nabla\frac{\delta F}{\delta\phi} + \boldsymbol{\Lambda} + \lambda\nabla|\nabla\phi|^2 + \zeta(\nabla^2\phi)\nabla\phi \right)=0" border="0"/>

If we start from the same intial configuration, we see similar phenomena where the fluid phase-separate into high density and low density. However in the steady state, we get a boiling droplet. The droplet is in _perpetual_ boiling state, which is not possible in equilibrium because all the liquid will be evaporated.

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/_figures/AMB+.png" alt="drawing" width="1200"/>

<video src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/_movies/boiling-droplet.mov" controls="controls" width="480" height="480" />




