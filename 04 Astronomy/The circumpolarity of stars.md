---
tags:
  - star
  - astronomy
  - coordinate_systems
  - celestial_sphere
  - observation
  - calculation
  - mathematics
---
When we look up into the night sky, we see [[Stars]]. Lots of them. We have, throughout history, given them names, assigned them shapes (constellations), and given rise to a comprehensive guide to where is what in the sky. However, not every star is visible from every location on Earth, and some stars we don't see all the time! 

Based on their visibility, we divide stars into 3 categories:
1. <mark style="background: #f2e863;">CIRCUMPOLAR</mark> - always visible
2. <mark style="background: #f2cd60;">RISING AND SETTING STARS</mark> - they rise and set, we see them for a set amount of time
3. <mark style="background: #f25757;">ANTICIRCUMPOLAR</mark> - from our latitude, we never see them

Our visibility of stars depends on 2 factors:
- **Our latitude** - depending on where you we are on Earth, we can see different portions of the sky, meaning our *horizon* ([[The celestial sphere]]) will be higher/lower.
- **The declination of the star** - depending on the star's position itself, we might not be able to see it.
![[circumpolar stars.jpeg|400]]
### Star A
---
Star A is circumpolar, since its parallel of declination is above the horizon and we can see it at all times. Let the point between NSP and N where the parallel of declination touches be called $M$. In order for a star to be circumpolar then, it is obvious that: (NSP = P)
- eg $$PM < PN$$, or $$90º-\delta < \phi$$ $$\delta > \phi - 90º$$

- n $M$ is called the **lower culmination** of star A, while the point between Z and T where the parallel of declination touches is called **upper culmination**. It can be bellow or above the zenith. 

![[culminations.jpeg]]

We can therefore conclude (from the image above) that:
1. Above the Zenith:$$h_d = \phi - 90º + \delta$$ and $$h_g = \phi + 90º - \delta$$
2. Below the Zenith:$$h_d = \phi - 90º + \delta$$, and $$h_g = 90º - \phi + \delta$$
If we knew the heights of the upper and lower culmination, using some simple algebra we could determine that:$$\delta = \frac{1}{2}(h_g + h_d)$$ and that$$\phi = 90º - \frac{1}{2}(h_g - h_d)$$
- !! Another thing worthy of mentioning is that the Hour Angle (H) for a n upper culmination is 0 hours, while for a lower culmination is 12 hours. 

## Rising and setting stars
---
These have a specific rising and setting time, when:$$\phi-90º < \delta < 90º-\phi$$
What are the rising and setting times of stars? Well, they rise/set when **their altitude is 0!** So, if we know the value of RA ($\alpha$) and knowing the relationship between standard time, H and $\alpha$ we can calculate H using the ==conversion from the HA-dec system to the horizontal system==([[Transformations of astronomical coordinates]]) $$sin\;h = cos\;H\;cos\;\delta\;cos\;\phi + sin\;\delta\;sin\;\phi$$
$$\begin{align} cos\;H\;cos\;\delta\;cos\;\phi = sin\;h - sin\;\delta\;sin\;\phi \\
cos\;H = \frac{sin\;h - sin\;\delta\;sin\;\phi}{cos\;\delta\;cos\;\phi} \\
cos\;H = -\frac{sin\;\delta\;sin\;\phi}{cos\;\delta\;cos\;\phi} + \frac{sin\;h}{cos\;\delta\;cos\;\phi} \\
cos\;H = -tg\;\delta\;tg\;\phi + \frac{sin\;h}{cos\;\delta\;cos\;\phi}
\end{align}$$
And if we assume that $h=0º$ without atmospheric refraction ([[Perturbation phenomena]]) then we get the final formula of:
- eg $$cos\;H = -tg\;\delta\;tg\;\phi$$

When it comes to the rising and setting time of the Moon, we account for it when the altitude of the moon is equal to the atmospheric refraction, minus the apparent radius of [[The Moon]] (on average 15.5') and $\pi$ or parallax (57' on average). 
## Anticircumpolar stars
---
These stars never rise and never set since *we can never see them from our latitude!* So, if:$$h_d < 0, or\;\delta < \phi - 90º$$
- !! All of this is also true for the **southern hemisphere** if we switch the signs of the declination and the latitude. Everything is symmetrical!

