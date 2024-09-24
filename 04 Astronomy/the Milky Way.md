---
tags:
  - galaxy
  - cosmology
  - astronomy
  - physics
  - mathematics
---
Putting all of the pieces of the puzzle together, [[Star formation]], [[Stars]], [[The Interstellar medium]], we can construct an object in the universe called **a galaxy.** We call our home galaxy the Milky Way.

![[globular distribution 1.png|300]]
![[globular distribution 2.png|300]]

We realized that we are around 8.5 kpc away from the centre of the galaxy, due to the spherical distribution of globular clusters in the **halo**, and the open clusters in the **disk**. We also discussed *Population I and II stars*, which have helped us form a better picture of our galaxy. At the centre of the galaxy there is a **bulge**. 

![[schematic milky way.png|200]]

# Round the carousel
---
Since the galaxy is not a rigid structure, we have something called **differential rotation**, where parts closer to the galaxy rotate faster, and parts further away slower. We can model this behavior using [[Calculus]].

Let's assume that each mass clump in the galaxy follows a circular orbit (this is indeed false, but just a starting assumption). Each clump has a distance from the centre $r$, a tangential velocity $v(r)$ and an angular velocity $\Omega(r)$. The mass distribution is:$$M(r) = \int_0^r \rho(r) dV$$ (density and the change in volume). If we combine gravity and [[Circular motion]], we get:$$\frac{GM(r)m}{r^2} = \frac{mv^2(r)}{r}$$, and solving for $M(r)$, we get:
- f $$M(r) = \frac{v^2(r) r}{G}$$ or if we use the angular velocity instead $v = \Omega r$:$$M(r) = \frac{\Omega^2(r)r^3}{G}$$

The function of velocity or rotational velocity is the **rotation curve of the galaxy**, since if we can find the velocity, we find the mass.

But, how do we find the velocity? Using [[The Doppler effect]]. We can track using spectra ([[Radiation mechanisms]]) how the spectral lines shift, based on the position of the gas in the galaxy:
![[galactic doppler shift.png|200]]

Based on our line of sight, different points have different doppler shifts, helping us deduce their velocities. In tracking these, a coordinate system we use is the **galactic coord system** ([[The celestial sphere]], [[Transformations of astronomical coordinates]]), with **galactic latitude $b$** and **longitude $l$**. We also need to define a velocity component to have a reference frame: *local standard of rest, LSR*. 
- eg The **dynamical** definition of this quantity: the origin of the galactic coord system orbits at a distance $R_0$, and it moves with a velocity of $v(R_0) = v_0$, or $\Omega(R_0) = \Omega_0$. 
- eg The **kinematic** definition of LSR: The origin of the coordinate system moves with the average velocity of all the stars in the vicinity of the Sun.

Then, according to this:
- n The Sun is moving at about 20 km/s towards a right ascension of 18h, and a declination of 30º . (In galactic coordinates, this is $l=56º$ , $b=23º$.)

Let's analyze the velocity of a piece of material at some distance $R$ from the centre of the galaxy. 
![[differential rotation scheme.png|200]]
Radial velocity is the one which is along the **line of sight**, or the blue line from the sun, through P. So, the radial velocity is the observed radial velocity minus LSR:$$v_r = v(R)\cos(90º-\theta) - v_0\cos(90º-l)$$
Using the approximation of the first quadrant, we get:$$v_r = v(R)\sin\theta - v_0\sin l = R\Omega(R)\sin\theta - R_0\Omega_0\sin l$$
We can measure $l$, since it is a part of the coordinate system, but $\theta$ is kinda impossible to measure. We need to get rid of it using the law of sines. $$\frac{\sin(180º-\theta)}{R_0} = \frac{\sin l}{R}$$, or:$$\sin \theta = \frac{R_0\sin l}{R}$$
Substituting into the above formula we get:$$v_r = R_0\Omega(R)\sin l - R_0\Omega \sin l$$, so:
- f $$v_r = [\Omega(R) - \Omega_0]\;R_0\sin l$$

Now that we have the radial velocity, we can use it and **transverse** velocity to calculate the actual velocity of galactic material. So:$$v_t = v(R)\sin(90º-\theta) - v_0 \sin(90º-l) = v(R)\cos\theta - v_0\cos l$$
And then we get:$$v_t = R\Omega(R) \cos\theta - R_0\Omega_0 \cos l$$
From the schematic above, we can rewrite $R\cos\theta$, as:$$R\cos\theta = R_0\cos l - d$$
And so:$$v_t = \Omega(R)[R_0\cos l - d] - R_0\Omega_0 \cos l$$
Finally:
- f $$v_t = [\Omega(R) - \Omega_0]\;R_0 \cos l - \Omega(R) d$$

