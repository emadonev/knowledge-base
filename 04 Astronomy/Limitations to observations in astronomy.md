---
tags:
  - astronomy
  - math
  - physics
  - light
  - atmosphere
  - observation
  - telescope
---
[[Light]] is known to change its **angle of incidence** when passing from one material through another due to the **different refraction indexes of materials**. 
- !! The first law of refraction: *The incident ray, the normal and the refracted ray are coplanar.* ![[first law ref.png]]

- !! The second law of refraction:$$\frac{sin \; i}{sin \; r} = n$$, where $i$ is the incident angle, $r$ is the exiting angle and $n$ is the **index of refraction.**  (derivation includes derivatives, so come back to another time)

# Astronomical refraction
---
What's important for us is the **astronomical refraction** of the light which comes from [[Stars]] so we can observe them with [[Telescopes]] properly. 
![[astronomical ref.png]]
We can see that through the atmosphere of the [[Earth]], light refracts many many times, and we can make a good approximation of the real zenith distance of a star based on previous knowledge. $z$ is the true zenith distance, since X is parallel to the starting AB ray of light. $\xi$ is the apparent zenith distance. Using Snell's law, we can say that: $$sin \; z = n \; sin \; \xi$$
And also $R = z - \xi$ be the angle of refraction, since that is the difference between the true and apparent value. So, we can measure R  to get the true zenith distance:$$z = R+ \xi$$And using some [[Fundamental trigonometry]], we can get that:$$R = 206265(n-1) \; tan\; \xi$$ or we can use the constant $k$ instead:$$R = k \; tan \; \xi$$
# Constant refraction
---
We can also have a constant refraction when considering **circumpolar stars**, where the entire observed path of a star is refracted due to the atmosphere. AB is the observed path, but CD is the **real path**.
![[constant ref.png]]
We can see that:$$CA = k \; tan \;\xi_A, \; DB = k\;tan\;\xi_B$$
From the image, we can see that ZC is the real zenith distance, which we can get by adding ZA, the apparent zenith distance and AC, or R. 
$$ZC = PC-PZ = 90 - \delta - (90 - \phi) = \phi - \delta$$
- !! $$\phi - \delta = \xi_A + k\;tan\;\xi_A$$
Analogous to that:$$ZD = ZP + PD = 90 - \phi + 90 - \delta = 180 - \phi - \delta$$
- !! $$180 - \phi - \delta = \xi_B + k\;tan\;\xi_B$$

# Horizontal refraction
---
What if we are observing from the horizon? The Earth is not a flat sphere, so there are mountains and such which make us able to see more than we should, plus we have **atmospheric refraction at the horizon, 35' to be exact.** (At least for 0º apparent altitude). 
![[horizontal ref.png]]
Our first step is to calculate the angle of our dip, meaning how below we can see below our vantage point at O. We can see that the actual altitude is actually:$$a = a' - \theta$$, where $a'$ is the observed altitude. Using the fact that TCO = $\theta$, we can say that:
- !! $$cos \;\theta = \frac{R}{R+h}$$

So, we can observe: $$\epsilon = \theta + 35'$$
So for circumpolar stars: $$\delta > 90 - (\phi + \epsilon)$$
