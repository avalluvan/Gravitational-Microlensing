---
tags: [Microlensing/Task 1]
title: Introduction to Gravitational Lensing
created: '2021-05-27T18:18:52.792Z'
modified: '2021-05-29T16:51:03.951Z'
---

# Introduction to Gravitational Lensing

> Massimo Meneghetti

> 27.5.21

Section 1.2

<!--
Go through the references and read the sections mentioned
Derive all the intermediate steps in the sections
Extract the answers of the questions mentioned
-->

<!--
Derive the general expression of deflection angle  (eq 1.36) and shapiro delay (eq. 1.42) using fermat's principle.
Deflection angle for a point mass lens (eq. 1.41)
-->
## Fermat's Principle and Light Deflection

 - Geodesic curves from the field equations of general relativity can be equivalently described by Fermat's Principle, as in geometrical optics
   - Light waves of a given frequency traverse the path between two points which take the least time
   - Snell's Law: $n_1 \sin\theta_I = n_2 \sin\theta_R$
 - Travel time $= \int\frac{n}{c}\text{ dl}$
   - Taking extremal path $\Rightarrow \delta \int_A^B n(\vec{x}(l))\text{ dl} = 0$ where, as usual $A$ and $B$ are fixed points
 - To find $n$:
   - Assume lens is weak $\Rightarrow \frac{\Phi}{c^2} \ll 1$ where $\Phi$ is the Newtonian gravitational potential. Valid in virtually all cases of astrophysical interest
   - and lens is small compared to distances between source, lens and observer
 - $\eta_{\mu\nu} = (+---)$
 - From spacetime interval $ds = 0$ $$\Rightarrow \left(1 + \frac{2\Phi}{c^2} \right)c^2dt^2 = \left(1 - \frac{2\Phi}{c^2}\right)d\vec x^2$$
 - Speed of light in gravitational field $c' = \frac{\vert d\vec x\vert}{dt} = c\left(1+\frac{2\Phi}{c}\right)$ $$c' = \frac{c}{n} \Rightarrow n \approx \left(1 - \frac{2\Phi}{c^2}\right)$$
 - $\rightarrow$ Travel time $\alpha\text{    } \int n(\vec x(l))\text{ dl}$
   - Light path $\Rightarrow \delta \int_A^B n(\vec{x}(l))\text{ dl} = 0$ variational problem can be solved using Euler equation
   - $\text{dl } = \left\vert\frac{d\vec x}{d\lambda}\right\vert d\lambda$
   where $\lambda$ is some curve parameter
   - $n(\vec x(l)) \left\vert\frac{d\vec x}{d\lambda}\right\vert \equiv \mathcal{L}(\dot{\vec x}, \vec x, \lambda)$ where L is the Lagragian

> 28.5.21

Derived the equations for deflection angle (central force problem), point mass lens and Shapiro delay
