---
tags:
  - star
  - astronomy
  - binary_system
  - orbits
  - physics
  - mathematics
---
Binary [[Stars]] systems involve 2 stars orbiting each other around a center of motion. 

There are multiple types of binary stars:
1. **Optical binaries** - appear to be binary, but are not really
2. **Visual binaries** - we can differentiate the stars with a telescope, truly binary
3. **Composite spectrum binary** - then looking at spectra, we find 2 stars via the lines present.
4. **Eclipsing binary** - since brightness fluctuates in this [[Variable stars]] ([[Eclipsing variables]]) we can find them.
5. **Astrometric binary** - wobbling stars across the sky - presence of a companion.
6. **Spectroscopic binary** - when spectral lines shift ([[The Doppler effect]]), we can see that another object exists which shifts the lines.

- eg The **Radial velocity** is the velocity of the source in line of sight between the source and the observer:$$v_r = v_s\cos \theta - v_0\cos\theta$$

# Motion in binary star systems
---
![[binary system.jpeg|200]]
![[binary orbit ellipses.png|500]]
The 2 stars orbit in a straight line connecting the 2 stars, meaning that **they have the same period of orbiting**. In this case, $a$ is the distance between them:$$a = r_1+r_2$$
And since they orbit along a straight line around the **centre of motion**:
>$$a_1 = a\frac{M_2}{M_1+M_2}$$ and $$a_2 = a\frac{M_1}{M_1+M_2}$$

