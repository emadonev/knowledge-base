---
tags:
  - star
  - star_formation
  - astronomy
  - physics
  - math
---
# Gravitational [[Potential energy]] 
---
We can approximate [[Stars]] as uniform spheres with a uniform particle density since there is an enormous number of particles, as describing the actual state would be way too complex, and this is a fairly good approximation. So, the mass of that star would be:$$M(r) = \frac{4\pi}{3}r^3\rho$$
And the gravitational potential energy is really the **work required to bring all of that material with mass M from infinity to the radius of the star**. To help us achieve this, we layer shells of a star with thickness $dR$, and slowly build up the end star, as the cloud collapses. Since work isn't dependent on the process, we can use [[Integrals]] to calculate this. 
![[potential_energy_star.jpeg]]
If we wanted to calculate the change in volume for a specific layer of the star, it would be:$$dV = 4\pi r^2\ dr$$, with $r$ being the radius at that point, $dR$ being the thickness. Since we know the relationship between [[Mass]], volume and density, we can calculate the change in mass for a particular layer:$$dM = 4\pi r^2 \rho \ dr$$
The gravitational potential energy between any 2 points is:$$U = \frac{-GMm}{r}$$
which we can modify into the following equation:$$dU(r) = \frac{-GM(r)dM}{r} = -G\frac{16\pi^2}{3}\rho^2\ r^4\ dr$$
using [[Derivatives]] to help us quantify each layer and its change. (there is no fraction since $r^5$ canceled out with the r on the bottom) Now, we need to integrate $U$ over the entire radius of the star, so from 0 to $R$. We achieve this the following way:$$\begin{aligned}
U = \int_0^R dU(r) \\ 
= \int_0^R -G\frac{16\pi^2}{3}\rho^2\ r^4\ dr \\
= -G\frac{16\pi^2}{3}\rho^2\ \int_0^R r^4 dr \\
(antiderivative \ of \ r^4 \ is \ 1/5r^5)\\
= -G\frac{16\pi^2}{3}\rho^2 (\frac{1}{5}R^5 - \frac{1}{5}\ 0^5) \\
= -G\frac{16\pi^2}{3}\rho^2\frac{1}{5}R^5 \\
= -\frac{G\frac{4^2\pi^2}{3^2}*\frac{3}{1}\rho^2\frac{1}{5}R^6}{R} \\
= -\frac{\frac{3}{5}G(\frac{4\pi}{3}\rho \ R^3)^2}{R}\\
= -\frac{3}{5}\frac{GM^2}{R}
\end{aligned} 
$$
We can use this equation to determine the total thermal energy we would gain by **converting the gravitational potential energy into thermal energy**, using [[Thermodynamics]] for particles:$$K = \frac{3}{2} NkT, N = \frac{M}{m}$$, were N is the total number of particles which we can calculate with the mass per particle (which we know due to the composition of [[Molecular clouds]]), and the total mass. $k$ is the boltzmann constant and $T$ is the temperature in K. 

- n What is *Kelvin time*? This is the notion that perhaps *stars could use gravitational energy as their main energy source*, so this is the time which it could be possible to sustain, and its calculated by:$$t_g = \frac{E}{L} = \frac{-\frac{-3}{5}\frac{GM^2}{R}}{4\pi R^2 \sigma T^4}$$ And for  [[The Sun]] it is currently valued at 20 million years, which is nothing to the full lifetime of the Sun and even a glimpse into [[Earth]]'s history. So, obviously, [[Potential energy]] is not enough to power a star.

- eg What about **chemical energy?** This would amount to the energy released in chemical reactions, so a fraction of the **binding energy** would be released, around 1 eV per [[Atoms]] in the Sun. However, this would amount to *much less* energy than potential energy. Obviously, there must be something else at play.

However, we didn't really consider **which** type of chemical reactions we are looking at. While normal reactions give around 1 eV, [[Nuclear fusion]] brings around 1 MeV per atom, around $10^6$ times more energy per atom. Much better I would say. So, [[Nuclear physics]] is the key to stellar power.

# Nuclear physics - fusion in stars
---
We all know the fundamental properties of [[Atoms]]: they have a [[Nucleus]] which contains [[Protons]] and [[Neutrons]], with an electron cloud with [[Electron]]s. We also know that there are 4 fundamental forces in the universe: [[The universal law of gravitation]] (gravity), [[Electromagnetic force]], [[Strong nuclear force]] and the [[Weak force]]. The strong force is (as the name suggests) the strongest, while gravity is the weakest. 

