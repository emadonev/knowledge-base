---
tags:
  - star
  - gas
  - medium
  - astronomy
  - physics
  - mathematics
  - galaxy
  - star_formation
---
While as much as we want to observe the night sky with [[Telescopes]], [[Detectors and instruments]], there is a little something making everything just a bit harder. **The interstellar medium**, filled with stuff blocking the transfer of light ([[Photometric quantities]], [[Radiation mechanisms]]). It is also the birthplace of stars, and [[Star formation]] is crucial for the rest of the universe.

# When interstellar went extinct
---
What exactly is blocking the light though? 2 processes:
1. **Scattering** - the photon of [[Light]] is bounced about, with its direction changed.
2. **Absorption** - the photon and its energy remain within a dust grain of the interstellar medium.
![[extinction light.png|300]]

The combination of both of these is called **interstellar extinction**. The amount of light which went "extinct" is discussed in [[Photometric quantities]] with **optical depth** of the dust. 

### Counting stars
---
Since not all light reaches us, then **we won't be able to see some stars**, they will be too faint for us to see through the interstellar medium. If an image has a limit of $m_0$, all stars brighter are visible. Account for extinction, only stars above $m_0 - A$ are visible. We can use an integrated stellar count and compare images with obstruction and images without obstruction to determine the number of stars.

### Turning red
---
It turns out that interstellar gas likes certain wavelengths of light more than others. The higher the wavelength, the more it is absorbed, leading the **interstellar reddening.** 

![[interstellar reddening.png|300]]

We can compare the absolute and apparent magnitudes of a star in different wavelengths, for example Visual vs. Blue (we can choose any range, and adjust accordingly.) We know then that if we subtract one distance formula from the other, $r$ cancels out and we get:$$m_B - m_V = M_B - M_V + (A_B - A_V)$$ We can gain the 2 quantities of magnitudes from observation, but the correction we need to calculate. Since both values are proportional to the **dust column density**, we can define some number $R$:
$$R = \frac{A_V}{A_B - A_V}$$
Which is called **ratio of total-to-selective extinction**. Through experiments, it has been shown that $R$ is typically equal to $3.1$, which is great! We only use this information to gain information about everything else on the star. 

### Modelling curves
---
By tracking how extinction changes depending on the wavelength of light, we can gain information on the medium. However, we need a plot **independent of the dust column depth**, so we divide by $A_V$ or $A_B - A_V$. The function is:$$f(\lambda) = \frac{A(\lambda)}{A_V}$$
![[extinction by wavelength.png|400]]

And we can se a clear bump. This means that *infrared light is the best absorbed wavelength of the lower types.* We will see that this comes in handy later.

# Dusty grains
---
Now, let's talk about the constituent of the interstellar medium - **dust grains**. 
### A physical exam
---
The size of a grain depends on the extinction of a wavelength. If $A(\lambda)$ is constant and $r << \lambda$, then the dust grains are too small for the wavelengths to bounce of so we can see them. If $r$ is comparable to $\lambda$ then diffraction tells us about the size.

Through observation, we have deduced that there are 2 general categories of dust with their own size distributions.

When it comes to shape, we use **polarization** to tell us if they are perfect spheres or some other shape. If the light just bounces off in any direction, it indicates a sphere, but if polarization is present, then the dust grains are elliptical in shape or flat-like. 

### A looksy inside
---
We use spectra to analyze the composition of larger grains, but we look at their infrared spectra rather than visual. Since they are tiny, the lines are a bit smudged. However, we found the presence of $SiO$ and $SiO_2$, and water ice. Since silicates are found on Earth in dirt, we call grains **dirty ice.** 

![[spectra of grains.png|300]]

However, extinction present in the ultraviolet part of the spectrum indicates that **carbon** must be present, so we think that *small graphite grains* help in the interstellar medium. 

The teeniest tiniest grains are around 1 nm across, and they are made of **aromatic hydrocarbon formation of carbon.** These are called *polycyclic aromatic hydrocarbons or PAHs*. 

It has been suggested that grains are actually not just a lump of something, rather they are differentiated like planets with tiny layers:
![[differentiation grain.png|200]]

