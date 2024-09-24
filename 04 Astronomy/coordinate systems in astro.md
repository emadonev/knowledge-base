---
tags:
  - astronomy
  - coordinate_systems
  - numbers
  - calculation
  - celestial_sphere
  - star
  - space
---
# The horizontal system
---
In the horizontal system, we value the **observer's position** over everything else, as the first image shows:
![[coord1.png]]
For starters, we have 2 very important points: ==zenith and nadir== - the 2 points directly above and below the observer. They form a 90º angle with the **horizon**, another important aspect of the system. Next, we have the *equator and poles*, and while these are important for another coordinate system, they are necessary for the horizontal one to provide context.
- eg The horizontal system is **location specific** - it isn't useful for tracking the positions of objects in the night sky permanently, rather night to night. So, to put things in context we include the equator and poles for objectivity

Looking at the illustration, we can conclude that P2OB is parallel to P1CQ, making the **latitude $\phi$** the angle between the ==horizon and the pole projected onto the horizon==. Latitude is an elementary component of the Earth's coordinate system consisting of **latitude and longitude**. 
- !! Latitude is directly related to which part of the sky we see and don't see, so it is very important to include it in coordinate systems.

On the horizon, there are *4 cardinal points* - North, East, South and West, and we use **azimuth** in angles from 0º to 360º to measure it. The arcs between each cardinal point is called a *vertical*. 
- !! Azimuth is measured **westward along the horizon**, or the **angle between the vertical through the north point and the vertical through the object X**. 
- !! **True bearing** is a third way of measuring azimuth, from the north point eastwards
The second coordinate for the horizontal system is called **altitude**, which is the angular distance from the horizon to the object of interest. 
![[coord2.png]]
$$a,h - altitude, A - azimuth$$
We also use a second quantity called the *zenith distance*, and the relationship is as such:$$a = 90º-z$$
where $z$ is the zenith distance.

# Equatorial system
---
This coordinate system is based on the **celestial equator**, which makes it more objective and able to track the motions of the objects for loong periods of time (where they truly are in the sky). 
![[coord3.png]]
Every object travels along its ==parallel of declination==, the red line in the drawing above. The object has its **point of transit**, or when it reaches its maximum and passes the observer's meridian. Along its parallel of declination, the object *transits, sets, rises and has a minimum point*! 
- eg **Declination ($\delta$)** is the angular distance in degrees of the star from the equator along the meridian through the star

Another parallel quantity is the **north polar distance**:$$npd = 90º - \delta$$
And the ==second== coordinate is the **hour angle**:
- eg **Hour angle (H)** is measured from the observer's meridian westwards to the meridian through the star from 0 to 24h - it increases by 24h each sidereal day for a star

### Southern hemisphere
If you are wondering what this all looks like from the southern hemisphere, here is a diagram:
![[coord4.png]]
# Circumpolar stars
---
Every star or constellation can be put into exactly 3 classes
1. Stars that are above the horizon for all values for their hour angle (*constantly above the horizon*) - **CIRCUMPOLAR STARS**
- !! These stars are always above the horizon, so they have **upper and lower transits or *culminations*** 
2. Stars that are below the horizon for all values for their hour angle (*constantly below the horizon*) - **ANTICIRCUMPOLAR STARS**
3. Stars that rise and set (*parts are below and parts above the horizon*) - **REGULAR STARS**

The following image depicts stars:
![[coord5.png]]

As you can see from the image, the green lines are circumpolar stars, the black lines are the "normal" stars, and the red lines are anticircumpolar stars. But, how do we define which star falls into which category?

### Circumpolar star category
So, CD is parallel to the declination of star $X_2$. We can see that if we want the star to be circumpolar:
- o  PD has to be less than PN - it has to be above the horizon! From the diagram, we can see that:$$90-\delta < \phi$$ $\ce{->}$ PD is equal to $90-\delta$ because PC is $90-\delta$, and CD are equally distant from P, hence their values are equal, and PN is obviously the latitude

If our star has the upper transit on the south side of the zenith, then PC must obviously be larger than PZ:
- o $$90-\delta > 90-\phi$$ $\ce{->}$ As mentioned before, PC is also $90-\delta$, and PZ is $90-PN$, or $90-\phi$ $$\phi > \delta$$

### "Normal" and anticircumpolar stars
Since these stars are constantly below the horizon, they aren't exactly defined, but there is of course a limiting declination that a particular observer can see, and so every star which is below this limit is invisible. We can see from the image above that the ==declination is the limiting value==, $JS = 90-\phi$, and $JQ=90º$, and $SQ = 90-\delta$. Combining all of these values together:
- o $$180-\phi -\delta = 90$$$$\phi + \delta = 90$$
Hence, if the declination is less than $90-\phi$, then the star comes above the horizon, and if it is greater than or equal to this value, it never goes above the horizon. 

Solving problems with coordinate systems always require drawing out the system, and it isn't very hard:
1. Draw a sphere
2. Draw in the horizon, the horizontal circle with the radius of the sphere
3. Draw the equator at an angle agains the horizon, and this angle is $90-\phi$
4. Draw a vertical line in reference to the horizon which passes through the centre of the sphere - where it intersects with the sphere in the above hemisphere, that is the ==zenith==, and the angle between the zenith and horizon iz $90º$
5. Draw another vertical line in reference to the equator which passes through the centre of the sphere - where it intersects with the sphere in the above hemisphere, that is the ==north pole==, and the angle between it and the equator is $90º$
6. Insert the rest of the diagram as so:
![[coord7.png]]


