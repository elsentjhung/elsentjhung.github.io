---
layout: page
title: Research 1
permalink: /research1/
---

## Time reversal symmetry breaking

In statistical physics we often say this system is in equilibrium and that system is out-of-equilibrium _et cetera_. But what is equilibrium? and what is out-of-equilibrium?

We say that a system is in equilibrium if it respects time reversal symmetry (TRS) at steady state and out-of-equilibrium if it violates TRS at steady state. For example, consider the pedestrations on Champs Elysee. They clearly constitute a non-equilibrium system because if we watch the movie backwards they will appear to walk backwards. 

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/people1.png" alt="drawing" width="800"/>

But now suppose we pay half the people 5€ each to walk backwards. They now become an equilibrium system because if we watch the movie backwards they look exactly the same

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/people2.png" alt="drawing" width="800"/>

## Active field theories

Probably we are familiar with the Cahn-Hiliard equation:

<img src="http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7B%5Cpartial%5Cphi%7D%7B%5Cpartial%20t%7D%20%2B%20%5Cnabla%5Ccdot%5Cleft%28%20-%5Cnabla%5Cfrac%7B%5Cdelta%20F%7D%7B%5Cdelta%5Cphi%7D%20%2B%20%5Cboldsymbol%7B%5CLambda%7D%20%5Cright%29%20%3D%200&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="\frac{\partial\phi}{\partial t} + \nabla\cdot\left( -\nabla\frac{\delta F}{\delta\phi} + \boldsymbol{\Lambda} \right) = 0" width="210" height="47" />

In the equation above, _ϕ_ is the density of the fluid. If we start from a homogenous density _ϕ=-0.6_, the system will phase-separate into high density _ϕ=+1_ (liquid) and low density _ϕ=-1_ (vapour) phase. In steady state _t = ∞_, we end up with a single big drop of liquid.

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/MB.png" alt="drawing" width="1200"/>

Introducing the non-equilibrium Cahn-Hiliard equation...

<img src="http://www.sciweavers.org/tex2img.php?eq=%5Cfrac%7B%5Cpartial%5Cphi%7D%7B%5Cpartial%20t%7D%2B%5Cnabla%5Ccdot%5Cleft%28%20-%5Cnabla%5Cfrac%7B%5Cdelta%20F%7D%7B%5Cdelta%5Cphi%7D%20%2B%20%5Cboldsymbol%7B%5CLambda%7D%20%2B%20%5Clambda%5Cnabla%7C%5Cnabla%5Cphi%7C%5E2%20%2B%20%5Czeta%28%5Cnabla%5E2%5Cphi%29%5Cnabla%5Cphi%20%5Cright%29%3D0&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="\frac{\partial\phi}{\partial t}+\nabla\cdot\left( -\nabla\frac{\delta F}{\delta\phi} + \boldsymbol{\Lambda} + \lambda\nabla|\nabla\phi|^2 + \zeta(\nabla^2\phi)\nabla\phi \right)=0" width="394" height="47" />

If we start from the same intial configuration, we see similar phenomena where the fluid phase-separate into high density and low density. However in steady state, we get a perpetual boiling droplet, which is not possible in equilibrium because all the liquid will be evaporated.

<img src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/AMB+.png" alt="drawing" width="1200"/>

<video src="https://raw.githubusercontent.com/elsentjhung/elsentjhung.github.io/master/boiling-droplet.mov" type="video/mp4s"/>