#### Kepler's third law with binary stars
Now, we can apply Kepler's third law with binary stars as well! Let's go through this step by step.
First, we know that the 2 stars exhibit a force of gravity, in equal magnitude one upon the other.$$F_{g, 1} = F_{g, 2} = \frac{Gm_1m_2}{(r_1+r_2)^2}$$
Now, in order for them to stay in a, well, circular orbit (I know they don't orbit in circles, but we are oversimplifying everything), and so their centripetal forces have to have a constant magnitude, and since they are orbiting in a straight line, ==their angular velocities must stay the same as well!== $$F_{c, 1} = m_1\omega^2\;r_1, \;\;\;F_{c,2} = m_2\omega^2\;r_2$$
And we also know that the centripetal force and force of gravity are equal in orbits:$$\begin{align} \frac{Gm_1}{(r_1+r_2)^2} = \omega^2\;r_1 \\  \frac{Gm_2}{(r_1+r_2)^2} = \omega^2\;r_2\end{align}$$
Adding the  equations together yields the following result:$$\frac{G(m_1+m_2)}{(r_1+r_2)^2} = \omega^2\;(r_1+r_2)$$
And, knowing the definition of $a$, we can substitute that in our equation. Finally, since $\omega = 2\pi / T$, we get that:
- f $$T^2 = \frac{4\pi^2}{G(m_1+m_2)}a^3$$

Great! Now, it turns out that this equation also works for elliptical orbits, except in this case, $a$ is defined as the sum of the semi-major axes $a_1$ and $a_2$, and not the total distance between them. 

### The Doppler shift and binary stars
---
We can discover binary stars in multiple ways, and one of them is with [[The Doppler effect]], where the shift in wavelengths of light can be seen due to the gravitational tug of each star. 
![[binary star radial motion.png]]
We can see that the tangential velocity is always constant, but the **radial velocity** due to the effect of the Doppler shift is constantly changing due to the angle, $\theta = \omega \;t$. And so, with trig, we get:
- f $$v = v_r \;cos\;\omega t \ce{->} z = \frac{\Delta \lambda}{\lambda_0} = \frac{v_r}{c} cos\;\omega t$$, or with the inclination of the orbit:$$v_r = v\sin i\cos (\omega t)$$

### The mass function
---
If we have 2 stars with certain velocities and periods, we can rewrite their distances from the centre of motion as such:$$r_1 + r_2 = \frac{P}{2\pi}(v_1 + v_2)$$
Using the orbital speed and the fact that the orbit has an inclination, we get:
- f $$\frac{P}{2\pi G}\frac{(v_1+v_2)^3}{\sin^3 i} = m_1 + m_2$$, and this is called the **mass function**.

# A scale for the stars
---
An interesting fact is that we actually use binary stars to determine the masses of [[Stars]] and their spectral types ([[Radiation mechanisms]]). We thus gain the **mass-luminosity relationship**:
- f $$\frac{L}{L_s} = (\frac{M}{M_s})^\alpha$$, where $\alpha = 1.8$ for $M < 0.4 M_s$, $\alpha = 4.0$ for $0.3M_s < M < 3M_s$ and finally $\alpha = 2.8$ for $3M_s < M$.

We can then calculate the radius of the star using luminosity gained from this relationship. When we explore [[Stellar structure]], we'll see why $\alpha$ is roughly 3 for all stars.
# Evolution in close binaries
---
Now, binary stars can be far away, but they can be quite cosy and close, which is what we are going to explore. Tidal forces which distort stars due to strong gravitational forces are at play in close binaries. As the 2 binary stars form together, **their orbits synchronize, they are always one opposite the other**. (like in the beginning with binary motion). 

We can plot the system of binary stars using **effective gravitational potential**, combining the actual gravitational potential with $$\frac{J^2}{2mr^2}$$, which describes the centrifugal force of orbiting. Combining these two, we gain the effective potential, which we can plot for a 2-body system. We gain **equipotential lines**, similar to those on Earth for altitudes, and *no work is done if we move along a equipotential line*. Similarly, 5 points exist where the effective gravitational force is 0: [[Lagrange points]]. Finally, the figure eight which describes the limits of the size and distance of 2 binary stars are called **Roche Lobes**.

![[equipotential gravity binary.png|500]]

# Types of binaries
---
We distinguish 3 types of close binary systems:
### 01 Detached
Every star is within its own Roche lobe, and they never touch and never come closer.

### 02 Semidetached
One of the stars is touching the end of its Roche lobe, while the other is within its own lobe.

### 03 Contact binaries
Both stars are touching at the end of their Roche lobes.


# In a flash of white
---
The first category of close binaries include ones with the presence of a [[White dwarf]]. These little stars are powerful and quite dramatic when they have their duo in tow. 

Let's imagine 2 stars orbiting each other. One of them evolves off the main sequence, slowly transforming into a white dwarf, filling its Roche lobe and transferring that matter into the other companion. When the first star turns into a white dwarf, the second star now starts evolving off the main sequence, filling its Roche lobe. Now the **second mass transfer begins, and things get interesting.**

As the mass falls towards the white dwarf, it forms an **accretion disk**, since material can fall parallel to the axis of rotation, but not perpendicular to that axis. 

During this process, potential energy decreases, and kinetic energy increases, **but not by the same amount.** The [[Virial theorem]] tells us that around half of the decrease in potential energy becomes kinetic energy, and the rest is radiated away. However, the kinetic energy that does get in, doesn't produce radiation in itself, but the *accretion disk heats up and emits heat.*

We can actually estimate the energy available from the change in potential energy. $$L = \frac{dM}{dt}(\frac{GM}{r_2} - \frac{GM}{r_1})$$
Where $r_2$ and $r_1$ are the ending and starting points of the material, respectively. The final form is:
- f $$L \approx GM\frac{dM}{dt}(\frac{1}{r_2} - \frac{1}{r_1})$$

As mass falls in, a few scenarios can occur. These are [[Dwarf Novas]], [[Novas]] and [[Supernova]]s. 

# When neutrons get involved
---
There is a possibility that a binary system exists with a [[Neutron stars]] and a normal star, however this seems super unlikely. How is it possible that a neutron star formed? 
- n The issue is that for a system to stay bound (E = 0), the supernova explosion in order to create a neutron star would have to remove 50% of the mass of the more massive star, so the system would lose a lot. If the system cannot respond quickly enough to this huge change, **we get runaway stars**. The mass we are left with is:$$m = m_1[\frac{1}{2 + m_2/m_1}]$$, where $m$ is the remaining mass of the bigger star, $m_2$ and $m_1$ are the starting masses.

Nevertheless, scientists have figured out possible ways for this to still work.
1. There are some combinations of initial conditions which allow a system to stay bound after a supernova explosion.
2. Before exploding, some mass was transferred to the smaller star, enabling the system to stay bound.
3. If the other companion is originally a white dwarf, some matter transform can reach the Chandrasekhar limit and turn it into a neutron star.

### X-man
---
There is a special binary system with neutron stars where a neutron star and a normal star, but mass transfer occurs from the normal one to the neutron star. *This mass causes irregular bursts of X-ray emission when it is heated and falls to the surface*. A famous source is **Her X-1**, and its light curve looks like so:
![[Her X-1.png|400]]

This system can later transform into a system with **2 compact objects**, as the mass transfer becomes so heavy that the X-rays are blocked by the falling material.

In this system, we now have [[Pulsars]], and it can explain millisecond ones as well. As mass is transferred, an **accretion disk forms**, and due to the conservation of [[Angular momentum]], **the star rotates faster**, conserving its period.

### Radiogirls
---
Other than X-ray phenomenons, scientists Joseph Taylor and Russel Hulse discovered a pulsar with a changing period ([[The Doppler effect]]), so they concluded it was a binary. They discovered **gravitational radiation**, where gravitational radiation carries away energy, so the total energy of the orbit is decreasing, the period should become longer. They won the Nobel prize for this discovery!

# Black hole sun
---
If a black hole comes in tow with another star in a binary system, using the doppler effect as in spectroscopic binaries, knowing the mass of the visible star, the inclination of the orbit and the shortness of emission of X-rays as they hit the event horizon of the black hole, **we can find these black holes without observing them**. This was true for the system *Cyg X-1* 

