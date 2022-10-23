---
layout: page
title:
---

This site accompanies the paper [Efficiently Learning the Inverse Kinematics With Obstacles](https://ieeexplore.ieee.org/) by
[Johannes Tenhumberg](https://scholar.google.com/citations?user=2RZuYZMAAAAJ), [Arman Milke]((https://scholar.google.com), [Darius Burschaka](https://scholar.google.com/citations?user=y-MzVoUAAAA ) and [Berthold Bäuml](https://scholar.google.com/citations?user=fjvpDsEAAAAJ).


![Agile Justin in front of a shelf](/assets/imgs/justin_shelf2.png){:.this
style="width: 600px;
display: block;
margin-left: auto;
margin-right: auto"}

# Abstract
---
A fast and efficient inverse kinematics (IK) solu- tion is central to robotic planning.
Traditionally those methods are based on root-search and optimization algorithms.
This approach can be sped up by using neural networks to provide a valuable initial guess, which can then be quickly refined numerically.
While learning-based approaches to the IK exist, none account for obstacle-collision in diverse environments.
We introduce an unsupervised training method that removes the need for the initial data generation and eliminates the problem of a single label for an ambiguous problem.
Using the network’s prediction as an initial guess for a two-stage jacobian-based solver allows for fast and accurate computation of the collision-free IK.
Besides a detailed analysis of the problem and the network structure, we compare our method on complex 3D environments for the humanoid robot Agile Justin to a random multi-start and supervised training.
Our method significantly outperforms the random multi-start and requires much less training time than the supervised method while achieving comparable results.