### Electricity in the air
---
A little grain can become electrically charged if either charged particles strike the grains and stick on them, or photons bust out electrons due to the photoelectric effect, changing the charge balance. 
##### And strike
---
Electrons, being small, have a greater average speed than protons or ionized atoms, and they bombard the grain and transfer their charge. After a certain amount of time, protons will start to get accelerated, and the charge is conserved. 
If we want the charge to be conserved, electric potential and kinetic energies have to stay the same. The net charge on the grain is $-Ne$, and the potential energy is:$$U = \frac{Ne^2}{r}$$, while the kinetic energy is:$$K = \frac{3}{2}kT$$Equating these two helps us see how large the charge is. However, this is a big approximation, since a portion of electrons which travel at super fast speed really increase the charge, and they aren't accounted for here.

### Its getting hot in here
---
The principle behind the temperature of a dust grain is the same as for a planet ([[Planetary properties]]) The amount of energy in is the same as the amount out. So, let's imagine a scenario with a dust grain, a certain distance from a nice star. Its luminosity is $L_s = 4\pi R_s^2 \sigma T_s^4$. We project the area of light striking is a circle, or $\pi r^2$, but at a certain distance $d$ from the Sun, in a spherical distribution, so $4\pi d^2$. Each grain also has its albedo, which is the amount reflected, but we need the amount **absorbed.** So, the rate of energy is:$$P = \frac{(1-a)(4\pi R_s^2)(\sigma T^4)(\pi r^2)}{4\pi d^2} = \frac{(1-a)\pi\sigma R_s^2T_s^2r^2}{d^2}$$
- n The quantity $\pi R_s^2/d^2$ is a **solid angle** as seen from the star to the grain. So, the star is like a **dilute blackbody**, as it has a blackbody spectrum with its intensity down by a factor of a solid angle. 

