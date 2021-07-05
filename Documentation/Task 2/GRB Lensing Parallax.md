---
tags: [Microlensing/Task 2]
title: GRB Lensing Parallax
created: '2021-06-09T16:45:00.941Z'
modified: '2021-06-22T09:58:57.994Z'
---

# GRB Lensing Parallax

> Sunghoon Jung

Needs to be presented to Professor

[Interesting read](https://en.wikipedia.org/wiki/Primordial_black_hole)

## Abstract

 - PBH comprising full dark matter abundance is currently allowed if its mass lies between $10^{-16} M_\odot \leq M \leq 10^{-11} M_\odot$
 - Lightest mass range is hard to be probed by ongoing gravitational lensing observations
 - Lensing parallax of GRBs $\Rightarrow$ observed simultaneously by spatially separated detectors
   - Can probe 'the unconstrained mass range' (?)
 - Achievable detector separation = $r_\oplus - AU$
   - Large enough to resolve GRB lensing by lightest PBH DM

## Introduction

 - PBH is a DM candidate
   - Possibly formed from overdensities in primordial density fluctuations during inflation
   - Too large: Could have disturbed CMB
   - Too small: Evaporated through Hawking Radiation
   - Mass range within constraints: $10^{-16} M_\odot \leq M \leq 10^{-11} M_\odot$
 - Probing PBH DM:
   - Induced dynamics - effects on observed systems
   - Gravitational lensing - paper expects it to be more robust
     - Microlensing possible for $10^{-11} M_\odot \leq M \leq 10 M_\odot$
     - Strong lensing for higher masses
     - $10^{-16} M_\odot \leq M \leq 10^{-11} M_\odot$ too weak to be resolved - requires wave optics effects to be accounted

## Lensing Parallax

 - **Parallax:** The apparent displacement of an object because of a change in the observer's point of view
   - Lensing parallax is the parallax caused due to the effect of gravitational lensing
     - It allows the detection of lensing by correlating the brightnesses (or fluxes) of a source simultaneously measured by spatially separated detectors
 1. If spatial separation of detectors, $\Delta r \gtrsim R_E = \theta_E D_L$ of a PBH lens (where $\theta_E = \sqrt{\frac{4GM}{c^2}\frac{D_{LS}}{D_LD_S}}$) then the two detectors will observe different lensing magnifications
 - Observed magnification of unresolved images, $$A = \mu_+ + \mu_- + \sqrt{\mu_+ \mu_-}\cos \left(\frac{2\pi c\Delta t_d}{\lambda}\right)$$ where $\Delta t_d$ is the time delay, $u=\frac{\beta}{\theta_E}$, and magnification of brighter and dimmer images are, $$\mu_\pm = |\frac{1}{2} \pm \frac{u^2 + 2}{2u\sqrt{u^2 + 4}}|$$
   - Last $\cos$ term accounts for interference fringes and it averages quickly (unless $\lambda \sim \mathcal{O}(\frac{GM}{c^2}) \equiv \frac{c\Delta t_d}{\lambda} \sim \mathcal{O}(1)$) $\Rightarrow A \simeq \mu_+ + \mu_-$, independent of frequency for majority of the parameter space
   - Nevertheless, GRBs are very high frequency waves

| Lensing Parallax                                        | Microlensing                               |
|---------------------------------------------------------|--------------------------------------------|
| Detectable with short-transients                        | Requires long transients                   |
| Simultaneous observations from well-separated detectors | Single observer over (a necessary) temporal variation |

 - Both lensing parallax and microlensing measure brightness at multiple relative angles to detect lensing
 2. Apparent source angular size, $\mathbf{\theta_S} = \frac{r_S}{D'} \lesssim \mathbf{\theta_E}$ (where $r_S$ is the physical transverse emission size and $D'\sim D_S\sim D_L$) to induce sizable lensing, otherwise only a small part of the source will be magnified
     - $$\Rightarrow \delta A \equiv \frac{|A_1 - A_2|}{(A_1 + A_2)} \gtrsim \frac{\epsilon}{2}$$ where $\epsilon$ is the fractional brightness resolution and $A_i$'s are the magnifications at the two detectors
     - $\delta \equiv \frac{\theta_S}{\theta_E} \lesssim 1$ (?) possible inconsistency
 3. Probe wavelength $\lambda \lesssim R_{Sch}$ of the PBH lens, otherwise the wave cannot see the lens
     - $$\Rightarrow 0.1\lambda \lesssim \frac{2GM}{c^2}(1+z_L)$$ where $z_L$ is the lens redshift and recall that $\lambda = \frac{c}{f}$
 - From 1. $$M_{max} \lesssim \left(\frac{\Delta r}{AU}\right)^2 \left(\frac{Gpc}{D}\right)10^{-7}M_\odot$$
 - From 2. $$M_{min} \gtrsim \epsilon \left(\frac{r_S}{r_\odot}\right)^2 \left(\frac{Gpc}{D}\right) 10^{-12}M_\odot$$
 - From 3. for GRBs with $f = 10^{19} - 10^{21}$ and negligible $z_L$ $$M_{min} \gtrsim (10^{-15} - 10^{-17})M_\odot$$
 -  2. is more dominant over 3. for GRBs

## GRB Parameters

### Source Parameters

 - Parameters:
   - Minimum variability time scale $t_{var} \sim \frac{r_S}{c}$
   - Source redshift $z_S$
   - Lorentz factor $\Gamma$
   - Observed burst duration $T_{90} \sim \frac{\Gamma}{c}$
   - Number of GRB detections $N_{GRB}$
 - Probing range:
   - $r_S \lesssim r_\odot$ (10% abundance in GRB progenitors) probe lightest unconstrained (?) PBH mass range
   - High frequency GRB spectrum (of photon counts. They vary among GRBs) probe lightest PBHs
     - Workaround by using $\epsilon = 0.1$ (conservative scenario) or $\epsilon = 0.01$ (optimistic scenario)
     - Works when different frequencies show the same magnification (with appropriately different fluxes)
   - Conservative: Fermi (Gamma-Ray Space Telescope) observes $E \sim 0.5MeV \Rightarrow f \approx 10^{20}Hz$ (highest frequency with reasonable photon detection) ($N_{GRB} = 10^3$)
   - Optimistic: $f \approx 10^{21}Hz$ ($N_{GRB} = 10^4$)
   - Cosmological distance of GRBs $z_S = 0.5 - 3$

### Wave-Optics Effects

### Upper Bound on PBH Abundance

## GRB Results

 - Optical depth $\tau$ is the expected number of PBHs withing volume of desired PBH locations that can lead to appreciable lensing parallax $$\tau \approx \frac{2\pi}{3}\frac{G\rho}{c^2}D_S^2$$ for $\rho = Mn$
   - $n \approx \rho_{crit,0}\Omega_{DM}\frac{f}{M}$ where $f=\frac{\Omega_{PBH}}{\Omega_{DM}}$ is the PBH abundance (?)
 - Unconstrained PBH DM mass range, $$\Rightarrow 10^{-16}M_\odot \lesssim M \lesssim 10^{-11}M_\odot$$
 - Largest astrophysical separation that can be created $\Delta r = 2AU$ over half revolution of Earth around Sun
   - Largest simultaneous separation $\Delta r = 2r_\oplus$
 - Better resolution can be achieved $\epsilon < 0.1$ with
   - Higher proton counting rates from larger detector area
   - Higher sampling frequency
   - Better detection efficiency

### Nearby Stars Results

 - GAIA is an example of a telescope at L2 point
   - Current optical telescopes can be used for probing
 - Stars are more sensitive to heavier PBHs (if at all they exist) and are closer to Earth (frequency emitted is lower $\Rightarrow$ energy is weaker and amplitude is lost at longer ranges)
   - Apparent radii of stars are also larger (even $>R_E$)
   - Conservative range: $10^{-9}M_\odot \lesssim M \lesssim 10^{-2}M_\odot$
   - Optimistic range: $10^{-12}M_\odot \lesssim M \lesssim 10^{3}M_\odot$

## Discussions
 
 - GRB lensing parallax opens a new range of PBH DM to be probed
 - Longer distance + more compact source make it small compared to $\theta_E \propto M_{PBH}$ of the lightest PBH
 - Lesser scattering dispersion (a limiting factor for longer wavelengths) (?) isn't rayleigh scattering inversely proportional to 4th power of wavelength
   - I am not fully clear on this, but I believe the dispersion referred to here is the intergalactic scattering dispersion of FRBs
 - Higher frequency relaxes interferometric and fringe effects on intensity, averaging it out instead
 - Combined with optical and GRB, full range of PBH DM can be probed by lensing
 - I think brightness resolution refers to radiometric resolution