- !! *gravity and the electromagnetic force* are long ranged, while the *nuclear forces* are short ranged and are noticeable on the scale of protons and neutrons. This ratio of forces depending on distance **keeps atoms in balance.** The neutrons inside the nucleus keep the electromagnetic force of repulsion between the protons in balance with the strong nuclear force pulling the neutrons and protons closer together. So, **atoms need approximately as many neutrons as protons** in order for them to keep stable.

### <mark style="background: #EA63Ac;">Binding energy</mark>
There is of course a certain amount of energy keeping the [[Nucleus]] in check. This is called the *binding energy* of the nucleus, and it is the amount needed to separate the individual components of the nucleus - hence it is also the amount which keeps it together. By this logic, <mark style="background: #f2e863;">the higher the BE, the more stable the nucleus is.</mark> 

We can calculate the binding energies of objects in MeV, and represent them with the following equation following Einstein's famous $E=mc^2$ law and the conservation of energy:$$M_{nucleus}c^2 + BE = Zm_pc^2 + Zm_nc^2$$
![[binding energy.jpeg]]

## <mark style="background: #BBE6E4;">Nuclear reactions</mark>

So, nuclear reactions are proving to be much more efficient as a stellar energy source, as the binding energy of the nucleus is around a **million** times greater than that of the [[Atoms]]. What are the types of nuclear reactions though? The first one is [[Radioactive decay]], with alpha, beta and gamma particles. Another type is nuclear fission, which is the action of breaking up the nucleus into smaller parts - used in nuclear reactors. And finally we have [[Nuclear fusion]], which is the **main source of energy for stars**. It requires light elements (in which stars are plentiful) however, it is <mark style="background: #f2e863;">difficult to begin fusion</mark>. In order to begin fusion, the strong nuclear force needs to overcome the electrostatic force of repulsion between the protons in the nucleus, which can only happen at *high energies and at very close distances (where the [[Strong nuclear force]] can act)*. 

- exp We can increase the **Kinetic energy** of a particle by *increasing the temperature*, since it is the average $E_k$ per particle - if the temperature is high enough, they will move fast enough to overcome electrical repulsion.

The good part is that *material is confined to the insides of a star due to **gravity***. If the temperature isn't high enough, we cannot start fusion, and we cannot have a star! So, what is the desired temperature?

Let's begin with a case of 2 protons trying to fuse together. (This is like saying that we want to fuse 2 hydrogen atoms together in the star, but since the material is plasma in the core, the nucleus is separate from the electrons). What we want to do is bring a proton from some distance, *r_p*, to the distance of 1 proton radius apart - basically bringing them together. Their [[Electric potential energy]] is:$$U = \frac{e^2}{r}$$, which is actually equal to the kinetic energy, as:$$E_{k1} + E_{p1} = E_{k2} + E_{p2}$$$$0 + U = K + 0, \;\;\;U = K$$
So, by doing that and **applying the fact that this is thermal energy**, we can see that the temperature required for **nuclear fusion** is around $2*10^{10} \;K$, which is a very high temperature. But, this is the average temperature required, which means that ==not every particle needs to be at this temperature in order for fusion to occur: a smaller fraction have to be, and by releasing this energy, other particles also begin fusing, etc.== 

- n By bringing 2 protons close enough together, we can *overcome electrical repulsion*, and then *nuclear attraction would begin due to the [[Strong nuclear force]].* This point is also called the **turning point**, as when a proton would come to this distance from another proton it would usually head away due to the repulsion.

##### How do protons pass this barrier between nuclear attraction and electrical repulsion?
They have to **quantum tunnel** to an area after the turning point - of course, there is a higher probability of the proton being far away from the turning point, but as we get closer, there *still exists a probability, it is just small*. A particle can only tunnel a distance approximatively equal to its wavelength, or $$\frac{h}{mv} \ce{->} \frac{1}{2}mv^2 = \frac{Z_1Z_2e^2}{r_0}$$, where if we plug this into the Maxwell-Boltzmann velocity distribution, we can see that an **optimal temperature exists for quantum tunneling**, called the **Gamow peak**. 

### Actual nuclear fusion part
---
- eg So, by calculating the mass difference between an actual fused helium nucleus and 4 individual protons, we can see that 0.007 of the mass is **converted into energy** (James Bond reference). 

