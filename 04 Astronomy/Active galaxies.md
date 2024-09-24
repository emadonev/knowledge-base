---
tags:
  - galaxy
  - astronomy
  - physics
  - mathematics
---
We have covered [[Galaxies]], but many types of galaxies have suspicious activity in their nuclei, and we call these ==active galaxies==. Their nuclei are called **active galactic nuclei**. 

# Starburst!
---
These galaxies are considered active since their existence is pretty short term - they have **massive amounts of [[Star formation]]**, which lights up the galaxy brightly. These stars are quite massive and big, due to radio emissions signaling supernova remnants near the centre of the galaxy. As the stars use up the molecular clouds ([[The Interstellar medium]]), there can be less star formation, making this phenomenon a passing one. There are multiple theories to suggest as to *why are the molecular clouds unstable in these galaxies so they have super efficient star formation?* The answer is not yet known, but it is theorized that through galaxy interactions material has been dumped into the other galaxy.

# Radio galaxies
---
These galaxies are characteristic of the fact that they emit a really large, around 1000000 times more radio waves than regular galaxies. They have huge jets on both sides of the galaxy, which aren't very dense or magnetically active, but they are very large. We are trying to currently model these types of galaxies, with their general structure like so:
![[general schematic radio galaxies.png]]
We then look in closer to the nucleus, where we have a confining disk which creates parallel jets on either side. Although sometimes there is only one jet in the galaxy, but 2 lobes still remain. 
![[radio galaxy 2.png]]
The closer we get, we approach the black hole and its accretion disk, where we theorize is the source of radiation.
![[radio galaxy 3.png]]

Nuclear reactions within a star could never achieve such high energies required to emit that much radio emission. However, matter falling into a black hole definitely can. We can estimate the energy gained when we put a particle traveling to the Schwarzschild radius, until of course it reaches it, since afterwards we don't have any more energy. So:$$E = \frac{GMm}{R_s}$$, and substituting for $R_s$, we get:
- f $$E = \frac{1}{2}mc^2$$ We can calculate the luminosity using the change in energy over time, as mass changes over time:$$L = \frac{1}{2}(dm/dt)c^2$$
(In reality, 40% of the energy can be used, due to the matter taking a spiraling route to the black hole.)

For radio galaxies to get enough radiation to be so powerful, black holes would need to be around a billion times the mass of [[The Sun]]. 

## Superluminous problems
---
There is a slight issue with radio galaxies though. The galaxies seem to have some components which are moving faster than the speed of light, which is of course impossible. However, it all depends on the frame of reference. The body is not actually moving at that speed, it only appears to do so.

![[superluminous.png]]
We can rewrite x and y as components of r, and we know that the time it takes for an object to move the distance r is $t = r/v$. But, we can see that $x$ is shorter than $r$, hence the time should be shorter by $$t_a = t - x/c$$, or if we substitute:$$t = r/v - (r/c)\cos\theta$$
And so, $v_a$ is:$$v_a = \frac{y}{t}$$ or 
- f $$v_a = \frac{v\sin\theta}{1-(v/c)\cos\theta}$$

If we differentiate this equation (or apply Lorentz transformation), we get that:$$\cos \theta = v/c$$
and that $$\frac{v_a}{v} = \frac{1}{\sqrt{1-(v/c)^2}}$$

# Seyfert galaxies
---
These galaxies have huge nuclei which shine super bright (in the optical spectrum). They totally dominate the total light of the galaxy. We actually have 2 different types of Seyfert galaxies, one with **forbidden lines** that are broad, and ones where they are narrow. The narrow ones are called type I, and the other type II. Type I have non-thermal radiation, weak radio source, strong X ray emission. Type II have thermal radiation, moderate radio source.

# Quasars
---
These super mysterious stellar objects look like stars, but have the absolute magnitude of 26, which is around $10^{12}$ more brighter than the Sun!!! This is an insane amount of radiation and it actually radiates more in the radio spectrum than in the visible. We noticed the extreme distance modulus due to the enormous redshift in the spectrum of the QSR or **quasar** (quasi-stellar radio source), which would mean that the object was super far away and extremely bright. Another type of object, **quasi-stellar object** is a quasar with no radio emission.

Quasars have very high ultraviolet emission, so looking for objects with high ultraviolet emission, we should be able to find more quasars. Since they have such a high redshift, they actually give us a view into what the universe looked like waaay before us. Another interesting fact is that in their spectra, the Lyman lines are very visible, the most excitable part of hydrogen lines. This means that the temperature is low, and mostly coming from **material around the object itself**. 

Quasars bring about an interesting problem - **the energy-redshift problem**. This means that we can either explain why there is so much energy in quasars, or redefine how redshift works for very high values, or where the redshift is coming from.

(Gravitational redshift has the following formula: $$\frac{\Delta \lambda}{\lambda} = \frac{GM}{rc^2}$$, where $r$ is the radius of the object with the gravitational redshift.)

As of right now, the problem isn't of that much concern, as with the discovery of high energy processes in astronomy, we have assurance that there is some process which explains what is happening.

- n An interesting thing happens around strong gravitational fields - they bend light. And if they bend light, they act like a lens, making an image better and brighter. We call this process **gravitational lensing**. 

In the case of a quasar, a galaxy is in the way between an observer and quasar, and its strong gravitational influence makes the light bend slightly downward/upwards, forming an **einstein ring** of images around the galaxy.  The equation for the angle of light deflection from gravitational lensing is:$$\theta = \frac{4GM}{bc^2}$$, where $b$ is the distance from the object to the beam of light.

> When we look at the various examples of AGNs, we see many features in common: large energy output, rapid variability meaning small sources of energy, and jets. The explanations involve mas- sive black holes fed by material passing through an accretion disk. There are also uniform out- flows that can be collimated into narrow jets. This leads us to ask whether radio galaxies, Seyferts and quasars are different manifestations of the same basic phenomenon.

While back then we weren't sure if these objects were black holes, like in the centre of our galaxy or in M87, but now with pictures, we can confirm that these are indeed black holes. 
