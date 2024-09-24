---
tags:
  - sun
  - astronomy
  - motion
  - celestial_sphere
  - coordinate_systems
  - calculation
---
[[The Sun]] is at the centre of [[The solar system]], and [[Earth]] is one of the planets orbiting it. Its orbit is an *elliptical path*, with varying speeds across the year. In the same way that Earth orbits the Sun, the Sun's apparent motion around the Earth is also an ellipse and we call this the **ecliptic**.

![[ecliptic.png]]
## As seen from Earth
---
![[height of sun.jpeg|400]]
The sun appears to revolve around the Earth once a day tracing a yearly path called the ==ecliptic==! Because of this, the Sun's *declination changes throughout the year, having a peak and a minimum in winter and in summer - at the solstices*. We can see the changes in declination in the graph above, and we can track the change in declination as follows:
$$PA = 90º = 90º-\phi + z + \delta$$
or $$\delta = \phi - z, z = +-(\delta - \phi)$$
# Declination of the Sun
---
![[ecliptic_dec_ra.jpeg|400]]

On the image above we can see how the Sun passes through its yearly path called the ecliptic, and we can also notice that the ==angle between the equator and ecliptic is 23.5º==!! This angle is called the **obliquity of the ecliptic**. The Sun also goes through the 12 zodiac constellations, as we all know. They are in order: Aries, Taurus, Gemini, Cancer, Leo, Virgo, Libra, Scorpius, Sagittarius, Capricornus, Aquarius and Pisces. 

The Sun reaches a couple of important points throughout its journey:
- *winter solstice* - the lowest declination value, shortest day and longest night, 21.12.
- *spring equinox* - declination is 0º, day and night are equal, 21.3.
- *summer solstice* - highest declination value, longest day and shortest night, 21.6.
- *autumn equinox* - declination is again 0º, day and night are equal, 21.9.

However, the declination of the Sun varies throughout the year continuously, not just during these 4 points. Since the Sun is at the ecliptic, its ecliptic latitude is always equal to 0. We also know that the ecliptic longitude depends on the Sun's position in orbit, which of course depends on the **orbit or ecliptic**. It takes the sun one ==tropical year== to complete the path of the ecliptic ([[Time systems in astronomy]]). We then calculate the angular speed of the sun (in radians) and multiply by the current time to gain the **position**: $$\lambda = \frac{2\pi}{T_{trop}}t$$
Using the information about the ecliptic latitude and longitude as well as the last equation in [[Transformations of astronomical coordinates]], we get the following:
- n $$sin\;\delta = sin\;\epsilon\;sin\;\lambda$$, where then delta is equal to:$$\delta = arcsin[sin\;\epsilon\;sin\;(\frac{2\pi}{T_{trop}}t)]$$

# Length of a day
---
The length of a day varies throughout the year, as the Sun's declination changes accordingly. It is easy for the equinoxes as H=+-90º, so day and night are both exactly 12 hours. 

But what about every other point inbetween? Well, we can use the relationship between the hour angle, rectascension and standard time ([[Time systems in astronomy]]) ([[The celestial sphere]]) to determine the rising and setting times of the Sun throughout the year. We derived an equation for calculating the Hour angle for rising and setting stars in [[The circumpolarity of stars]]:$$cos\;H = -tg\;\delta\;tg\;\phi$$
We can see the Sun for $2H$ and the declination is equal to the Sun's declination throughout the year. We also need to convert everything into hours. 
- f $$t_{day} = 24h[1 - \frac{1}{180º}arccos(tg\;\delta_s\;tg\;\phi)]$$

, where we used the identity:
- n $$arccos(-x) = 180º - arccos\;x$$ since we all know that $$cos(180º-x) = -cos(x)$$