## Now, how do we determine the rotation curve?
---
The rotation curve is determined using measurements of the 21 cm line of hydrogen discussed in [[The Interstellar medium]], and using the radial velocity measurements we could construct a rotation curve:
![[rotation curve.png|300]]
As we can see, the velocity remains constant after the Sun, even though there is supposedly less mass in the farther regions. However, the density remains approximately the same, and the further reaches rotate just as fast as the Sun does. We call the excess matter **dark matter**!

# Distribution of gases
---
In order to understand [[Star formation]] in the galaxy, it is important to see the distribution of clouds of [[The Interstellar medium]], $HI, HII$ clouds, how thick is the disk, does it vary, etc.

### $H I$! and $H_2$ 
---
$H \;I$ doesn't fall off very quickly the larger $R$ becomes, or the further away we move from the centre. When it comes to $H_2$, 
![[H2 distribution.png|300]]
There appears to be a peak at around 6 kpc (5 kpc), called the **molecular ring**. This $H_2$ appears to be concentrated in a large molecular cloud, and not split up into tiny clouds. 

### Thickness of disk
---
- eg We generally express the thickness of the disk by finding the separation between the two points, one above and one below, at which the $HI$ density falls to half of its value in the middle of the plane. This is called the full-width at half-maximum or **FWHM**.

We use the 21 cm line for observations, and we measure the thickness using density. We can see that the thickness gets larger the further we move away, producing **flares**. 
![[thickness of disk 1.png|300]]
We can see the structure of the thickness in here:
![[thickness of disk 2.png|300]]
- n From observations, we noticed that $HII$ regions are younger than $HI$ regions in the galaxy, and that molecular clouds are the youngest.

By using various tracers, we can see how the thickness varies, which means that different materials are found in different places.
![[thickness of disk 3.png|300]]

# Round and round we go
---
How do we map our lovely spirals?

1. We tried to use the fact that spirals or "arms" are not perfect but chunky, so we thought that they were $HII$ regions with $OB$ associations, however optical observation proved to be very difficult, since the interstellar medium is kinda thick. It gives us a **hint at the spiral structure**, but not very detailed.
2. Next, we tried to use **radio observations** of the 21 cm line, and kinematic distances to try and model galaxy structure. This method proved to be quite good, as we could very easily using the rotation curve track spirals beyond our sun
3. Also, another method is to compare our galaxy to other [[Galaxies]], which helps understand our own better.

# Down down we go
----
What about the centre of the galaxy? What's going on there?

Even though we originally thought the centre of the galaxy was the Sun, we now know it isn't but rather in the direction of Sagittarius. But, we didn't really know if there was anything special going on, until we observed other galaxies. 

Optical observations are impossible, so by using radio, infrared, near-infrared, x-ray observations, we managed to get a picture of what is going on.
- There is an *ionized gas bent arc of emission perpendicular to the galactic plane*
	- the structure shows filaments
	- emission in thermal (free-free) radiation and [[Synchrotron radiation]].
- very high temperatures

All of these signs indicate that there must have been **a big explosion in the past**. The [[Supernova]] caused a large gust of star formation, often called **starburst**. 

At the centre, matter is shown to be quite dense, hotter, moving much faster than in regular cloud, and is way more massive. 

> There is a high density to help, but it is inhibited by higher temperatures, velocity dispersions, magnetic pressure, and tidal effects. - Star formation is super rich!

### Black hole sun
---
It was thought of for a long time that at the **centre of the galaxy is a supermassive black hole**, which was only proven with a photograph recently. But, how did we even get some proof of this happening?

Well, if the gravity of a black hole is huge, then *the velocities of stars orbiting it should be huge as well*. Doppler shift is impossible to measure with the accuracy needed for such a short schwartzchild radius, but measuring **proper motion** can be done, and it has been done. Tangential velocities of 1400 km/s were found, and 90 stars have been observed with tangible proper motions. Plotting the orbits of 2 of these stars it was determined that they were Keplerian, and we could actually estimate the mass, which coincides with estimates for black holes. 
