---
tags:
  - radiation
  - light
  - observation
  - physics
  - quantum_physics
  - astronomy
  - mathematics
---
We observe the universe using [[Telescopes]], and we gather information using [[Light]], which is actually **electromagnetic radiation**, described by [[Maxwell's Electromagnetic Wave Theory]]. This light spans the entire [[Electromagnetic spectrum (EM)]], where different types of telescopes observe different phenomena. We observe the light from objects as [[Photometric quantities]] on Earth. 

##### But, where does that light come from?

# Radiation of [[Atoms]] and [[Molecules]]
---
From quantum physics, we know that energy comes in little packets we call **quanta.** These packets travel around in the forms of both **particles and waves.** ([[Wave-particle duality]]) [[Light]] is composed of these small quanta called **photons**, and they are a form of **electromagnetic radiation**, which is a wave quantity. 

These photons have a certain energy associated with them:
- f $$\Delta E = h\nu$$, where $h$ is the plank constant, and $\nu$ is the frequency. 

[[Atoms]] can release an electron, its energy decreases by that amount and if it gains an electron it increases by that amount. 

Other than being a mass of [[Protons]] and [[Neutrons]] in a [[Nucleus]], surrounded by an [[Electron]] cloud, these electrons are in certain [[Orbitals]] and [[Electron shell]]s, which have ***quantized energy***:$$|E_i − E_f| = hν_{if}$$
Because of this, only ***specific photons with a specific energy*** can excite an atom into releasing energy. This gives rise to the science of [[Spectroscopy]]!

Other than energy, due to Broglie's law, each photon carries a [[Momentum]] of:
- f $$p = \frac{h}{\lambda} = \frac{E}{c}$$

The **radiation pressure** is the pressure that radiation applies when it shines upon an object, otherwise:
- f $$P = \frac{F}{c}$$

## Spectroscopy
---
William Hyde Wollaston and Josef von Fraunhofer were looking at [[The Sun]] one day and discovered that it had dark lines in its spectra called **Fraunhofer spectrum**. They didn't know why they occurred, but there was another scientist on the path to discovery. Kirchoff noticed that gasses could absorb or emit light at certain wavelengths, meaning that certain gases had different perfect wavelengths of emission or absorption. But, why?

- eg  **Spectrum** is a graphical representation of the amount of each color of light present in the object's radiation. The horizontal (x) axis is the color (or other proportionally related properties like wavelength, or energy) an the vertical (y) axis denotes the amount of light (or in other words brightness, intensity,  or flux([[Photometric quantities]])) 

![[simple spectra.png|400]]
**Continuous spectra** is when the spectrum of a body isn't interfered with by gases or other phenomena.

As will be discussed below, continuous spectra can form from *free-free transitions* of electrons.

> When the pressure of hot gas is increased, the spectral lines begin to broaden. At high pressure, atoms bump into each other more frequently, and the close neighbors disturb the energy levels. When the pressure is high enough, the lines begin to overlap. Thus the spectrum of hot gas at high pressure is continuous.

---

The fact that specific photons can excite electrons in an atom give rise to the **line spectrum**. <mark style="background: #BBE6E4;">Hot gas under low pressure</mark> has **emission lines**, or *emission spectra*, while <mark style="background: #BBE6E4;">that same gas when cooled</mark> has **dark absorption lines**, or absorption spectra. 

![[spectral lines complete.png]]

---

Atoms in gas are found in their natural energy, state, also called ***the ground state***. When we add energy into that system, the atom becomes **excited**, which usually lasts for a fraction of a second before the atom returns back to normal by releasing a photon. In this system a bound electron has *negative energy*, while an unbound one *positive energy* (exactly as in [[Planetary orbits]] from [[Conic sections]]). When an atom is ionized or it loses an electron, its called a **free-bound process**, but when an electron is accepted it's called **recombination**. A third type of interaction is when an electron gets knocked off from a nucleus or ion and isn't captured, called a **free-free radiation** or *thermal bremsstrahlung*. 

This is summarized by the following image:
![[energy processes spectra.png|400x260]]

---
# Composition of stars
Now, using absorption spectra, we can calculate the quantity of stuff in a star's composition, and its shown below in a logarithmic graph of the amount of atoms. We can see that of course, hydrogen and helium are at the top, with other elements getting lower and lower the higher atomic number it has.
![[elements of stars.png|400]]

> The corresponding mass fractions are $X ≈ 0.72$ and $Y ≈ 0.26$ for $H$ and $He$. All the remaining elements of the periodic table – commonly referred to in astronomy as “metals” – make up just the final two percent of the mass., denoted as a “*metallicity*” $Z ≈ 0.02.$ - ***Fundamentals of Astrophysics***







---
## Polarization of light

Light is an electromagnetic wave, with perpendicular electro and magnetic forces:
![[EM light.png|400x270]]

If the directions of *electric fields* in the p**lane perpendicular to the direction of propagation** are not evenly distributed, the radiation is ***polarized***. Polarization can be linear, circular or elliptical, depending on the direction the electron vector is pointing in relation to the plane. 

If this polarized ray of light travels in a magnetic field, it will start to rotate under **Faraday rotation**. It is proportional to the component of the magnetic field parallel to the line of sight, number of electrons along the line of sight, distance travelled, and square of the wavelength of the radiation.

- n Scattered is when light is absorbed and immediately released back, and **it is always polarized**.

# Describing the hydrogen atom
---
We can describe this atom using **Bohr's model** that electrons move around like in **planetary orbits**
- !! Which is completely false! However, it *has been shown that* it has success when it comes to the hydrogen atom. And only that one :LiSmile:

Using the conservation of [[Angular momentum]]:$$mvr = nℏ$$, where ℏ is $h/2\pi$, m is the mass of the electron, v is the velocity, and r is the distance of the orbit, n is the principal quantum number (shell).
- eg Radiation is emitted only when the electron jumps from a higher energy state to a lower one!!! (Bohr's second postulate)

So, the energy difference is:$$h\nu = E_{n2} - E_{n1}$$
Using [[Coloumbs law]] we can determine the energy of an electron. By using the equivalence of circular motion force and coloumb's force, we get:$$\frac{mv_n^2}{r_n} = \frac{e^2}{4\pi \epsilon_0 r_n^2}$$
Using the 2 main relations we get:
- f $$v_n = \frac{e^2}{4\pi \epsilon_0 n  ℏ}$$
And:
- f $$r = \frac{4\pi \epsilon_0 n^2  ℏ^2}{me^2}$$

And finally, the energy of the orbit is the kinetic plus this energy:
- f $$E = \frac{1}{2}mv_n^2 - \frac{e^2}{4\pi \epsilon_0 r_n^2} = \frac{-me^4}{32\pi^2 \epsilon_0^2ℏ^2n^2} = -C\frac{1}{n^2}$$, where $C$ is a constant (since all the values except n are constants).

We can apply this same approach with wavelengths of electrons instead of frequencies, but this constant would be called **Rydberg's constant**. 
- f $$\frac{1}{\lambda} = R(\frac{1}{n_1^2} - \frac{1}{n_2^2})$$

![[hydrogen lines detail.png|500]]

# Line profiles - why do spectral lines look the way they are
---
Even though lines give the illusion of being super sharp, in reality, due to different quantum effects they are a tad blurry. We are going to try and analyze why they appear to be fuzzy.

Due to the Heisenberg uncertainty principle, we cannot know an electrons **position and speed** at the same time, not **its energy and time at the same time**:
- f $$\Delta x\;\Delta p \approx \Delta E \Delta t \approx \frac{h}{2\pi}$$

we know that a change in frequency is proportional to energy and inversely proportional to the planck constant, and as well as using the previous statement, it can be shown that:
- f $$I_v = \frac{\gamma\;I_0}{2\pi (\nu-\nu_0)^2 + \frac{\gamma^2}{4}}$$, where $\gamma$ is the **natural width of the line** and $I$ is the intensity:$$\gamma = \frac{\Delta E_i + \Delta E_f}{h/2\pi} = \frac{T_i+T_f}{T_iT_f}$$, where $T$ is the time of excitation, and $i, f$ signalize the initial and final states.

![[intensity of spectral line.png|400]]

At the centre, maximum, the intensity is exactly:$$I = \frac{2}{\pi \gamma} I_0$$, while for $\nu = \nu_0 + \gamma/2$, it is exactly one half of the intensity, which means that at this frequency we have the **FWHM** or Full Width Half Maximum. 

Other than using the Heisenberg principle, due to the atoms/molecules of gas constantly moving around in a thermal environment (they have kinetic energy), [[The Doppler effect]] gives us a way to track the movement of these atoms, which skew the lines.
	![[doppler broadening.png|300]]

The dotted out part is due to the broadening, but the area of the curve stays the same. This is also called the **Voigt profile**.

We can find an **equivalent width** when the area of the rectangle in the image up above is the same as the area of the curve, and use this value to calculate the rest. 

# Using quantum mechanics to describe an electron
---
This is where we enter the world of quantum mechanics. Quanta is just a notion that each property of an electron has little packets of "something". It can be energy, a quantum number, angular momentum, etc. We define **4 quantities to describing an electron, or well any particle.**
#### 01 Principal quantum number, or $n$
This is the one we have encountered so far. It tells us the quantized energy levels inside an atom. It tells us how much energy an electron can have in a certain shell of an atom.

#### 02 Angular momentum quantum number, or $l$
The orbital angular momentum of an electron, which is somewhere in the electron cloud, whizzing around the atom in a probabilistic orbit, is quantized as such:
- f $$L = \sqrt{l(l+1)\frac{h}{2\pi}}$$

$l$ has to be a whole number, from 0 to n-1. A specific angular momentum number corresponds to **a specific electron [[Orbitals]]**, like s, p, d, f,... 

- n Although l determines the magnitude of the angular momentum, it does not give its direction. In a magnetic field this direction is important, since the orbiting electron also generates a tiny magnetic field.

#### 03 Magnetic quantum number
If we project our angular momentum onto the axis of the direction of the applied magnetic field, we get:$$L = m_l\frac{h}{2\pi}$$, where $m$ is the magnetic quantum number. This number **splits the spectral line into multiple parts,** depending on what the angular momentum is. Due to the magnetic field, lines differentiate into multiple states since the magnetic quantum number can be in multiple states for one angular momentum value. (**Zeeman effect**)

![[zeeman effect.png|300]]

#### 04 Spin
Probably the most elusive concept, **[[Quantum spin]]**, defined with $s$. 
- f $$S = \sqrt{s(s+1)\frac{h}{2\pi}}$$

Spin helps make fine spectrum shapes, like double lines or close lines.

---
The total angular momentum of an electron is:$$J = S + L$$ or $$j = l +- \frac{1}{2}$$
# How does the state of an electron change?
---
Now that we can describe an electron and understand the quantum mechanics properties of these cool particles, we can use this knowledge to further analyze spectral lines!

#### Electric dipole transitions
These are the most likely, where an atom behaves like an oscillating dipole! There are other types, but they are **forbidden** as they are only possible if a gas is rarified (aurora, planetary nebulae) and are suuuuuuuper rare. 

The laws for this transition are:
- $\Delta l = ± 1$
- $\Delta m_l = 0, ± 1$
- $\Delta j = 0, ±1$
- $\Delta m_j = 0, ±1$

An interesting thing is that out of these forbidden states, one transformation, **magnetic dipole transition**, which allows electrons to switch between parallel and antiparallel states of spin, giving rise to the **famous 21 cm hydrogen line** from the super rare gas of our galaxy.
![[21 hydrogen.png]]

#### Population numbers
What are they? The population number $n_i$ of an energy state i means the number of atoms in that state per unit volume. In thermal equilibrium, the population numbers obey the Boltzmann distribution:
- f $$\frac{n_i}{n_0} = \frac{g_i}{g_0}e^{-\Delta E/(kT)}$$, where $k$ is the Boltzmann constant, $E$ is the change in energy (equal to $h\nu$), $g_i$ is the statistical weight of the level i (it is the number of different states with the same energy Ei). 

## What about molecules?
---
Since they are much more complex than singular atoms, their **rotation** gives rise to different spectral lines. In the case of a molecule, there are many more possibilities: atoms can vibrate around their equilibria and the molecule can rotate around some axis. Both vibrational and rotational states are quantized.

# Intrinsic radiation - Blackbody radiation
---
![[blackbody radiation.png|300]]
- eg Blackbody radiation is when a **blackbody,** or an object which absorbs all wavelengths of light, radiates a from a certain range of wavelengths based on its temperature. 

> Planck showed that as thermal motions of the material approach a *Thermodynamic Equilibrium (TE)* in the **exchange of energy between radiation and matter**, the SED can be described by a function that depends only on the gas temperature T (and not, e.g., on the density, pressure, or chemical composition). 
---

We can quantify the intensity of light for a given wavelength with Planck's formula of distribution:
$$I(\lambda, T) = \frac{\frac{2hc^2}{\lambda^5}}{e^{hc/\lambda kT} - 1}$$

==**Wien's displacement law**== is about the relationship between the most preferred wavelength(color) and temperature of a blackbody object. $$\lambda_{max}T = 0.002897755 \;m \;K$$
We can extract Wien's law by using a bit of calculus: we notice how the higher the energy or intensity, the shorter the peak wavelength. We need to find a peak, or where the derivative equals 0:$$[\frac{dB_{\lambda}}{d\lambda}]_{\lambda = \lambda_{max}} = 0$$
> While using SED is a great way *in theory* to calculate a star's temperature, real SEDs of stars are not quite like blackbodies, and using this simple law to create an intensity graph is not very precise. The reason why its not the same is because of **absorption lines.** They cause disturbances in the SED, which makes it hard to calculate temperature. It's just easier to use **[[The color index]].**

---

We can use Wien's displacement law and the Planck distribution to create a simplified version of the distribution function for wavelengths which approach the maximum wavelength (or above the maximum wavelength) determined by Wien's law.
$$e^{hc/(λkT)} ≫1$$
Is our starting approximation, and hence:$$I_\lambda(T) \approx \frac{2hc^2}{\lambda^5}e^{-hc/(\lambda kT)} $$
When $hc/(λkT ) ≪ 1$ ($λ ≫ λ_{max}$), we have
$$e^{hc/λkT} ≈1+hc/(λkT)$$, or finally the **Rayleigh-Jeans approximation**
- f $$I_\lambda(T) = \frac{2ckT}{\lambda^4}$$

---

As the temperature increases, as we can see from the image above, the wavelength decreases, meaning hotter objects are lighter in color! [[Energy]] is inversely proportional to wavelength, so a spectrum shifted to higher energy needs to have shorter wavelength because then energy and temperature are proportional. If we wanted to calculate the total energy (luminosity) of an object which basically means the energy output from **all wavelengths**, we would integrate our intensity function ([[Stars]]) and come up with this: $$B(T) = \frac{\sigma T^4}{\pi}$$
We know that the intensity is **surface brightness multiplied by** $\pi$, and so:$$F_s = \sigma T^4$$, known as the **Stefan-Boltzmann law**.

And luminosity is literally just the total energy multiplied by the area of the star. An Austrian physicist Josef Stefan in 1879 showed that the [[Luminosity]] of a blackbody object with an area and temperature is given by:$$L = AσT^4$$
Later, Ludwig Boltzmann derived the ==*Stefan-Boltzmann*== equation using [[Thermodynamics]] and [[Maxwell's Electromagnetic Wave Theory]]. $$L = 4πR^2σT_e^4$$, where $σ$ is equal to $5.670400 × 10^{-8} \; W m^{-2} K{-4}$. We use the above equation to define the surface temperature of a star's surface. This is an awesome equation which ties together luminosity and temperature together! If we wanted to know the flux of the surface of a star, we would just divide by the surface are and get the following: $$F_{surf} =σT_e^4 $$Using this we can determine the ratio between radii and temperatures for 2 different stars:
- f $$M_{bol} - M_{bol1} = -5 log\frac{R}{R_1} - 10log\frac{T}{T_1}$$

And we can determine the temperature of a star from its angular size and flux density:
- f $$F = (\frac{\alpha}{2})^2\sigma T^4$$


---
Other than Planck's equation for the intensity of light, we can say that **intensity is the flux per solid angle**, or:
$$I = \frac{F}{\Omega} = \frac{L}{4\pi^2 R^2}$$

![[surface brightness and solid angle.png|400]]

> By the above 3 ways of describing the light from a star: *absolute* (***luminosity***), *apparent* (***flux***) and *intrinsic* (***surface brightness***).

---

The **color temperature** of a star is the ratio of its flux densities for 2 wavelengths using the planck distribution. The thermal temperature is equal to $E = \frac{3}{2}NkT$, where $N$ is the number of atoms in a gas. The pressure is equal to $P = nkT$, where $n$ is the density or amount of particles per volume. 


## But, why is it like this? 
---
Why do objects glow when [[Heat]] is applied or when they produce heat themselves?

[[Atoms]] are made of [[Electron]]s, [[Protons]] and [[Neutrons]]. The electrons make up the ==electron cloud==, and each cloud is shaped into [[Orbitals]]. Each orbital has a specific energy level, as they are placed in specific [[Electron shell]]s. So, in order for **an electron to switch between orbitals, specific packets of energy are required!** So, the change in the position of an electron inside the atom creates [[Light]]! 

- eg If an atom vibrates at the right frequency due to heat being acted upon the atoms, the change in energy can cause the electron to jump the "ladders" or orbitals in the electron cloud. After the excitement, the electron ultimately wants to return to the ground state, and then it releases that energy in the form of photons.
- n You can probably notice the similarity between [[Blackbody radiation]] and [[Spectra]] and [[Spectroscopy]], except in spectroscopy its not inner heat which causes atoms to produce spectra (at least in cold clouds), but rather the hitting of light upon material and giving it energy.

So, that's why blackbody radiation works. The internal heat of an object heats up its atoms, and when they bump and vibrate against each other and even partly share their electron clouds and getting even more energy, they emit even more light. This is why ==hotter [[Stars]] glow brighter and vice versa==.

But let's be more specific. What exactly happens in stars?

#### Blackbody radiation in stars
---
So, in stars we have a new type of material, [[Plasma]]. Here, electrons ==are detached== from their "host" atoms, and so they aren't bound by their energy usage. These electrons are called **free electrons**, and they can contain as much energy as they want! However! Since there are many free electrons in the cores and layers of stars, they bump into each other ==a lot==, **significantly reducing their kinetic energy**: this reduction causes them to release photons to mediate that change in energy: and voila! Blackbody radiation or light is emitted from stars at a very high rate! 

- eg In a nutshell, blackbody radiation is the **radiation that comes from within the object and isn't reflected or transmitted by other light sources**. The hotter an object is, the more it becomes a blackbody object and transmits and reflects less light. 

So the core principle of  these stars is that they try to approximate **thermodynamic equillibrium**, which basically means that there is <mark style="background: #d4a373;">no net energy flow between the star and the surroundings</mark>.
