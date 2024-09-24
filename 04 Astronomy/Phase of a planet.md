---
tags:
  - planet
  - astronomy
  - solary_system
  - math
  - geometry
  - physics
---
An interesting property of the planets and [[Light]] is the **phase of a planet**, which we can observe in eg. [[Venus]] and the [[Moon]]. And we can use some simple geometry and [[Fundamental trigonometry]] to get to the answer. 
![[phase of planet.png]]
From the position of [[The Sun]], the light part of the photo is visible, but from the [[Earth]]'s perspective, only above line CD is everything visible, meaning that PBD is going to be dark - the phase of the planet. 

So, the phase of a planet is really:$$phase = \frac{CF}{CD} = \frac{CP + PF}{CD}$$ and using some trigonometry, 
- !! $$phase = \frac{CP + cos\;\phi\;CP}{2CP} = \frac{1}{2}(1+cos\;\phi)$$

--- 
However, we want to find the phase of the planet depending on its position around the Sun. For that, we need the angle theta in the drawing above to see what's what. Using the sine formula:$$\frac{SE}{sin\;\phi} = \frac{SP}{sin\;(180-(\theta+\phi))}$$ So we can get that:$$SP\;sin\;\phi = SE\;sin\;(\theta+\phi)$$ where we can use the fact that the tangent is equal to the sine over cosine, we can get:$$tan\;\phi = \frac{SP\;sin\;\theta}{SE - SP\;cos\;\theta}$$ and we can calculate theta by:$$\theta = 360 \frac{t}{S}$$, where $t$ is the time which has passed since the beginning of the cycle, an $S$ is the *synodic period*. 