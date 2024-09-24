---
tags:
  - star
  - astronomy
  - cluster
  - observation
  - physics
  - mathematics
---
Most [[Stars]] in [[the Milky Way]] are grouped together into a **cluster.** We have 2 types: ***galactic or open clusters*** and ***globular clusters.*** 
- eg **Open clusters** are confined to the galactic disk and have a more dispersed shape (like the Pleiades) and diffuse gas, they have less than 1000 stars and are less than 10 pc across.
- eg **Globular clusters** are found in the galactic halo around the galaxy, and they have many more stars, around 1000000, confined to a compact spherical appearance. They are also much bigger, 20-100 pc across. 

# Run, cluster, run
---
We use **proper motion** and **radial velocity** to calculate the distance of a cluster. ([[Perturbation phenomena]]) We use the angular line of sight to calculate both velocities with the help of [[The Doppler effect]]. However, as the cluster moves away from us, the line of sight changes as well. After a long while, the cluster **converges**, and we don't have a feeling it is moving anymore. This is the proper $A$ to take as our angle of line of sight. 
![[moving clusters.png|300]]

![[convergetnt point.png|300]]

# Dynamics of clusters
---
Stars constantly move around in clusters, moving around and disrupting the gravitational balance between objects. All of the stars form together a **gravitationally bound cluster**, and when a cluster reaches an equilibrium of energy we say it is **dynamically relaxed.** The kinetic and potential energies are related by the [[Virial theorem]], which is extremely important! This means that the energy of the system is:$$E = \frac{1}{2}⟨U⟩$$

In the cluster, each star has kinetic energy or:$$K = \frac{1}{2}m \sum_{i = 1}^N \vec{v_i}^2$$, and the total mass of the cluster is $mN$, so:
$$K = \frac{1}{2}(mN) \frac{1}{N} \sum_{i = 1}^N \vec{v_i}^2$$

And we now have the average speed per star, or:$$K = \frac{1}{2}M⟨v^2⟩$$
Combining this with the [[Potential energy]] of gravity and the virial theorem, we get:$$M⟨v^2⟩ = \frac{3GM^2}{5R}$$, we get the **root mean square velocity or rms velocity** of internal motions in the cluster (if we take the square root).
- f $$⟨v^2⟩ = \frac{3GM}{5R}$$

Relating this to **escape velocity** ([[Energy in orbits]]) we can say that the **escape velocity is greater than the rms velocity**, in a gravitationally bound system.

### Chillaxing
---
Let's say that a star really wants to escape, and it has the escape speed to go out of the cluster. In doing so, it disrupts the **velocity distribution** of the cluster, hence *the cluster takes some time to return to equilibrium of velocities*. This is called the ***relaxation time of a cluster.*** 

We can quantify this by tracking the motion of a star where it has to pass through some cylinder radius $r$, distance $v\;t_{rel}$, where $v$ is the velocity of the star. The volume is:$$V = \pi r^2 v\;t_{rel}$$This cylinder defines $r$ such that the potential energy of the star is equal in magnitude to the kinetic energy of our star which is "colliding" with it. So:$$\frac{Gm^2}{r} = \frac{mv^2}{2}$$
In this volume, there are an $n$ amount of stars per volume, so total amount of stars is $nV$. If the cylinder is designed for the time between 1 collision, then:$$t_{rel} = \frac{1}{n\pi r^2 v}$$, and substituting for $r$ we get:$$t_{rel} = \frac{v^3}{4\pi G^2 m^2n}$$
Now, let's rewind and redefine $n$. It is the total number of stars divided by the volume:$$n = \frac{N}{V}$$, and by redefining $N$ as $M/m$ (total mass divided by individual mass) and plug in the volume, we get:$$n = \frac{3M}{4\pi m R^3}$$
Putting this back into the original formula:$$t_{rel} = \frac{v^3R^3}{3G^2mM}$$
We can now use clever mathematical loopholes to rewrite this. By using $N, m, M$ interchangeably and rewriting $v^3R^3$ as $v^4R^2 \;\frac{R}{v}$, we can gain the following:$$t_{rel} = \frac{(R/v) \;R^2v^4\;(M/m)}{G^2M^2}$$
Now using the **virial theorem** and the **rms velocity (squared)** we can see that lots of terms cancel out, leaving:
- f $$t_{rel} = \frac{3}{25}(R/v)(M/m) = \frac{3}{25}(RN/v)$$
We ignore the numerical factor as **this is just an estimate**, leaving:
- f $$t_{rel} = \frac{RN}{v}$$

A timeframe around 100 times greater than the relaxation time is the **evaporation time**, or the time it takes *many stars to leave the cluster*. 

## Virial masses
---
Combining the kinetic energy and potential energy of a cluster with the virial theorem, we gain the **virial mass**, which is:
- f $$M = \frac{5⟨v^2⟩R}{3G}$$

- !! It is important to note **which motion we are talking about**. The cluster has its own motion around its centre of mass, shared by every star. Each star has its own individual motion, tugging along the cluster. The vector sum is what we observe. So, the quantity $⟨v^2⟩$ **is the average of the square of the star velocities with respect to the centre of mass of the cluster.** 

We can measure the individual velocity of a star using [[The Doppler effect]]. But, this is only the radial velocity, not the true velocity. However, we might just be able to relate these without having the transverse velocity.

---

By plotting the velocity in a [[Cartesian coordinate system]] with x, y and z coordinates, we get the velocity as components:$$v = v_x\;\vec{x} + v_y\;\vec{y} + v_z\;\vec{z}$$
The x, y and z [[Vectors]] are called **unit vectors** which apply the direction part to the magnitudes of $v_x, v_y, v_z$. 

The square of a vector is the magnitude of that vector, hence:$$v^2 = v_x^2 + v_y^2 + v_z^2$$, or if we time-average it:$$⟨v^2⟩ = ⟨v_x^2⟩ + ⟨v_y^2⟩ + ⟨v_z^2⟩$$
Now, we can use a neat little trick.
- n If the **motions of the stars are *random***, then that means that the **average velocities *are all equal***. $$⟨v_x^2⟩ = ⟨v_y^2⟩ = ⟨v_z^2⟩$$

And so:$$⟨v^2⟩ = 3⟨v_x^2⟩$$, and the $x$ direction is the one **corresponding to the line of sight** which means that it is the radial velocity. Putting this into the formula for virial mass, we gain:
- f $$M = \frac{5⟨v_r^2⟩R}{G}$$

- !! NOTE: all of these formulas apply for **spherical, uniformly dense, gravitationally bound** clusters. 

# The HR of clusters
---
Using the ***HR diagram***, we can look at the structure and variability of stars in a cluster. The amount of stars in each phase of the HR diagram can tell us the age of a cluster. Hotter massive stars evolve faster, leave the main sequence sooner. Each graph has a **turn-off point**, where no more hot stars are seen on the main sequence, the graph starts to deviate towards the right.

> We can tell the relative age of two clusters by comparing their turn-off points.

From this analysis we concluded that **globular clusters are much older than open ones**, due to the length of their main sequence and strength of turn-off point. 

As for the stars themselves, the **particular abundance of *metals*** in a star tells us in which ==population== it is. Stars with high metallicity are called *Population I*, while low-metallicity stars are *Population II*. The Population I are younger and therefore have more metals which the Population II produced, since in the beginning the galaxy was made of mostly hydrogen and helium. 

Globular clusters are older and dust-less, so all stars have already formed and contributed to the galaxy, while open clusters are diffuse and full of material for production of new stars. 