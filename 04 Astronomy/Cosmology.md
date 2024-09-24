---
tags:
  - cosmology
  - galaxy
  - astronomy
  - physics
  - mathematics
---
In complete opposition to quantum mechanics, **cosmology** deals with the science of the large, with how the universe overall works, and how simple physical laws can explain how we got here. We deal with the universe as a **fluid**, and ignore the lumps, like stars, galaxies, etc. 
- eg The *main force at play here* is the **gravitational force**!!

The base all of our models on one principle, called ==the cosmological principle==. 
It states that *on the largest scale the universe* is:
1. **homogenous** - at each instant(on average) has the same properties (density, composition) are true everywhere
3. **isotropic** - at each instant, the universe appears the same in all directions.

# Why is the sky dark?
---
This was the question Heinrich Olber asked in his book, and it proved quite a difficult question to answer. If there are so many stars in the universe, why hasn't all of their light reached us, and why isn't the night sky just one giant surface of a star, enormously bright? [[Olber's paradox]], was a very famous paradox, and from it we gain the knowledge that the ==**universe has a finite size or age (or both).**== If it has either of these, the amount of stellar radiation from stars in concentric circles around the Earth, $dr$ in thickness, some light would have never reached us since we need to cut off at one point.

# Expansion tracking
---
Due to the homogeneity of the universe, we can actually Show Hubble's law. If we are tracking the change in length of vectors from an observer at point $P$ to points $O$ and $O'$, we would get lengths $r$ and $r'$. The difference in space between $O$ and $O'$ is $a$. The velocity function from $P$ to $O$ is the same as to $O'$. This means that $$v'(r-a) = v(r-a)$$, or that $$v(r-a) = v(r) - v(a)$$, so $v$ is a linear relationship with $r$. And Hubble's law is that velocity is linearly dependent on distance, or $$v(r) = H(t)r$$

# Newton in the mix
---
Using newtonian mechanics for the acceleration of the expansion of the universe, the fact that the density changes since it expands, etc. we gain:$$a = \frac{8\pi}{3}\frac{G\rho_0}{R} - k$$, where the fate of the universe depends on the factor $k$. 
1. If $k = 0$, then the universe always expands, but the acceleration decreases with time, it becomes smaller. 
2. If $k>0$, then the universe expands to a point $R_{max}$, which is equal to:$$R_{max} = \frac{8\pi G\rho_0}{3k}$$, and then starts to collapse. We call this a **closed universe.**
3. If $k<0$, then the expansion continues forever, and this is an **open universe**. 

Now, we want to know **if the universe is open or closed**. That's a pretty important question, as it decides the fate of the universe. 

We define a **decceleration parameter** which tells us if it is open or closed, or in the middle, with $k = 0$. It is equal to$$q = \frac{4\pi G\rho}{3H^2}$$, where the ranges of $q$ depend on $k$. 
1. If $q>1/2$, with $k>0$, then we have a closed universe. 
2. If $0<q<1/2$ and $k<0$, then we definitely have an open universe.
3. If $k = 0$, then $q = 1/2$, and the universe is neither open nor closed.

What is the decceleration parameter related to? Probably the density of the universe. If we have a **critical density**, one where if the density of the universe is above it is open, and if below it is closed, can be defined based on the things we previously said.
- n Based on the explanation above, **the critical density must be calculated from the scenario where $k=0$ and $q=1/2$ in the equation above**.
Using this, we can see that 
- f $$\rho_{crit} = \frac{3H^2}{8\pi G}$$

Finally, we can define a quantity called the **density parameter**, which tells us how much above our true density is above the critical one. We say:$$\Omega = \frac{\rho}{\rho_{crit}}$$, and if we use Einstein's biggest blunder, "the cosmological constant", $$\Omega = \frac{\Lambda}{8\pi G \rho_{crit}}$$

If our universe is really at $k>0$, then after reaching the critical radius, it will collapse again, back into one tiny spot with a ton of energy and matter. Will the universe form again? Maybe. This theory is called **the oscillating universe**, where we constantly go about a cycle of formation and destruction. 

- n For a flat universe, $$\Omega_M + \Omega_\Lambda = 1$$, where $\Omega_M$ is the density parameter of matter, and $\Omega_\Lambda$ is the density parameter with the cosmological constant.

Different values of $k$, $q$ and $\Omega$ actually dictate the shape of the universe.
![[shape of uni.png]]

![[parameters for universe.png|500]]

# Doppler becomes cosmic
---
Since the universe is expanding, it is fairly logical that we observe a **cosmological redshift**, due to space itself expanding between us and distant galaxies, causing redshift. So, photons are expanded by the same amount depending on the expansion.

And so, we get that:$$z = H_0 \Delta t \ce{->} cz = H_0 d$$

---

But, why is it important if the universe is open or closed? Because, the actual shape of the universe changes, and then **most of our equations for light, radiation, flux, apparent magnitude, etc. have to be adjusted for the shape.** 

So, which is it?

A huge problem is dark matter. If we could only determine the density of our universe, we could start making some progress. Unfortunately, since we have no idea what dark matter is, we cannot really estimate the density of the universe as it makes up such a huge portion of total matter. 

We could count the number of radio sources in each shell of our universe, and see how they fall off with distance. Results thus far have been consistent with $1/r^2$, or a flat universe. The research done with the formation of elements in the big bang support an open universe. So, everything is still on the table. 

# The big bang!
---
If the universe is expanding right now, at a certain point it used to be a **tiny point in space**. We call the theory where the universe expanded from such a point **the big bang theory.** 

After the "explosion" of the big bang, the universe was super hot plasma filled with electrons and protons and neutrons. This plasma was quite dense, or opaque, so **photons couldn't pass through.** As the universe cooled, it reached the **recombination phase** where atoms formed, and neutral atoms don't scatter light so well, they absorb certain wavelengths [[Radiation mechanisms]], and so **light could travel through the universe**! This light, with a big redshift, kept traveling in the background of the universe, waiting to be observed as **cosmic background radiation.** Arno Penzias and Robert Wilson in 1965 discovered the cosmic microwave background, and determined that the radiation was blackbody at 3 K. 
![[cmb spectra.png]]
After many measurements with the COBE satellite, we determined that the cosmic microwave background is truly blackbody, with super tiny errors compared to the ideal blackbody curve. 

Even though we consider the CMB homogenous, it is actually necessary for there to be tiny pockets of slightly hotter material, which would later form galactic clusters, galaxies, and eventually stars and us. Using another satellite, BOOMERANG, which is actually an observing ballon, we managed to observe a pretty detailed picture of the CMB, which really points to a flat universe. ![[boomerang.png]]

### Compton scattering
---
Slight detour for a cool scattering effect: when photon initially has more energy than an electron, when they interact energy is transfered, and the photon loses energy, and changes wavelength. Inverse compton scattering is the opposite, when the electron has more energy. In the intercluster area, **inverse compton scattering occurs, since $e^-$ have more energy than $\gamma$**. 

> Photons get a large boost in energy, going in as radio wavelength photons and coming out at shorter wavelengths. This means that if we look in the directions of clusters of galaxies at radio wavelengths, some of the background radiation will have been removed - **Sunyaev–Zeldovich** effect

# T-3 minutes
---
This period was characterized by very high temperatures, perfect for nuclear reactions which could spark the creation of elements (or at least the nuclei of these elements) by fusing hydrogen nuclei to form helium nuclei. These further fused in the first 3 minutes, albeit most matter after hydrogen and helium was made in stellar explosions after the big bang. 
![[abundance of elements big bang.png]]

# Fundamental everything
---
But, what happened in the first second? Here, we need to explore elementary particles which make up our little protons and neutrons, as they reveal a lot about the beginning of the universe.
![[fundamental aprticles.png]]

Leptons obey the Pauli exclusion principle and don't interact with the strong force, while Hadrons do not obey the principle, but interact with the strong force. While leptons really are elementary, neutrons and protons are further made up of **quarks**, which are suuuuper tiny:
![[quark powers.png]]

We call the different types of quarks **flavors**, even though they aren't real colors, but they help us understand that quarks cannot show up single but always in pairs, as only **colorless** quark configurations are allows (the colors cancel out).


- n Every single particle of matter has its own **antiparticle**, and when they meet they annihilate each other. 

Other than particles, we have the 4 fundamental forces, **gravity, electromagnetic force, strong and weak nuclear force.** The only one which doesn't fit in with quantum mechanics is **gravity**, as it doesn't have a carrier particle (which we have seen yet) and it difficult hence to integrate with everything. 

# The flow of time
---
So, let's finally answer some questions. 
![[after big bang.png]]

1. We cannot say anything about the first $10^{43}$ seconds, or Planck time. To describe phenomena on this time scale we need a *quantum theory of gravity*. It is even possible that the continuous fabric of space-time breaks down at this scale.
2. Due to spontaneous symmetry breaking, more matter was in the universe than antimatter, which enabled everything around us to exist. As the particle and antiparticle particles annihilated each other, 2 photons were produced as energy of the collision, which is why there are **so many photons per baryon in the universe**.
![[matetr antimater inbalance.png|300]]
3. At $10^{-35}$ seconds, the **baryon number was conserved**, and no more antiparticles remained, and the symmetry between the electroweak theory and color theory broken.
4. By $10^{-12}$ seconds, the electromagnetic and weak forces divided. 
5. By $10^{-6}$ seconds, quarks were confined to their baryons, or protons and neutrons
6. Neutrinos and matter decoupled, just as radiation and matter decoupled 100000 years later, when the universe became matter dominant rather than radiation dominant. 

There is a little stitch in this timeline, called **inflation**. Here it is thought that the universe rapidly expanded, and then normal expansion resumed, when the nature of **the vacuum changed.** This is still all a bit speculative. 

Inflation might give us the appearance that the universe is flat, since so much of it expanded suuper fast, it is outside of the observable universe, we can't see further, not enough time has passed, hence it appears flat. 

So, with all the knowledge we currently posses, here is the summary:
1. The Hubble constant most likely has a value of $70 km/s/Mpc$. 
2. The Hubble time is most likely 14 billion years.
3. The universe appears to be flat, by inflation and by small scale fluctuations of CMB.
4. If it is flat, then we approximate $\Omega_M$ as 0.3, and $\Omega_\Lambda$ as 0.7. 
5. The effect of the cosmological constant is to make galaxies fly apart - the expansion of the universe might be increasing (**dark energy**)

