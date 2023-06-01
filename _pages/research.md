---
permalink: /research/
title: "Research"
excerpt: "Eugene Klyshko - About my research"
author_profile: true
redirect_from: 
  - "/research.html"
---

**Studying protein dynamics using molecular dynamics sumulations.** 
<img src="/images/crystal.jpg" alt="idp" width="180px" align="left" style="padding:10px;"><img src="/images/ezgif-3-e1da36ca2200.gif" alt="md" width="180px" align="left" style="padding:10px;"> 
This approach is sometimes referred to as a “computational microscope”; equations of motion are numerically integrated for every atom based on an empirical potential energy function. Simulations produce long time-resolved trajectories of atomic coordinates and provide a representation of a given molecule’s structural ensemble. <img src="/images/idps.png" alt="idp" width="150px" align="right" style="padding:10px;"> 
In my work, I study a full spectrum of the dynamic disorder observed in proteins: from folded crystalline proteins to intrinsically disordered proteins (IDPs) in solution. Compared to folded proteins, IDPs lack a stable three-dimensional structure, and instead they dynamically interchange between a large ensemble of conformational states corresponding to shallow minima of the free energy landscape. 

---

**Defining conformational states of proteins using dimensionality reduction and clustering algorithms.**
<img src="/images/clusters.png" alt="clusters" width="200px" align="left" style="padding:10px;"> 
 I am trying to build an intuition about the clustering of molecular conformations in order to apply it to protein simulations.  <img src="/images/MDS.png" alt="mds" width="200px" align="right" style="padding:10px;">  Clustering methods used to analyze MD trajectories require specification of the number of clusters. The number of clusters is an approximation to number of conformational states since geometrically and energetically similar structures share the same conformational states. This parameter is often unknown in advance and is the quantity of interest itself. 

---

**Developing Markov State Models to describe the conformational space and dynamics of proteins**
I am seeking for a methodological approach to build robust, accurate and easy to interpret [Markov state models](https://pubs.acs.org/doi/10.1021/jacs.7b12191) for the dynamics of protein.  <img src="/images/MSM.png" alt="MSMs" width="250px" align="left" style="padding:10px;"> The steps will include proper featurization of conformational states, extraction of the most significant features through dimensionality reduction, clustering  of  the  conformations  into  distinct  kinetically  relevant  states,  building  an  MSM  transition  matrix,  and estimating the accuracy of the MSM based on objective quality metrics.
