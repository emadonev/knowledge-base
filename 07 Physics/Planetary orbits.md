---
tags:
  - planet
  - solary_system
  - orbits
  - star
  - gravity
  - astronomy
  - physics
---

![[orbital elements.png|400]]

An orbit of a planet consists of several parameters most of which are constant:
- **inclination**, or $i$ - how much is the orbital path of the planet inclined against the **ecliptic** ([[Motion of the Sun]])
- **semi-major axis** or $a$ - half of the length of the ellipse ([[Kepler's first law - the law of ellipses]])
- **eccentricity** or $e$ - how much is the ellipse "elliptical"
- **longitude of the ascending node** or $\Omega$ - the point at which the planet crosses the ecliptic from south to north, measured clockwise from the vernal equinox
- **argument of the perihelion** or $\omega$ - direction of the perihelion, measured from the ascending node in the direction of motion
- **time of the perihelion** or $\tau$ 

We have 2 expressions including the orbital elements:
- f $$\Pi = \Omega + \omega$$, where $\Pi$ is longitude of perihelion.

- f $$L = M + \omega + \Omega$$, where $L$ is the mean longitude and $M$ is the mean anomaly!

# Determining position in orbit
---
In our discussion of [[Kepler's laws]] and other phenomena, we haven't touched up on the fact of **tracking a planet down** on its orbit around [[The Sun]]. We need to convert our radius vector into a [[Functions]] of time! 
![[position of planet.png|400]]
> *In the image, $a$ is the semi-major axis, $b$ is the semi-minor axis, the distance from the centre of the ellipse and the sun is $c$, or $ae$, the angle between the sun and the radius vector $\vec{r}$ is $f$. Finally, we have the elliptical path and the position of the planet at point $P$. But, if we were to extend the semi-major axis into **a circle** to form an alternative orbit, where **the planet would supposedly be at point $P'$** with a vertical drawn downwards to point $Q$. $E$ is defined as the **eccentric anomaly**, and is the angle from the centre of the ellipse to the "position" of the planet on the circle.*  

1. How can we express $\vec{r}$?
Since $\vec{r}$ is a vector, we need to add 2 vector quantities together, which we do by multiplying scalars by **unit vectors, $\vec{i}, \vec{j}$**. 
$$\vec{r} = a(\cos E - e)\vec{i} + b\sin E \;\vec{j}$$
If we want to find the actual distance value, we need to square the values since **we have a right triangle, and hence the pythagorean theorem.**
$$r^2 = a^2(\cos E - e)^2 + b^2\sin^2 E$$$$r^2 = a^2(\cos E-e)^2 + a^2(1-e^2)\sin^2 E$$
$$r^2 = a^2[(\cos E - e)^2 + (1-e^2)(1-\cos^2 E)]$$
$$r^2 = a^2[\cos^2 E - 2e\cos E + e^2 + 1 - \cos^2 E - e^2 + e\cos^2 E]$$
$$r^2 = a^2[1 - 2e\cos E + e\cos^2 E]$$
- f $$r = a(1 - e\cos E)$$

2. How to find $E$ as a function of time?
Using [[Kepler's second law - the law of areas]], we can create 2 equivalent statements for area using geometry and basic math.

The first equation, is that the area of an ellipse (from [[Kepler's first law - the law of ellipses]]), is $ab\pi$. A fraction of that area after perihelion passes constantly, so:$$A = ab\pi \frac{t-\tau}{P}$$, where $t - \tau$ is the time passed since perihelion and $P$ is the total period. 

![[anomalies of planets area.png|400]]

For the second equation, we need to use [[Geometry]]. We know that the area which the planet passed is the shaded one in the picture, and we can figure out what that area is. Since **an ellipse is an affine transformation of a circle,** any area of a circle **can be multiplied by $b/a$ to get scaled to ellipse sizes.**
$$A = \frac{b}{a}(A_{CP'X} - A_{SP'C})$$
$$A = \frac{b}{a}(\frac{\pi a^2 E}{2\pi} - \frac{1}{2}a\sin E \;ae)$$
$$A = \frac{b}{a}[\frac{1}{2}(a^2E - a^2 e\sin E)]$$
- f $$A = \frac{1}{2}ab(E - e\sin E)$$

If we equate the two:
$$ab\pi \frac{t-\tau}{P} = \frac{1}{2}ab(E - e\sin E)$$
- f $$M = E - e\sin E$$, where $M$ is equal to:$$M = \frac{2\pi (t-\tau)}{P}$$ and is also called **the mean anomaly**.


Also, if we want to know the angle passed by the planet in terms of the eccentric anomaly:
- f $$\cos f = \frac{\cos E - e}{1 - e \cos E}$$ and $$\sin f = \sqrt{1-e^2}\frac{\sin E}{1 - e\cos E}$$

# Planet's path - but with coordinates
---
Now that we can track a planet's movement across its orbit, how do we translate this to [[The celestial sphere]] and [[Transformations of astronomical coordinates]]? 

![[coordinates of planet orbit.png|400]]

We can of course use **ecliptic coordinates** along with the elements of a planetary orbit to determine a planet's course. The point at which the planet comes above the ecliptic is where we begin our spherical triangle ([[Spherical trigonometry]]). We see it has traveled some angle, $f$ and also the argument of perihelion $\omega$. At the bottom, it has a certain ecliptic longitude (measured from the vernal equinox to the point where the inclination begins) and it traveled an extra longitude of the ascending node, and we have its **ecliptic latitude.** Finally, one angle is inclination, and the other a right angle. We can apply the sine formula:
$$\frac{\sin \beta}{\sin i} = \frac{\sin (\omega + f)}{\sin \pi/2}$$, where $\pi/2$ is in radians for 90º. Since this is equal to 1, we get:
- f $$\sin \beta = \sin i \sin(\omega + f)$$

And for the ecliptic longitude, we have via the sine-cosine formula:
$$\cos(\pi/2)\sin\beta = -\cos i \sin(\omega + f)\cos (\lambda - \Omega) + \cos(\omega + f)\sin(\lambda - \Omega)$$
And finally:
- f $$\tan (\lambda - \Omega) = \cos i \tan (\omega + f)$$

How do we take these coordinates (the ecliptic ones) and transform them back into equatorial coordinates? 

>  Using rectangular coordinates and relative position of Earth:

- f $$x = r\cos\lambda\cos\beta$$$$y = r\sin\lambda\cos\beta$$$$z = r \sin\beta$$

We now turn these into equatorial ecliptic coordinates:
- f $$X_P = x$$$$Y_P = y\cos \epsilon - z \sin \epsilon$$$$Z_P = y\sin \epsilon + z\cos \epsilon$$

 (note: all of this could have been done with spherical trig, but this is a tad easier actually)

Now, to get the actual position of the planet **with respect to the Earth**, we subtract Earth's values for X, Y and Z from the planet's values. Finally:
- f $$\alpha = \arctan (Y_0/X_0)$$$$\delta = \arctan \frac{Z_0}{\sqrt{X_0^2 + Y_0^2}}$$

# In relation to the Earth
---
While the planets move around the Sun in their orbits, we from Earth have a complicated viewpoint of how they move. Partly because of the Earth's motion around the Sun, things get a bit distorted. Sometimes planets travel in **direct motion**, other times in **retrograde**.

We distinguish 2 types of planets: **inferior and superior**. Inferior are the ones before Earth, and superior the ones after. All of the planetary positions are denoted in the image below:
![[planetary positions.jpeg|300]]
#### Inferior planets
They are Mercury and Venus, and they move really close to the Sun, however never exceeding their **maximum elongation.** The angle E2S (the sun is point S) is a right angle, hence the maximum elongation can never exceed:
- f $$\epsilon_{max} = \frac{d}{d_s}$$, where $d$ is the distance from the planet to the Sun, and $d_s$ Earth-Sun distance.

- n For Venus, the values range from 45º to 48º, and for Mercury from 18º to 28º. 

The motion of the inferior planets is described as such:
1. At point of maximum eastern elongation, it is visible shortly after sunset.
2. The Sun sets earlier than the planet, making it visible during twilight. 
3. At point of inferior conjunction it is directly in line with the Sun, and a **transit** might occur. 
4. It then moves retrogradely to the west, and is visible just before dawn.
5. It appears to be stationary at its western maximum point.
6. It then reverses motion, faster and faster reaching the Sun.
7. At upper conjunction it disappears behind the Sun.
8. The cycle continues.

#### Superior planets
These are Mars, Jupiter, Saturn, Uranus and Neptune, and they are more free to move, and can reach a maximum elongation of any value. Here is the motion of these planets:
1. In conjunction they are barely visible as they rise and set with the Sun.
2. They move until the point of eastern quadrature and stay there.
3. it then moves away, faster and faster until opposition, when it is best seen.
4. it moves again until western quadrature, and appears stationary. 
5. The cycle repeats.


## Periods of orbiting
---
We differentiate 2 different kinds of periods, just like in [[Time systems]]. We have the **synodic period** - interval of time between 2 successive conjunctions/oppositions of a planet. We also have the **sidereal period** or the interval of one complete orbit around the Sun. 

Looking at the angular velocities of the planets, the angular velocity of inferior planets is larger than the Earth, hence:$$\omega_{diff} = \omega_{planet} - \omega_e$$

For superior planets, the Earth's angular velocity is bigger, and so:$$\omega_r = \omega_e - \omega_p$$
Since the numerator of each fraction is the same, we get the final equations:

- f For **inferior planets**: $$\frac{1}{S} = \frac{1}{T} - \frac{1}{A}$$, and for the **superior planets**: $$\frac{1}{S} = \frac{1}{A} - \frac{1}{T}$$

### Retrograde motion
---
The reason that we have the heliocentric model was because of the difficulty of explaining **retrograde motion in a geocentric model**. This is the phenomenon of planets moving suddenly eastward across the sky, and then back west. It could be simply explained if we orbited [[The Sun]], and because of the differing [[Velocity]]es of orbit due to [[Kepler's third law - the law of proportionality]], we could explain this "backwards" motion.
![[retrograde_mars_eartjPOV.png|400]]



### Phase of a planet
---
An interesting property of the planets and [[Light]] is the **phase of a planet**, which we can observe in eg. [[Venus]] and the [[Moon]]. And we can use some simple geometry and [[Fundamental trigonometry]] to get to the answer. 
![[phase of planet.png|300]]
From the position of [[The Sun]], the light part of the photo is visible, but from the [[Earth]]'s perspective, only above line CD is everything visible, meaning that PBD is going to be dark - the phase of the planet. 

So, the phase of a planet is really:$$phase = \frac{CF}{CD} = \frac{CP + PF}{CD}$$ and using some trigonometry, 
- !! $$phase = \frac{CP + cos\;\phi\;CP}{2CP} = \frac{1}{2}(1+cos\;\phi)$$

--- 
However, we want to find the phase of the planet depending on its position around the Sun. For that, we need the angle theta in the drawing above to see what's what. Using the sine formula:$$\frac{SE}{sin\;\phi} = \frac{SP}{sin\;(180-(\theta+\phi))}$$ So we can get that:$$SP\;sin\;\phi = SE\;sin\;(\theta+\phi)$$ where we can use the fact that the tangent is equal to the sine over cosine, we can get:$$tan\;\phi = \frac{SP\;sin\;\theta}{SE - SP\;cos\;\theta}$$ and we can calculate theta by:$$\theta = 360 \frac{t}{S}$$, where $t$ is the time which has passed since the beginning of the cycle, an $S$ is the *synodic period*