The power radiated by the grain is:$$P_g = (1-a)\pi r^2 \sigma T^4$$
Why $(1-a)$? Because that is the amount of radiation it can absorb, and can only emit that much as well. (It doesn't have internal heating or things like that).

Equating the two values and doing some math tells us that:
- f $$T = T_s\sqrt{\frac{R_s}{2d}}$$

---
We actually know extremely little about the evolution of dust grains. Our current theory is that they form in the atmosphere of a red giant, get detached, solidify into tiny grains, get blown off into the interstellar medium, where after a long time they can form a new star.

# Interstellar gas
---
## Various studies of light
---
We use spectroscopic studies of light to detect the presence of molecules and compounds. Using optical light, we could only detect reactive particles and unstable ones, like $CH$, $CN$, and $CH^+$. This indicates that the gas cloud is generally quite not dense, as these compounds would have reacted with something if it were. By looking into the ultraviolet, we found Lyman lines, indicating the presence of hydrogen.

The lines of the medium are much narrower than the lines from stars, so we can differentiate them. An interesting note is that not all stars have medium spectra in them, suggesting that **it is clumpy, and not uniform**. 

### The 21 cm line
---
![[21 cm H line.png|300]]
As we discussed in [[Radiation mechanisms]], each particle has a **spin** associated with it. The relative orientation of the spins affects the magnetic force between the electron and proton. The energy difference between aligned spins and opposite spins is 1400 MHz, or *the 21 cm line*. The temperature needed for this magnetic reaction to take place is 0.07 K, which is **extremely cold**. 

The 21cm line is extremely useful for studying the composition of interstellar gas,  calculating its density, temperature, for the analysis of galactic motion, etc. 

![[spectra of 21 cm line.png|300]]

We can see that the **Zeeman effect** is present in the lines, and the amount of shift indicates **the strength of the magnetic field of the gas**. (as seen above) 

With the help of the 21 cm line, we have discovered the following:
- n Typical clouds have the following physical parameters: temperature, 100 K; hydrogen density $n_H \approx 1-10 /cm^3$, lengths of tens of parsecs; hydrogen column densities up to $1021 cm^2$. The clouds fill about 5% of the volume of interstellar space, meaning that the average density of atomic hydrogen in interstellar space is of the order of $0.1 cm^3$

We also found structures called $HI$ shells,:
![[hi shells.png|300]]
Which depict the spiral structure of the milky way.

---
Since the medium is grouped into clumps, we have interstellar medium, and intercloud medium. Their pressures **are the same**. 

# Molecules galore
---
By conducting regular calculations of the probability of complex molecules forming, like $CO$ or higher order molecules, we realized that it was extremely small. We needed to account for the quantity of each specific element, the speed at which they are traveling and the area where they can meet. We also had to account for the high energy photons crashing into these molecules and breaking them apart. 

However, by doing some actual research at millimeter lengths of wavelengths, we found an enormous amount of molecules! The list includes things such as formaldehyde, methyl alcohol, $HCO^+$, $SiO$, $CH_3C_4H$, etc. There are over a hundred molecules present in the interstellar medium. 

The reason we don't see the 21 cm line in these clouds is because the hydrogen **has converted into molecules of $H_2$,** which don't show up on spectra. We differentiate a few types of clouds:
1. <mark style="background: #C2E812;">HI clouds</mark> - clouds where we find hydrogen in the mostly atomic state
2. <mark style="background: #190E4F;">HII regions </mark>- clouds where hydrogen is mostly ionized 
3. <mark style="background: #B33C86;">Molecular clouds</mark> - clouds where hydrogen is mostly molecular $H_2$

---

Of course, having molecules is great, but we need to figure out how they form and also, how they interact together in the medium. This is where the super important **dust grains** come in. 

![[interstellar chem.png|300]]

2 $H$ atoms can come onto the surface of a dust grain, where it provides the area necessary for them to combine together. Once they do, energy is released into the grain, heating it up, and the $H_2$ goes of into the medium. However, most molecules don't form this way, since a gaseous environment is required. However, using **ion-molecule** reactions and a much higher (now known) density of the interstellar medium, things become more likely. 

Since dust grains are negative (discussed earlier), the medium has to be positive, which is confirmed by the high amount of positive ions found. 
![[electric dipole interstellar.png|300]]

Even though the molecule has an overall net 0 charge, tiny polarization of the molecule enables an electric dipole to form, where the negative part is attracted to the positive ion, and so the entire molecule moves.

---

How do we observe these molecules though?

Normal electron transitions are not possible for such a cool cloud, and neither are vibrational transitions. The only thing left is **rotation**, specifically the ***rotation of the molecule end-over-end***, which we can detect.
A molecule with angular speed $\omega$ and rotational inertia $I$:$$E = \frac{1}{2}I\omega^2$$ Angular speed can be rewritten as:$$\omega = \frac{L}{I}$$, where $L$ is the total angular momentum. Total over inertia is speed (kind of like mass and velocity). 

And now, the energy is:
- f $$E = \frac{L^2}{2I}$$

We can **quantize** this energy by introducing $J$, we can describe the energy as:
- f $$E = \frac{J(J+1)(h/2\pi)^2}{2I}$$

The higher the $J$ value, the more spaced out the energy levels are, making them harder to achieve in the cold interstellar medium. The reason why so many molecules are observed in the millimeter part of the spectrum is because it corresponds to low energy changes for small $J$. 

# Thermodynamics of the medium
---
- eg **Temperature** - the balance between heating and cooling / average kinetic energy per particle

The easiest and most common way of heating a gas is with **photons!** 
1. **Heating the dust** - photons strike the dust grains, grains heat up, they hit other things, the medium has increased kinetic energy
2. **Excitation** - a photon collides into an atom or molecule, they get excited, bump into another atom/molecule, transfer the energy and return to a lower state, but the next atom/molecule is excited now
3. **Ionization** - a photon knocks out an electron from an atom, and this electron wreaks havoc, bumping into stuff all the time, increasing kinetic energy
4. **Photoelectric effect** - a photon strikes a grain, an electron gets ejected, bumps into everything

Other than photons, **cosmic rays** are also responsible for all of these processes. On the large scale, [[Supernova]]s, explosions, etc. can transfer their kinetic energy onto the medium. 

When it comes to cooling, energy **has to be taken away** from the system. 
1. **Emission from grains** - an atom/molecule bumps into the grain, losing some energy, and the grain radiates that energy away
2. **Excitation** - collision of excited atom/molecule into unexcited atom/molecule, with the second one going back to its ground state before it collides with another molecule/atom. 
3. **Ionization** - after the ionization of an atom/molecule, it bumps into another one, the second ionizes but **recombines**, and emits a photon.

Specific atoms/molecules heat up or cool down the gas, which gives rise to various pockets of cool medium, around 10 K to very hot packets of gas reaching 100000 K. 

