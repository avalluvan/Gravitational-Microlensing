---
tags: [Microlensing/Task 2]
title: Introduction to Gravitational Lensing 2
created: '2021-06-09T16:42:53.090Z'
modified: '2021-07-05T07:01:31.122Z'
---

# Introduction to Gravitational Lensing 2

> Massimo Meneghetti

Section 2.2: Derive the lens equation (eq. 2.9)
Section 2.3: Lensing potential
Section 2.4: Magnification and distortion
Section 3.1: Images and their magnifications due to point lens
Section 4.1: Basics of Microlensing
Section 4.2: Searching MACHO using microlensing

##

### General Lens

 $$\hat \alpha \propto M$$ $$\Rightarrow \text{ the deflection angles of array of lenses can be linearly superposed}$$
 - For a sparse distribution of $n$ point masses on a plane whose positions and masses are $\vec\xi_i$ and $M_i$ $\forall$ $i=1\dots n$, then the deflection angle of a light ray crossing the plane at $\vec \xi$ will be $$\hat \alpha (\vec \xi) = \sum_i \hat \alpha_i (\vec \xi - \vec \xi_i) = \frac{4G}{c^2}\sum_i M_i \frac{(\vec \xi - \vec \xi_i)}{\vert\vec \xi - \vec \xi_i\vert^2}$$
 - Thin lens approximation $\Rightarrow$ planar distribution of matter in the lens plane (aka thin screen approximation. Can also be applied to source / source plane) $$\text{Surface density, }\Sigma (\vec \xi) = \int \rho(\vec \xi, z)dz$$ where $\vec \xi$ is a 2D vector on the lens plane and $\rho$ is the 3D density $$\Rightarrow \frac{4G}{c^2}\int d^2\xi' \frac{(\vec \xi - \vec \xi')\Sigma(\vec \xi')}{\vert\vec \xi - \vec \xi'\vert^2}$$
   - For an axially symmetric lens, $$\hat \alpha = \frac{4GM(\xi)}{c^2 \xi}$$ where the deflection is determined by the mass enclosed $M(\xi)$ by the circle of radius $\xi$
   By symmetry of mass distribution, $\hat \alpha \parallel \vec \xi$ and $\vec \eta \parallel \vec \xi$

### Lens Equation

 - "It is not guaranteed that the relation between physical size, distance and angular size can be written as $\text{[physical size] = [angular size] } \cdot \text{ [distance]}$ if space is curved. It is however possible to define distances in curved spacetime such that this relation from Euclidean space holds. Then, however, distances are not additive, such that $D_L + D_{LS} = D_S$"
 - Typical gravitational lensing system:
   - Observer and Optical axis
   - Lens plane ($\perp$ optical axis): Collection of lensing objects approximated as a point-source or and extended line source
   - Source plane ($\perp$ optical axis): Source star
 - Parameters:
   - Distances:
     - $D_L$ = observer to lens
     - $D_S$ = observer to source
     - $D_{LS}$ = lens to source
   - Angular distances:
     - $\beta$ = angular position of source
     - $\hat \alpha$ = deflection angle
     - $\theta$ = due to deflection, angular position at which observer appears to receive light from the source
   - Derived parameters:
     - $\vec \alpha = \vec \theta - \vec \beta$ = reduced deflection angle
     - $\vec y\eta_0 = \vec \eta = \vec \beta D_S$ = position of star on source plane from intersection with optical axis 
     - $\vec x\xi_0 = \vec \xi = \vec \theta D_L$ = impact parameter ($b = |\vec \xi|$)
     - $D \equiv \frac{D_L D_S}{D_{LS}}$ = effective lensing distance
     - $\theta_E = \sqrt{\frac{4GM}{c^2D}}$ = Einstein angle
     - $u = \frac{\beta}{\theta_E}$ = position of the source
     - $x = \frac{\theta}{\theta_E}$ = position of the lens
 - If angles are small, true position of the source and its observed position on the sky are related by the **lens equation** (obtained by a geometric construction) $$\theta D_S = \beta D_S + \hat \alpha D_{LS}$$ $$\Rightarrow (\theta - \beta) = \alpha(\theta) = \frac{D_{LS}}{D_S} \hat \alpha(\theta)$$
 - Dimensionless vectors, $$\vec x = \frac{\vec \xi}{\xi_0} \ \ \ \ \vec y = \frac{\vec \eta}{\eta_0}$$ where $\xi_0$ is a length scale on the lens plane and $\eta_0 = \xi_0\frac{D_S}{D_L}$ on the source plane
 Dimensionless reduced deflection angle, $$\alpha(\vec x) = \frac{D_L}{\xi_0} \left(\frac{D_{LS}}{D_S}\hat \alpha(\xi_0 \vec x)\right)$$ where $\alpha(\vec x) = \vec x - \vec y$

