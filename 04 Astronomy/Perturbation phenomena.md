---
tags:
  - observation
  - astronomy
  - celestial_sphere
  - coordinate_systems
  - trigonometry
  - mathematics
  - math
  - light
---
Understanding [[The celestial sphere]] and how to do [[Transformations of astronomical coordinates]], it is important to note that, as far and as distant as objects in space might be, *there exist effects which change or perturb our understanding* of the positions of these objects. 

# Precession & nutation
---

![[precession.jpeg|300]]

The first of such effects is ==precession==. Due to gravity, [[The Sun]] and the [[Moon]] (as well as other planets but miserably less) have an effect and pull upon the Earth. It responds by rotating its axis of rotation in that direction, effectively tracing out a cone with a period of around 26000 or 25765 years. 

- n This has the effect of moving every object's ecliptic longitude by 50" every year, as well as the RA-dec coordinates, so we need to update the coordinates **every century**, giving rise to different *epochs* of measurement - we are currently in the epoch J2000.0, since January 1st, 2000. 

By doing some fancy [[Calculus]], which we are not going to get into here, we can say that the change in declination and rectascension based on ecliptic longitude (which is the thing that is changing by 50" every year), is:
- f $$\frac{d\alpha}{d\lambda} = \sin \epsilon\sin\alpha\tan\delta + \cos\epsilon$$$$\frac{d\delta}{d\lambda} = \sin\epsilon\cos\alpha$$

==Nutation== is the oscillatory motion of the rotation axis as it moves along its precession cone. It is mostly due to the gravitational pull of the Moon and the direction of [[Angular momentum]]. Its period is 18.6 years, and has an extremely small amplitude of 9.2"

# Parallax
---
Other than just being used as a way of [[Calculating distances in astronomy]], is a form of perturbation. The type of parallax causing problems here on Earth is the **diurnal parallax**, which happens when we change our direction *due to the rotation of the Earth.* It also matters if the parallax in question is measured from the observer or the center of the Earth. 
- n The Moon's parallax is 57', and the Sun's is around 8.79".

# Aberration
---
![[aberration telescope.png]]
This type of aberration forms due to Earth's rotation or revolution, and when its light becomes distorted by it. It takes a certain time, $t = l/c$, for light to travel the length of the telescope. If it is moving at a certain velocity $v$, it has a component $v\sin\theta$ which is **perpendicular to light travelling**. It will be displaced by $x = tv\sin\theta = l(v/c)\sin\theta$. The angle is then$$A = \frac{v}{c}sin\;\theta$$, where v is either the speed of rotation or revolution. However, for normal intents and purposes we can assume that *since light is so far away, it comes in towards us at parallel lines*, making the following statement true:$$tg\;\theta = \frac{c}{v}$$, for the bottom angle theta, or for the top angle theta (90º-$\theta$) it is the opposite (v/c).

# Refraction
---
![[astronomical ref.png]]
[[Light]] is known to change its **angle of incidence** when passing from one material through another due to the **different refraction indexes of materials**. 
- !! The first law of refraction: *The incident ray, the normal and the refracted ray are coplanar.* ![[first law ref.png]]

- !! The second law of refraction:$$\frac{sin \; i}{sin \; r} = \frac{n_i}{n_r}$$, where $i$ is the incident angle, $r$ is the exiting angle and $n$ is the **index of refraction.**  (derivation includes derivatives, so come back to another time)

We can see that through the atmosphere of the [[Earth]], light refracts many many times, and we can make a good approximation of the real zenith distance of a star based on previous knowledge. $z$ is the true zenith distance, since X is parallel to the starting AB ray of light. $\xi$ is the apparent zenith distance. Using Snell's law, we can say that: $$n_0\;sin \; z = n \; sin \; \xi$$
And also $R = z - \xi$ be the angle of refraction, since that is the difference between the true and apparent value. And $n = 1$, since that is the index of refraction of light in a vacuum. So, we can measure R  to get the true zenith distance:$$z = R+ \xi$$
$$\begin{align} 
n_0\;sin\;\xi = sin(R+\xi) \\
n_0\;sin\;\xi = sin\;\xi\;cos\;R + sin\;R\;cos\;\xi \\
n_0\;sin\;\xi = sin\;\xi +R\;cos\;\xi \\
sin\;\xi(n_0 - 1) = R\;cos\;\xi \\
R = \frac{sin\;\xi(n_0-1)}{cos\;\xi} \\
R = tg\;\xi(n_0-1) \\
R" = 206265(n_0-1)\;tg\;\xi \\
\end{align}$$
And we finally reach the final form:
- !! $$R" = K\;tg\;\xi, \;K = 60.4"$$

At the horizon, this is equal to 35', which is the horizontal atmospheric refraction which allows us to see a little bit below the horizon.

- f $$\sin(\alpha + \beta) = \cos\alpha\sin\beta + \sin\alpha\cos\beta$$
- f $$\cos(\alpha+\beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$$

# Atmospheric extinction
---
The atmosphere, other than refraction, presents a very serious **extinction problem**, which is a problem for [[Photometric quantities]]. The observed apparent magnitude depends on our location on Earth and the atmosphere. 
![[atmospheric extinction.png|350x300]]
- f $$m = m_0 + k X$$, where $X = \sec z$, and z is the zenith distance. $k$ is the extinction coefficient. 

# Visibility of horizon
---
What if we are observing from the horizon? The Earth is not a flat sphere, so there are mountains and such which make us able to see more than we should, plus we have **atmospheric refraction at the horizon, 35' to be exact.** (At least for 0º apparent altitude). 
![[horizontal ref.png]]
Our first step is to calculate the angle of our dip, meaning how below we can see below our vantage point at O. We can see that the actual altitude is actually:$$a = a' - \theta$$, where $a'$ is the observed altitude. Using the fact that TCO = $\theta$, we can say that:
- !! $$cos \;\theta = \frac{R}{R+h}$$

So, we can observe: $$\epsilon = \theta + 35'$$
So for circumpolar stars: $$\delta > 90 - (\phi + \epsilon)$$

# Proper motion
---
![[motion across sky.jpeg|200]]

A star is moving through space, all the time. It has a certain velocity, $v$, which we can build from our point of view on Earth by vector addition of 2 components: **tangential velocity and radial velocity**. The *real* motion of the star is called proper motion, and it changes the shapes of constellations over time. 

***Radial velocity*** is the velocity heading directly away from our point of view, and we can calculate it using [[The Doppler effect]]:$$v_r = cz => (relativity)\;\frac{(1+z)^2 - 1}{(1+z)^2 + 1}c$$
***Tangential velocity*** is a tad harder to calculate, but it is very simple in theory. It is the change in the position of the star *relative to Earth*, so we track this type of velocity with **angular speeds and the changes in coordinates.** We can divide transversal velocity into 2 more components, the change in RA and the change in dec:
![[proper motion sphere.jpeg|400]]

One vector, $u_{\alpha}$ is the ***angular velocity*** of an object changing its position in rectascencion, multiplied by the cosine of declination since it travels along the parallel of declination, and its distance from the centre is $cos\;\delta$. The second vector is the angular velocity of the change in declination, $u_{\delta}$. Using the Pythagorean theorem, we get the value for **proper motion** of our star:$$\mu = \sqrt{u_{\alpha}^2cos^2\delta + u_{\delta}^2}$$
- eg The coefficient cos δ is used to correct the scale of right ascension: hour circles (the great circles with α = constant) approach each other towards the poles, so the coordinate difference must be multiplied by cos δ to obtain the true angular separation.

As we know from elementary physics, the tangential speed is the angular speed times the distance:$$v_t = u\;r$$, which means that the **proper motion, or the change in coordinates over a certain time period,** is equal to
- f $$\mu = \frac{v_t}{r}$$

What about the units? If we have:
- parallax $p$ in **arcsec**
- distance $d$ in **parsecs**
- proper motion $\mu$ in **arcsec/year**
then:
> $$v_t = \frac{\mu}{p}\; au/yr = 4.7\frac{\mu}{p}\;km/s = 4.7\mu\;d\;km/s$$

---

Let's say we have a star moving along the celestial sphere.
![[proper motion sphere.png|300]]
It moved from point A to point B. It changed its coordinates $\alpha, \delta$. If we use the **law of sines** from [[Spherical trigonometry]], then: $$sin\;\Delta \theta\;sin\;\phi = sin\;\Delta \alpha\;cos(\delta + \Delta \delta)$$, if we use the small angle approximation and neglecting higher order trig terms, we get:
- f $$\Delta \alpha = \Delta \theta \frac{sin\;\phi}{cos\;\delta}$$

If we now use the cosine rule but for declination, we would get the following:
- f $$\Delta \delta = \Delta \theta\;cos\;\phi$$

And now, if we wanted to know how much we have traveled:
- f $$(\Delta \theta)^2 = (\Delta \alpha\;cos\;\delta)^2 + (\Delta \delta)^2$$


And, coming back to the beginning, we can calculate the **real motion of a star**, by calculating both the tangential and radial velocity, with:
- f $$v = \sqrt{v_t^2 + v_r^2}$$


