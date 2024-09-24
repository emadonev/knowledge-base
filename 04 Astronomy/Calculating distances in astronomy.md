---
tags:
  - distance
  - astronomy
  - measurement
  - calculation
  - mathematics
---

There are numerous ways to calculate distances in astronomy. The first step is to get a rough scale of the solar system, which isn't that hard. We discovered that the distance from the Earth to the Sun is approximately 150000000 km, which we call **an astronomical unit.**
If we go to a higher scale, we run into **light years**, or the distance light travels in a year (an extremely far distance), so it is a very large scale of distance. But objects are even further away!


## Parallax
---
Another way of calculating distances is using the **parallax method**, where we use the orbit of the Earth to look at the same object using 2 different angles, and then with a little trig we can approximate the distance. We also gain a new measuring unit, the ==parsec==, which is equal to the distance of an object with 1" angular measurement, or 3.26 light years or 206265 AU distance. 

- eg We can calculate the formula for the parallax method using some [[Fundamental trigonometry]]. With a right hand triangle forming using the sun, the star an Earth, we can say that: $$tan \; p = \frac{1 AU}{d}$$Using the fact that p in angular minutes is equal to $2.06*10^5 \; rad$, and the **small angle rule** we can say that:$$\frac{d}{1 AU} = \frac{2.06*10^5}{p(")}$$ $$d(pc) = \frac{1}{p(")}$$ which is a super easy formula!

![[parallax.png]]

A famous telescope used for measuring parallax (which is a tough job since parallax is so difficult to measure because it is very small and the atmosphere distorts the light, and stars are at different distance ranges, etc.) is **Hipparchos satelite**. 
![[hip_obs.gif]]

If we wanted, we could use the diurnal parallax, which is when we measure the parallax of an object on Earth from 2 different sides of the equator, or we wait for 12 hours as it rotates. Then:
- f $$d = \frac{R\sin(\alpha /2)}{\pi_{p, rad}}$$, where $\alpha$ is the separation in longitude from the 2 locations, $\pi$ is the parallax angle and $R$ is the radius of the Earth.

## Solid angle
---
A **solid angle** is how much area on a sphere does an object take up, but in angular terms, since we project its area from a point onto our field of view. The unit of measurement is a *steradian*, and the whole sphere is $4\pi$ steradians. We calculate the solid angle with:$$\Omega = 2\pi[1-\cos\theta]$$
Where $\theta$ is half of the angle of the cone! (we gain this by [[Integration]]) 

How, we know that if we have an object in space and we try to get its radius, we have:$$\tan \alpha = \frac{R}{d} \ce{->} \alpha = \frac{R}{d}$$
 via the *small angle approximation.* From this, we can draw the following line of conclusion:
$$\Omega = \frac{A}{d^2} = \frac{\pi R^2}{d^2}=\pi\alpha^2$$, where $\alpha = R/d$. 

If we want to apply this knowledge to a coordinate system, where we have *azimuth* ($\phi$) and *co-latitude (measured from the north pole)* ($\theta$), where the width of the small rectangular segment **depends on $\sin\theta$,** meaning that: $$\Omega = \int d\phi \sin\theta \;d\theta$$
![[steradians.png]]

From this calculation, we also get that the full angle is $4\pi$. 
## Magnitude scales - spectroscopic parallax
---
Finally, we can use [[Photometric quantities]] and [[Visual magnitudes]] in order to determine distances. We use the photometric quantities of various objects, like [[The Interstellar medium]], [[Variable stars]] (more on that below) or using [[Supernova]]s, or 21 cm hydrogen line measurements from the [[Galaxies]].

An easy method using [[Stars]], [[Luminosity]] and [[Light]] is to use the [[Inverse square law]] to calculate the distance of the energy flux of an object on the surface of the observer.

- !! We can imagine that light travels in spherical spheres towards the earth from a star, and the further away we are, the less the flux is when it reacher earth. So, the part that reaches earth from the total velocity is proportional to the area of the sphere which radiates through all of space and the slice of earth: $$flux = \frac{L}{4\pi d^2}$$, where $d$ is equal to: $$d = \sqrt{\frac{L}{4\pi f}}$$

# Cepheids and RR Lyrae
---
Using the fact that both [[Cepheid variables]] and [[RR Lyrae]] are **standard candles**, we can use their **period-luminosity relationship** to determine how far away they are.
- f Cepheid relationship:$$\log\frac{L_a}{L_s} = 1.15\log P_d + 2.47$$, where $L_a$ is the average luminosity of the cepheid, and $L_s$ is the luminosity of the Sun, and $P_d$ is the period.
# Tully-Fisher relation
---
It has been shown that the **thickness of a 21 cm Hydrogen line** is proportional to the **absolute infrared luminosity.**
![[tully fisher relation.png|300]]
This means that we can measure distances to faraway galaxies using radio measurements of the 21 cm H line. 

![[tully fisher.jpeg|400]]

The galaxy is moving away from us with a radial velocity $v_c$, with its maximum rotational velocity from our sight $v_{rot}$, which is at the line of sight. The radial velocities from Earth are:$$v_1 = v_c - v_{rot}\sin i, \;\;\;v_2 = v_c+v_{rot}\sin i$$
And, the spectrum displacement is:$$\frac{\Delta \lambda_1}{\lambda} = \frac{v_c - v_{rot}\sin i}{c}$$, and the analogous is true for the other velocity. If we subtract one from the other, we get:
- f $$v_{rot} = \frac{c}{\lambda \sin i}(\Delta \lambda_2 - \Delta \lambda_1)$$

Of course, the velocity of the rotation depends on the gravity of the galaxy. The faster a galaxy rotates, the brighter it is. The luminosity-to-mass ratio is thus constant for all galaxies, or $C_{LM} = L/M$. Hence:$$L = C_{LM}\frac{v_{rot}^2R}{G}$$, now, we can also assume that all galaxies have approximately the same surface luminosity, meaning that $C_{LR} = L/R^2$, and putting a constant $C$ for everything: $C = C_{LM}^2/C_{LR}$:
- f $$L = Cv_{rot}^4$$, or the **Tully-fisher relation**

If we use magnitudes, we can rewrite this with luminosity fluxes differing depending on the expression above:
- f $$M_1 - M_2 = -10\log \frac{v_{rot,1}}{v_{rot, 2}}$$
# Hubble's law
---
Hubble's law, as mentioned in [[Galactic clusters]], is great for determining far distances, however it is difficult to determine wether an object is **in the hubble flow or not.** We then use various distance measuring techniques mentioned above to try and determine the actual velocity of an object, as its total radial velocity is:$$v_r = t_0d + \Delta v$$
The biggest problem with distance determination is:
- !! When we look at a distant galaxy, we are seeing it as it was a long time ago. However, we know that galaxies evolve, and as they do that, their luminosity changes. Luminosity calibrations on nearby galaxies might not apply to distant galaxies.

There are many problems with determining the Hubble constant, so our current accepted range of values is from 50 to 100 km/s/Mpc. This is a pretty wide range, but the universe leaves us with no choice. However, a number of recent studies suggest values of 70 km/s/Mpc with an uncertainty of 10 km/s/Mpc.

The distance using Hubble's law is
- f $$v = H_0 d$$