### Lensing Potential

 - For extended distribution of lensing matter
 - Characterised by effective lensing potential, $$\hat \Psi(\vec \theta) = \frac{D_{LS}}{D_LD_S} \frac{2}{c^2} \int \Phi (\vec \xi, z) dz$$ obtained by projecting the 3D Newtonian gravitational potential $\Phi$ on the lens plane (and properly rescaling it)
   - Dimensionless form, $$\Psi = \frac{D_L^2}{\xi_0^2}\hat \Psi$$
 - Properties of lensing potential,
   1. $$\vec \nabla_x \Psi(\vec x) = \vec \alpha (\vec x)$$
   2. $$\Delta_x \Psi(\vec x) = 2\kappa (\vec x)$$ where $\kappa(\vec x) = \frac{\Sigma (\vec x)}{\Sigma_{cr}}$ is the convergence factor of a lens (defined as a dimensionless surface density) with surface mass density $\Sigma (\vec \theta) = \frac{1}{4\pi G}\int_{-\infty}^{+\infty} \Delta \Phi dz$ and the critical surface density, $\Sigma_{cr} = \frac{c^2}{4\pi G}\frac{D_S}{D_L D_{LS}}$, a characteristic quantity of the lens system
   This equation is derived from the Poisson equation, $\Delta \Phi = 4\pi G\rho$
 - In dimensionless quantities, $$\Rightarrow \kappa(\vec x) = \frac{1}{2}\Delta_x \Psi(\vec x)$$ $$\Rightarrow \Psi (\vec x) = \frac{1}{\pi}\int_\mathbb{R^2}\kappa(\vec x')\ln |\vec x' - \vec x | d^2x'$$ $$\Rightarrow \alpha(\vec x) = \frac{1}{\pi} \int_\mathbb{R^2} d^2x'\kappa(\vec x')\frac{\vec x - \vec x'}{|\vec x - \vec x'|}$$

### Magnification and Distortion

 - The distortion of images is described by the **Jacobian matrix**, $$A \equiv \frac{\partial\vec y}{\partial\vec x} = \left( \delta_{ij} - \frac{\partial \alpha_i(\vec x)}{\partial x_j} \right) = \left( \delta_{ij} - \frac{\partial^2 \Psi(\vec x)}{\partial x_i\partial x_j} \right) \equiv \left( \delta_{ij} - \Psi_{ij} \right)$$ where $$\Psi_{ij} = \begin{bmatrix}\Psi_{11} & \Psi_{12}\\\Psi_{21} & \Psi_{22}\end{bmatrix}$$
   - It is a symmetric matrix and can be broken down into diagonal (isotropic) + traceless (anisotropic)
   - Traceless matrix contributes to a pseudo-vector (shear) $\vec \gamma = (\gamma_1,\gamma_2)$ on the lens plane who components are $$\gamma_1(\vec x) = \frac{1}{2}(\Psi_{11} - \Psi_{22})\ \ \ \ \gamma_2(\vec x) = \Psi_{12} = \Psi_{21}$$
     - Eigenvalues = $\pm \sqrt{\gamma_1^2 + \gamma_2^2} = \pm \gamma$
  Thus, there exists a coordinate rotation by $\phi$ such that, $$\Gamma = \begin{bmatrix}\gamma_1 & \gamma_2\\\gamma_2 & -\gamma_1\end{bmatrix} = \gamma\begin{bmatrix}\cos 2\phi & \sin 2\phi\\\sin 2\phi & -\cos 2\phi\end{bmatrix}$$
  $$\Rightarrow A = \begin{bmatrix}1-\kappa-\gamma_1 & -\gamma_2\\-\gamma_2 & 1-\kappa + \gamma_1\end{bmatrix} = (1-\kappa)\mathbb{I}_2 - \Gamma$$
 - When $\gamma \neq 0$, the semi major and semi minor axes are, $$a = \frac{r}{1 - \kappa - \gamma}\ \ \ \ b = \frac{r}{1 - \kappa + \gamma}$$ where $r$ is the radius of the circular source
 - "Through the lens equation, the solid angle element $\delta\beta^2$ (or equivalently the surface element $\delta y^2$) is mapped into the solid angle $\delta\theta^2$ (or in the surface element $\delta x^2$)." (?)
 - Liouville Theorem (?)
 - Magnification, $$\mu = \det M = \frac{1}{\det A} = \frac{1}{(1-\kappa)^2 - \gamma^2}$$ where $M = A^{-1}$ is called the magnification tensor
   - How is the $\gamma$ term incorporated in this formulation. What is an intuitive reason to account for shear effects in an expression for magnification (?)
   - Total magnification $\mu = |\mu_+| + |\mu_-|$ (?)
 - The eigenvalues of $M$ measure the amplification in the tangential and radial directions $$\mu_t = \frac{1}{\lambda_t} = \frac{1}{1 - \kappa - \gamma} \ \ \ \ \mu_r = \frac{1}{\lambda_r} = \frac{1}{1 - \kappa + \gamma}$$
 - Lens critical lines (in the lens plane):
   - $\lambda_t = 0 \Rightarrow$ curve called tangential critical line along which an image is strongly distorted tangentially to this line
   - $\lambda_r = 0 \Rightarrow$ curve called radial critical line along which an image is stretched in the direction perpendicular to the line itself
 - The sources generating images around the critical lines are located along the caustics

## Lens Models

 - One of the main goals of lensing theory: Determine which combinations of lenses and sources can reproduce a particular image configuration
   - Simple analytic lens models
     - Point models, axially symmetric models
   - Numerical simulation models
     - Elliptical models

### Point Masses

 - Deflection angle of a point mass as lens, $$\hat \alpha = \frac{4GM}{c^2b}$$
 - Lensing potential of a point mass as lens, $$\hat \Psi = \frac{4GM}{c^2}\frac{D_{LS}}{D_LD_S}\ln |\vec\theta|$$
 - Let Einstein angle be defined as, $$\theta_E = \sqrt{\frac{4GM}{c^2}\frac{D_{LS}}{D_LD_S}}$$ $$\Rightarrow \beta = \theta - \alpha = \theta - \frac{\theta_E^2}{\theta}$$Quadratic in $\theta$ $$\Rightarrow \theta_\pm = \frac{1}{2}(\beta \pm \sqrt{\beta^2 + 4\theta_E^2})$$
 - Two images for any source (irrespective of $\beta$)
   - "Why not three? Because its mass is singular and thus the time-delay surface is not continously deformed" (?)
 - $$\mu_\pm = \frac{1}{1 - \left( \frac{1}{x_\pm} \right)^4}$$

####
 - Magnitude of star $\Rightarrow \Delta m = 2.5\log \mu$ <strike>(?)</strike>
   - Formula for star's apparent magnitude

## Microlensing

 - For lenses whose sizes are small compared to the scale of the lensing system
   - Small masses, distant lenses and sources
   - Typical mass range: $10^{-6} \leq M/M_\odot \leq 10^6$
   - Corresponding $\theta_E$ are smaller than a milli-arcsecond

### Lensing of Single Stars by Single Stars

 - Single foreground star (as lens), single background star (as source) within the Local Group
   - Distances of the order of kiloparsecs
   - Negligible curvature in spacetime $\Rightarrow D_S = D_L + D_{LS}$
   - Stars mass distribution assumed to spherically symmetric
     - Light absorbed if $b\leq R_\star$
     - Light deflected if $b > R_\star$
   - Stellar sources subtend considerably smaller angles than $R_E$ in microlensing systems
   - $u = \frac{\beta}{\theta_E}$ position of the source, and $x = \frac{\theta}{\theta_E}$ position of the lens
     - Image positions: $x_\pm = \frac{1}{2}\left( u \pm \sqrt{u^2 + 4}\right)$
     - Total magnification: $\mu = |\mu_+| + |\mu_-| = \frac{u^2 + 2}{u\sqrt{u^2 + 4}}$, a function of source position
   - Relative motion of the source wrt lens introduces **variability** in the light curve of the source $$\Rightarrow L(u(t)) = \mu(u(t)) \hat L$$ where $\hat L$ is the **source intrinsic luminosity**
   - The characteristic time scale of the change of $L$ is given by the (Einstein crossing) time needed by the source to cross the Einstein ring $$t_E = \frac{D_L \theta_E}{v_\perp}$$ where $v_\perp$ is the transverse velocity (perpendicular to the LoS, i.e., within the source plane)

####
 - Assume the motion of the source is linear. Express trajectory as $$u(t) = \sqrt{u_0^2 + \left(\frac{t-t_0}{t_E}\right)^2}$$ where $u_0$ is the minimal distance between the lens and source and $t_0$ is the time of closest approach ($u(t_0) = u_0$)
   - What is $u_0$ <strike>(?)</strike>
     - Closest point of approach of source when projected on lens plane
   - Can plot magnification vs source position (wrt time) for different impact parameters
 - Parameters of light curves:
   - Unlensed Luminosity (aka flux) = $\hat L$, measured when the source is at a large angular distance from the lens
   - Time of closest approach = $t_0$, maximum peak of the light curve
   - Distance of closest approach = $u_0$, from knowledge of the position of the lens
     - Is this the same as impact parameter in gravitational lensing <strike>(?)</strike>
       - No. Impact parameter is a general term for distance at point of closest approach
   - Einstein crossing time = $t_E$, physical information about the lensing system
 - Further assume that the source light dominates the lens light dramaticallly $\rightarrow$ blending effects are negligible

### Searching for Dark Matter with Microlensing

#### General Concepts

 - Massive Astrophysical Compact Halo Objects is a possible candidate for dark matter
 - While observing distant source stars, microlenses (in the foreground) would produce time-variable magnification
   - More abundant and massive the microlenses, more frequent and longer the microlensing events
 - Let solid angle of the observation (FoV) be $\delta \Omega$ and microlens density as a function of distance be $n(D_L)$, then the optical depth is (?) $$\tau = \frac{1}{\delta\Omega}\int_V dV\ n(D_L)\ \pi\theta_E^2$$ where $\theta_E^2$ is the cross section of the microlensing event. $dV = \delta \Omega\ D_L^2\ d(D_L)$ $$\Rightarrow \tau = \frac{4\pi G}{c^2} \int_0^{D_S} d(D_L)\ \frac{D_L D_{LS}}{D_S}\ \rho(D_L)$$ where $\rho = Mn$ $$\Rightarrow \frac{D_L D_{LS}}{D_S} = \frac{D_L (D_S - D_L)}{D_S} = D_L - \frac{D_L^2}{D_S}$$
   - "Optical depth is dimensionless, and in particular is not a length, though it is a monotonically increasing function of optical path length, and approaches zero as the path length approaches zero" [Source](https://en.wikipedia.org/wiki/Optical_depth)
 - If mass density is (assumed to be) a constant $\rho$ along the LoS (to the sources) $$\tau \approx \frac{2\pi}{3} \frac{G\rho}{c^2}D_S^2$$
 - For a galaxy whose stars revolve with velocity $v$, $\rho \approx \frac{1}{\frac{4\pi G}{3}}\left(\frac{v}{r}\right)^2 \Rightarrow \tau \approx \frac{1}{2} \left(\frac{v}{c}\right)^2$

### Observational Results in Searches for Dark Matter

 - Principle results:
   - 8% to 50% of the Milky Way's halo could be composed of MACHOs
   - Halo mass fraction in MACHOs is < 20% for masses between $10^{-7}M_\odot$ and $0.1M_\odot$
   - MACHOs have been detected between Earth and the Magellanic Clouds, but insufficient to explain all of the Milky Way's dark matter mass. 
   - Unlikely that all LMC lensing events are due to self-lensing by stars
   - Only a fraction of extended dark matter halos are composed of compact objects of stellar and sub-stellar mass
