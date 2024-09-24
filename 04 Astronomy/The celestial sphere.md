---
tags:
  - astronomy
  - coordinate_systems
  - mathematics
  - observation
  - celestial_sphere
---
Just like on the [[Earth]], we use coordinate systems in order to track various objects in the night sky. There are many different kinds, so here is an overview of all the types we use in astronomy - each has its own purpose!



## Earth's coordinate system
---
But before we tackle astronomical systems, let's review Earth's coordinate system. As we all know, Earth is a sphere (well, not quite but extremely close, its an oblate spheriod), so we use [[Spherical trigonometry]] for any complex calculations. 

![[geo_system.jpeg|400]]

We have 2 main coordinates: **longitude and latitude**, which are built by passing great circles through our position on Earth (X). Latitude is the angle between the equatorial plane and the straight line through XO. Longitude is the angle between the greenwich meridian and the straight line passing through XO. 

Longitude is used for [[Time]] tracking on Earth, while latitude tells us what we can observe in the night sky.

On Earth we have another value, **the height** of the observer! We discuss this more in [[Limitations to observations in astronomy]]. 

![[plumb line.png]]
*Here is a representation of the lattitude and how we use it later in **the horizontal coordinate system***. 

### But, Earth is not a sphere?
---
Well, yes, the Earth is an **oblate spheriod**, which makes it a tad harder to do calculations, although the discrepancies are minor. So, we have a different geocentric and geodetic latitude. How do we calculate the difference?

If the Earth is an oblate spheroid, we can approximate it as an ellipse, like so:
![[different latitudes.png]]

We know that:$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$, since we are talking about an ellipse. The eccentricity is:$$e = \sqrt{\frac{1-b^2}{a^2}}$$, and we can get:
- f $$\tan\;\phi' =\frac{b^2}{a^2}\;\tan\;\phi = (1-e^2)\tan\phi$$


# The horizontal coordinate system
---
Now that we have a base, our first coordinate system is the horizontal one! In the horizontal system, we value the **observer's position** over everything else. For starters, we have 2 very important points: ==zenith and nadir== - the 2 points directly above and below the observer. They form a 90º angle with the **horizon**, another important aspect of the system. Next, we have the *equator and poles*, and while these are important for another coordinate system, they are necessary for the horizontal one to provide context.
- eg The horizontal system is **location specific** - it isn't useful for tracking the positions of objects in the night sky permanently, rather night to night. So, to put things in context we include the equator and poles for objectivity

![[horiz_sys1.jpeg|300]]

Looking at the illustration, the **latitude $\phi$** is the angle between the ==horizon and the pole projected onto the horizon==. Latitude is an elementary component of the Earth's coordinate system consisting of **latitude and longitude**. 
- !! Latitude is directly related to which part of the sky we see and don't see, so it is very important to include it in coordinate systems.

![[horiz_sys2.jpeg|300]]
On the horizon, there are *4 cardinal points* - North, East, South and West, and we use **azimuth** in angles from 0º to 360º to measure it. The arcs between each cardinal point is called a *vertical*. 
- !! Azimuth is measured **westward along the horizon**, or the **angle between the vertical through the north point and the vertical through the object X**, or in other words, **clockwise from the North**!!! (Wrong in the image)!!!
- !! **True bearing** is a third way of measuring azimuth, from the north point eastwards
The second coordinate for the horizontal system is called **altitude**, which is the angular distance from the horizon to the object of interest. 

Here is a bit of perspective depending on the latitude of the observer, as seen from the. horizontal system:
![[horizontal system 2 ways.png]]


# Equatorial coordinate system
---
This coordinate system is based on the **celestial equator**, which makes it more objective and able to track the motions of the objects for loong periods of time. The first type, HA-dec still relies on time, while the second, RA-dec is true for long periods of time. Both systems use the dec coordinate.
### 1st type - HA-dec system
![[HAdec.jpeg|400]]
Every object travels along its ==parallel of declination==, the red line in the drawing above. The object has its **point of transit**, or when it reaches its maximum and passes the observer's meridian. Along its parallel of declination, the object *transits, sets, rises and has a minimum point*! 
- eg **Declination ($\delta$)** is the angular distance in degrees of the star from the equator along the meridian through the star

Another parallel quantity is the **north polar distance**:$$npd = 90º - \delta$$
And the ==second== coordinate is the **hour angle**:
- eg **Hour angle (H)** is measured from the observer's meridian westwards to the meridian through the star from 0 to 24h - it increases by 24h each sidereal day for a star

On the illustration, we also have 3 points: $R, S$ and $C$. $R$ represents the point at which our object **rises** into our field of view, $C$ is the **culmination point**, or the highest point it reaches in a day, and $S$ is the point at which the object sets, or disappears from view. 

### 2nd type - RA-dec system

![[RA-dec.jpeg|300]]

This second type is independent of time, and uses the RA coordinate or rectascension - it is the angle from the vernal equinox counted anti-clockwise from the vernal equinox and measured in hours. It is independent since the vernal equinox is the point at which the **ecliptic** - path of the sun hits the equator. It is constant throughout the year, as well as the equinox, so these coordinates are time independent. (However, due to [[Perturbation phenomena]], these coordinates do change). This coordinate system (as well as the ecliptic coordinate system), rely on the [[Motion of the Sun]].

Actually, since the vernal equinox is a point on the stellar background, it ==rotates around the Earth, transiting, rising and setting==. So, taking the hour angle of the first point of Aries(FPA) has a specific meaning, and it is called **local sidereal time!** We can see that if X is the star, that RA of X is the arc from the FPA to B, and the hour angle of X is the arc from A to B, and so we realise that actually:
- !! $$H + \alpha = LST!$$

![[sidereal time and equator.png]]

# Ecliptic coordinate system
---
Using the [[Motion of the Sun]], we can create another coordinate system which is perfect for tracking the motion of the planets across the sky. Its base is again the celestial equator, but also the ecliptic. 

![[ecliptic (from earth and sun).png]]
- *a super important diagram which shows the ecliptic coordinate system from Earth's or the Sun's perspective.*

![[ecliptic_coord.jpeg]]
# Galactic coordinate system
This system is super useful for vizualising objects in the galaxy, using the fact that the Galaxy is lens-shaped with the Sun in or near to the. median plane of the lens. We also have the ascending and descending nodes, but they aren't points of solstices but rather where the ==galactic equator intersects the celestial equator (N and N' in the drawing below)==. 
![[coord18.png]]
Every object with its coordinates in RA and Dec has corresponding galactic coordinates in latitude and longitude. 
**Galactic longitude** or $l$ is measured along the galactic equator to the point F in degrees. L is our reference point, and it was determined by the position angle PGL, which  which is equal to 123º. The **galactic latitude** or $b$ is measured along the great semicircle of X, or from F to X. Again, we use spherical triangles to calculate the conversion from Equatorial to galactic coordinates. 

![[meaning of galactic coords.png]]