## Geocentric celestial sphere
![[coord6.png]]
This shows that if we look at objects inside our solar system, the coordinate system falls apart a bit since **the distance is very small**, while for the stars we can ==assume they are infinitely far away==.  

# Conversions between systems
---
![[coord8.png]]
![[coord9.png]]
As you can see from the images above, in an example of converting from one system to another, [[Spherical trigonometry]] is required! When we correctly attribute every section, we realise that we get a spherical triangle with which we use the classical formula to calculate.

![[coord10.png]]
$\ce{->}$ another example!

# Equatorial system - with RA
---
Even though the equatorial system works great, it still has a problem - **the hour angle**. It constantly changes as time passes, so we need a new way to catalogue stellar positions. We ==need to choose a meridian which is connected directly to the celestial sphere==, so we can get a good, objective coordinate system. 
- o We chose the **first point of Aries** or the **VERNAL EQUINOX** as our reference point. And with that, we chose **right ascension RA** as the next coordinate - it is the angle measured along the equator from the vernal equinox eastward to the meridian of interest

# The Sun throughout the year
---
![[coord11.png]]
The sun appears to revolve around the Earth once a day tracing a yearly path called the ==ecliptic==! Because of this, the Sun's *declination changes throughout the year, having a peak and a minimum in winter and in summer - at the solstices*. We can see the changes in declination in the graph above, and we can track the change in declination as follows:
$$PA = 90º = 90º-\phi + z + \delta$$
or $$\delta = \phi - z$$
![[coord12.png]]
On the image above we can see how the Sun passes through its yearly path called the ecliptic, and we can also notice that the ==angle between the equator and ecliptic is 23.5º==!! This angle is called the **obliquity of the ecliptic**. The Sun also goes through the 12 zodiac constellations, as we all know. They are in order: Aries, Taurus, Gemini, Cancer, Leo, Virgo, Libra, Scorpius, Sagittarius, Capricornus, Aquarius and Pisces. 

The Sun reaches a couple of important points throughout its journey:
- *winter solstice* - the lowest declination value, shortest day and longest night, 21.12.
- *spring equinox* - declination is 0º, day and night are equal, 21.3.
- *summer solstice* - highest declination value, longest day and shortest night, 21.6.
- *autumn equinox* - declination is again 0º, day and night are equal, 21.9.

![[coord13.png]]
This diagram above shows the motion of the sun throughout the day. 

# Determining the sunset and sunrise
---
![[coord14.png]]
This is the celestial sphere indicating a sunrise for the Sun, obviously. Using spherical trig, we can calculate the Hour angle of the sun at sunrise, since the times change throughout the year **depending on the declination of the Sun**. If the latitude is north and dec positive, then it must be between 6 and 12 hours, and if dec is negative it is between 0 and 6 hours. We also note that the azimuth for the sun setting is also determined via spherical trig, and if the declination is positive, then its between 270 and 360 degrees, and if declination is negative then between 180 and 270. 

![[coord15.png]]
And this is the celestial sphere at sunset! The same applies here as with the sunrise, and the northern latitudes with positive declinations the azimuth limit is from 0 to 90, and the hour angle is from 12 to 18 hours. For negative declinations the azimuth limit is from 90 to 180, and the hour angle limit is from 18 to 24 hours. 

# Sidereal time
----
![[coord16.png]]
Actually, since the vernal equinox is a point on the stellar background, it ==rotates around the Earth, transiting, rising and setting==. So, taking the hour angle of the first point of Aries(FPA) has a specific meaning, and it is called **local sidereal time!** We can see that if X is the star, that RA of X is the arc from the FPA to B, and the hour angle of X is the arc from A to B, and so we realise that actually:
- !! $$H + \alpha = LST!$$

# Ecliptic coordinates
---
![[coord17.png]]
Of course, we have another system just for studying the **movements of the planets and the solar system**, to make things easier... and this system consists of the *ecliptic longitude and latitude*! The ==ecliptic longitude== is the angle between the FPA to point D, and it is measured along the ecliptic in the eastwards direction. The ==ecliptic latitude== is measured from D to X, or along the meridian of the object. In this coordinate system, FPA is often referred to as the *ascending node*, and the Libra point or the winter solstice point is often called the *descending node*. As per previous coordinate systems, we use spherical trig for everything!

# Galactic coordinate system
---
This system is super useful for visualising objects in the galaxy, using the fact that the Galaxy is lens-shaped with the Sun in or near to the. median plane of the lens. We also have the ascending and descending nodes, but they aren't points of solstices but rather where the ==galactic equator intersects the celestial equator (N and N' in the drawing below)==. 
![[coord18.png]]
Every object with its coordinates in RA and Dec has corresponding galactic coordinates in latitude and longitude. 
**Galactic longitude** or $l$ is measured along the galactic equator to the point F in degrees. L is our reference point, and it was determined by the position angle PGL, which  which is equal to 123º. The **galactic latitude** or $b$ is measured along the great semicircle of X, or from F to X. Again, we use spherical triangles to calculate the conversion from Equatorial to galactic coordinates. 

These are all the coordinate systems we use in astronomy and how they work!
