---
tags:
  - motion
  - position
  - orbits
  - astronomy
  - planet
  - physics
  - mathematics
---
Now that we understand **why and how** planets move, let's take a look at how we can put things into perspective for Earth and how planets move with respect to the Earth. 

We distinguish 2 types of planets: **inferior and superior**. Inferior are the ones before Earth, and superior the ones after. All of the planetary positions are denoted in the image below:
![[planetary positions.jpeg]]
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
![[retrograde_mars_eartjPOV.png]]



### Phase of a planet
---
An interesting property of the planets and [[Light]] is the **phase of a planet**, which we can observe in eg. [[Venus]] and the [[Moon]]. And we can use some simple geometry and [[Fundamental trigonometry]] to get to the answer. 
![[phase of planet.png]]
From the position of [[The Sun]], the light part of the photo is visible, but from the [[Earth]]'s perspective, only above line CD is everything visible, meaning that PBD is going to be dark - the phase of the planet. 

So, the phase of a planet is really:$$phase = \frac{CF}{CD} = \frac{CP + PF}{CD}$$ and using some trigonometry, 
- !! $$phase = \frac{CP + cos\;\phi\;CP}{2CP} = \frac{1}{2}(1+cos\;\phi)$$

--- 
However, we want to find the phase of the planet depending on its position around the Sun. For that, we need the angle theta in the drawing above to see what's what. Using the sine formula:$$\frac{SE}{sin\;\phi} = \frac{SP}{sin\;(180-(\theta+\phi))}$$ So we can get that:$$SP\;sin\;\phi = SE\;sin\;(\theta+\phi)$$ where we can use the fact that the tangent is equal to the sine over cosine, we can get:$$tan\;\phi = \frac{SP\;sin\;\theta}{SE - SP\;cos\;\theta}$$ and we can calculate theta by:$$\theta = 360 \frac{t}{S}$$, where $t$ is the time which has passed since the beginning of the cycle, an $S$ is the *synodic period*
