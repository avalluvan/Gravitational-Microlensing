---
tags: [Microlensing, Microlensing/Task 2]
title: Astrometric Microlensing
created: '2021-06-09T16:41:36.027Z'
modified: '2021-06-21T10:51:51.624Z'
---

# Astrometric Microlensing

> A. Nucita

Section 2: Basics of astrometric microlensing

## Abstract

 - Astrometric microlensing could be a channel to investigate the nature of both lenses and sources
 - It corresponds to the shift of the position of the (multiple) image (centroids) with respect to the source star location
   - Microlensing = micro to milliarcseconds and it depends on the charateristic of the lens-source system
 - Classes of events: single/binary lens acting on single/binary source
   - Additional effects: finite source size, blending (?), orbital motion of lens/source

## Introduction

 - Detect compact objects in disk, bulge and halo of galaxies
 - High quality observations is sensitive to low mass objects and can be used to characterise binary lens systems
 - Gravitational microlensing induces an astrometric shift between the "light centroid of the multiple images and the source star position" <strike>(?)</strike> (detailed later in the paper)

#### Point-like lens

 - Simplest case
 - Point-like object lensing a single source
 - Source image splits into two images
   - Shift in position of light centroid <strike>(?)</strike> describes an ellipse
     - i.e., over a period of time (characterised in units of $t_E$)
   - Semi-axes depend on the impact parameter of the lens $u_0$ and Einstein $t_E$ <strike>(?)</strike>
     - Einstein ring crossing time, $t_E = \frac{\theta_E}{\mu}$ where $\mu = v_\perp$ is the angular velocity of the star wrt the lens
####
 - In binary lens systems, the shape of the light centroid is more dependent on the binary system parameters - mass ratio and separation
 - Aim of the paper: discuss main observational features of astrometric microlensing and introduce second order effects detectable by high quality telescopes

## Basics of Astrometric Microlensing

 - Mathematical expressions given in units of $t_E$, $\theta_E$ and $R_E$ (scales in astrometric phenomena)
 - Multiple images are formed during gravitational lensing
   - $\mu_+ \rightarrow$ magnification of brighter image
   - $\mu_- \rightarrow$ magnification of fainter image
   - Source moves in the lens plane with transverse velocity $v_\perp$ $$\theta_E = \sqrt{\frac{4GM}{c^2}\frac{(D_S - D_L)}{D_LD_S}}$$ where $M$ is the mass of the lens, $D_S$ and $D_L$ are the distances from the observer to the source and lens respectively $$\Rightarrow \text{ Einstein Radius }R_E = D_L\theta_E$$
   - Projected coordinates parametrised as $$\xi(t) = \frac{(t-t_0)}{t_E} \text{ and } \eta(t) = u_0$$
 - Centroid of image pair $(+ \text{ and } -)$ $$\overline{u} \equiv \frac{\tilde{u}_+\mu_+ + \tilde{u}_-\mu_-}{\mu_+ + \mu_-} = \frac{u(u^2 + 3)}{u^2 + 2}$$
 - Astrophysical observable: Displacement vector of the combined image, i.e., the centroid shift traces wrt the source (?)$$\Delta = \overline\mathbf u - \mathbf u = \frac{\mathbf u}{u^2 + 2}$$
   $$\Rightarrow \Delta_\xi = \frac{\xi(t)}{u^2 + 2} \text{ and } \Delta_\eta = \frac{u_0}{u^2 + 2}$$ $\Delta_\eta :$ symmetric, positive-definite; $\Delta_\xi:$ antisymmetric with extrema at $t = t_0\pm t_E\sqrt{u_0^2 + 2}$
 - $\Delta$ traces an ellipse in the $\Delta_\xi-\Delta_\eta$ plane centred at $(0,b)$ with semi-major axis $a$ along $\Delta_\eta$ and semi-minor axis $b$ along $\Delta_\xi$ $$a = \frac{1}{2}\frac{1}{\sqrt{u_0^2 + 2}} \text{ and } b = \frac{1}{2}\frac{u_0}{u_0^2 + 2}$$ $$\Rightarrow u_0^2 = \frac{2\left(\frac{b}{a}\right)^2}{1-\left(\frac{b}{a}\right)^2}$$
 - Difference between astrometric microlensing and photometric microlensing <strike>(?)</strike>
   - Astrometric: Position of star
   - Photometric: Light flux of star

### Blending Effect

 - Intrinsic luminosity of the lens (or nearby stars) is taken into account
 - Blending refers to the fraction of light that does not get amplified (magnified) but contributes to the photons collected during observation
   - The lens could not be resolved on direct observations
 - Ratio between lens and source luminosities $f_L = \frac{L_L}{L_S}$
 - New definition for centroid position, $$\overline u = \frac{\tilde{u}_+\mu_+ + \tilde{u}_-\mu_- + \tilde u_L f_L}{\mu_+ + \mu_- + f_L}$$ where $\tilde u_L$ is the position of the lens
 - Centroid shift with respect to the source at rest is, $$\Delta_S = \overline u - u = \frac{u - f_Lu^2\sqrt{u^2 + 4}}{u^2 + 2 + f_Lu\sqrt{u^2 + 4}}$$ The frame of reference is centred on the lens $\tilde u_L = 0$
   - Where is the $(u^2 + 3)$ factor (?)
 - "However, it is necessary to further subtract the proper motion of the apparent source object which corresponds to the superposition of the source and the luminous lens. In this case, the resulting (blended) centroid shift is" (?) $$\Delta = \Delta_S + \frac{f_L}{1+f_L}u$$
 - Blended shift components along $\xi$ and $\eta$ axes $$\Delta_\xi = \Delta \cos \alpha \ \ \ \ \Delta_\eta \sin \alpha$$ where $\alpha = \arctan\left( \frac{u_0t_E}{t-t_0} \right)$

### Finite Size Source and Single Lens

 - Consider a source star of radius $\rho$ with no blending effects, then $$|\Delta| = \frac{\int_{A_{Source}} (\tilde{u}_+\mu_+ + \tilde{u}_-\mu_-)\ S\ dA}{\int_{A_{Source{}}}(\mu_+ + \mu_-)\ S\ dA} - u$$ where $A_{Source}$ is the area subtended by the source and $S$ is a weighting factor that accounts for surface luminosity function of the star
   - These surface integrals are solved numerically
   - $S=1$ for a uniformly bright circular source of radius $\rho \ll u_0$
     - $$\Delta \simeq \frac{u(u^2 + 3)}{u^2 + 2}\left(1+ \frac{\rho^2(u^6 + 9u^4 - 6u^2 - 24)}{8u^2(u^2 + 2)(u^2 + 3)(u^2 + 4)} \right)$$
 - What is $\Gamma$ (?)