By using this calculation, we estimate the Sun's lifespan to be around *ten billion years*!

#### <mark style="background: #B33C86;">The proton-proton chain</mark>
---
This is the most fundamental and most important reaction chain inside the Sun for energy production. It starts with 2 protons: $$p\;+\;p \ce{->} d\;+\;e^+\;+\nu$$, where d is a deuteron, $e^+$ is a positron, and $\nu$ is a neutrino. The deuteron now interacts with another proton:$$d\;+\;p \ce{->} \prescript{3}{}{\mathbf{He}} \;+\;\gamma$$, where $\gamma$ is a photon. This reaction occurs twice in order for a final helium nucleus to form:$$\prescript{3}{}{\mathbf{He}} \;+\;\prescript{3}{}{\mathbf{He}} \ce{->} \prescript{4}{}{\mathbf{He}} + 2p$$. The energy from this reaction is carried away by the photons, neutrinos and positrons. The positrons will anihilate with the electrons in the gas, effectively heating it up. The gamma ray will quickly also be absorbed into the gas and heat it up. The hotter gas emits new photons, which are later reabsorbed, etc. <mark style="background: #C2E812;">When they come close enough to the surface, they escape and we see them as light!</mark>

- !! The higher the temperature of the core of a star, the easier it is for particles to pass the barrier and fuse together!

### The triple-alpha process
---
For stars which have a higher mass than the Sun, they can fuse higher order elements, like in the triple alpha process. It starts off like so:$$\prescript{4}{}{\mathbf{He}}\;+\;\prescript{4}{}{\mathbf{He}} \ce{->} \prescript{8}{}{\mathbf{Be}} + \gamma$$. The third alpha comes into play after the beryllium is formed:$$\prescript{4}{}{\mathbf{He}}\;+\;\prescript{8}{}{\mathbf{Be}} \ce{->} \prescript{12}{}{\mathbf{C}} + \gamma$$

### The CNO cycle
---
For stars which are even more massive, there is a CNO cycle, which is quite important for energy production. It is a step after the triple-alpha process since it involves carbon, nitrogen and oxygen. 
1. $\prescript{12}{}{\mathbf{C}} + H \ce{->} \prescript{13}{}{\mathbf{N}} + \gamma$, which is brought on by the *strong force*. 
2. Next, via [[Beta decay]], the nitrogen decomposes into: $\prescript{13}{}{\mathbf{N}} \ce{->} \prescript{13}{}{\mathbf{C}} + e^+  + \nu$ 
3. Now, with this new isotope of carbon (which is highly radioactive), we can form a full nitrogen nucleus:$\prescript{13}{}{\mathbf{C}} + H \ce{->} \prescript{14}{}{\mathbf{N}} + \gamma$, mediated by the *strong force*, of course.
4. This shiny new nitrogen atom now can with a proton create deficient ==oxygen==:$\prescript{14}{}{\mathbf{N}} + H \ce{->} \prescript{15}{}{\mathbf{O}} + \gamma$.
5. So, the next step is to fix the oxygen via [[Beta decay]], where we get a super-nitrogen nucleus:$\prescript{15}{}{\mathbf{O}} \ce{->} \prescript{15}{}{\mathbf{N}} + e^+  + \nu$
6. And finally, we can get normal nuclei, and we are right back to where we started: $\prescript{15}{}{\mathbf{N}} + H \ce{->} \prescript{12}{}{\mathbf{C}} + \prescript{4}{}{\mathbf{He}}$
7. Voila!

- n In this specific cycle, the **carbon acts as a catalyst**, as it starts the reaction over and over again, stimulating nuclear fusion. 

But, what about higher elements? Well, the process is very similar, but it is important to note that ==the electrical repulsion becomes larger the greater the nucleus==. It is still able to catch neutrons, depending on wether they **travel fast or slow**. If a neutron approaches the nucleus slowly, it might be captured, and this is called an ***s-process***. If a neutron approaches very fast, it can be captured but beta decay will also occur, called an ***r-process***. 

- !! The heavier the element, the smaller its quantity is in the universe. The most abundant element is hydrogen, but heavier elements are harder to make and can only be made in specific stars, so their abundance is lower.

When [[Protostar]]s become [[Stars]], they need to begin nuclear fusion and slightly change their composition/[[Spectra]]. This change in the [[HR-diagram]] is denoted by the **zero-age main sequence or ZAMS**. 



