---
tags:
  - time
  - astronomy
  - coordinate_systems
  - celestial_sphere
  - space
  - calculation
  - numbers
  - math
  - history
---
Over time, people developed a sense of timekeeping with a steady and correct source, [[The Sun]]. 
- eg **Apparent solar day** = the time between successive passages of the Sun over the observer's meridian, or 24h
However, due to the apparent diurnal rotation of the heavens, we developed another definition of a day:
- **Sidereal day** = the time between two successive passages of a star across the observer's meridian

![[timekeeping1.png]]
Here we can see an illustrative form of the difference between a solar and a sidereal day, and why a sidereal day is **4 minutes shorter than a solar day**, since it take the earth an extra 1º to rotate fully to face the sun again. 

We can have a relationship between the sidereal and solar day where we know that there will always be **one more or one less synodic day than sidereal day** (depending on the fact if the planet rotates clockwise or retrograde)
- f $$\frac{1}{\tau} = \frac{1}{\tau_*} - \frac{1}{P}$$ and retrograde: $$\frac{1}{\tau} = \frac{1}{\tau_*} + \frac{1}{P}$$, where $\tau$ is the length of a synodic day, $\tau_*$ is the length of a sidereal day and $P$ is the orbital period around [[The Sun]].

## Sidereal time
---
- we already know that the First Point of Aries from [[coordinate systems in astro]] is used as a reference point for a sidereal day
- we also know that  **local sidereal time** is the same as the **HA vernal equinox** 
	- we can thus conclude that LST depends on the observer's longitude, as LST changes around the globe (also the reason for timezones and whatnot)

$$LST = HAX + RAX$$, or the local sidereal time is equal to the HA of object X and its right ascension. 

- !! NOTE: if RA is greater than LST then we first add 24h to LST and then subtract RA

However, we have a problem. But of course we do. *The reference point or the vernal equinox **precesses***. This means that its position changes over time, forcing us to keep adjusting our time systems. 
$\ce{->}$ the gravitational effects of the Sun and Moon cause small changes in the obliquity of the ecliptic, making the reference point precess
> So, time is moving backwards at a steady rate called **general precession**

- eg The *equation of the equinoxes*: $$equation \; of \;the\;equinoxes = GAST - GMST$$, where GAST means Greenwich Apparent Sidereal Time and GMST means Greenwich Mean Sidereal Time

Moving on, we can see that the time between transits of a celestial object over the main meridian and the local meridian is actually **longitude**. 
![[timekeeping2.png]]
From this we can conclude the following:$$GST = HA_{vernal} + \lambda W$$, or in other words:$$GAST = LST + \lambda W$$ but if the observer were east then: $$GAST = LST - \lambda E$$
However, sidereal time has 2 variants: **apparent and mean**, where the apparent time is determined from the *true position of the vernal equinox*, while the mean time is determined from the mean position of the equinox were it not for **precession and nutation** ([[Perturbation phenomena]].) So, the *equation of the equinoxes* to account for the difference is:
- f $$LST_a - LST_m = \Delta \psi \cos \epsilon$$, where $\psi$ is the nutation in longitude, and $\epsilon$ is the obliquity of the ecliptic.

If we wanted to see the sidereal time at some point **after** the vernal equinox, we would use the following:
- f $$LST \approx T + 12h + 4n$$, where $n$ is the amount of days after March 21st, and T is the local solar time.

## Mean solar time
---
The Sun used to be used extensively for timekeeping, with **sundials** being very fashionable. In that sense, the **apparent solar day** was the time between successive passages of the Sun across the observer's meridian, meaning that the Sun's hour angle had a value of 12 hours (which might be why the Romans used a 12 hour clock). And yet again we have a problem. The Sun isn't perfect, or well Earth's orbit isn't!
- !! The Earth's orbit around the Sun is elliptical so, taking into account [[Kepler's second law - the law of areas]], we can see how a day might vary throughout the year.
- !! The Earth's axis is also tilted, so the ecliptic is at an angle of 23,5º against the equator

So, we solve real problems by *inventing objects*, so we invented a **fictitious body called the Mean Sun**, and with it we measure ==mean solar time==. This body moves along the equator and not the ecliptic, keeping in touch with the mean angular velocity of our real Sun. A day of this time is called the **mean solar day**. 

In order to make our fictitious Sun a bit more useful, we need to align it with the real Sun, and this means we have to make it move so the right ascension increases at a constant rate. 
![[timekeeping3.png]]
We make this work by introducing another fictitious body! The **dynamical mean sun**. Basically, we have the mean sun and the dynamical sun, where the dynamical one (*D on the image above*) moves along the ecliptic mimicking the motion of the sun but with a mean angular velocity instead of the actual one. Its motion is tracked by the mean sun, which travels along the equator. You can imagine M and B being projections of the motions of D and S on the equator for measurement of RA.

- eg BM is referred to as the **equation of time**, since it shows the difference between the RA of the mean and the real Sun:$$equation\;of\;time= RAMS − RA$$, where RAMS is the right ascension of the mean sun, and RA is of the Sun. Remembering our old equation:$$LST = HA + RA$$, we can say that LST should be equal for both the real and the mean sun:$$LST = HAS + RAS = HAMS + RAMS$$Using these two equations, we can conclude that the equation of time is also equal to $$equation\;of\;time= HA - HAMS$$

Depending on the time of year, the equation of time changes in value (depending on the differences in the mean and actual angular velocity),  from -14.5 minutes to about 16.25 minutes. The following graph shows how much it fluctuates: ![[timekeeping4.png]]
## Universal time and Greenwich
---
We also have the concept of universal time, which is equal to Greenwich Mean Time, or:$$GHAMS +- 12h = GHA - equation\;of\;time\;+12h$$
We have the **ephemeris transit**, which is when the Sun transits the ephemeris meridian, very close to Greenwich, a bit to the east. We can approximate this time with:$$Ephemeris\;transit = 12h-\;equation\;of\;time$$

Greenwich is the standard meridian or the reference meridian for timekeeping on Earth. The hour angle of the mean sun is 0 when passing through Greenwich, so GHAMS is 0 at mean noon and 12 at mean midnight. 
But, we are mere mortals, and we use **greenwich mean time GMT** for our day to day timekeeping, which centers midnight at  12h. $$GMT = GHAMS +-12h$$
Since at every degree of the Earth timekeeping changes a little bit, (to be precise 4 minutes), we adopted **standard time zones** for people to be able to live their lives normally. This time is called **Zone Time or Standard Time ZT, ST** where each time zone is 15º or 1h wide! The zone separating the border between east and west is the **International Date Line**, where the day begins...

So, the time in a given place is$$GMT = ZT + \lambda$$, where $\lambda$ is the longitude. 

## What about a year?
---
We have only talked about days, but what about years of time? For normal people, we use the **tropical year** to measure 1 year of time, or 2 successive passages of the Sun through the vernal equinox. This equates to ==365.2422== mean solar days. Since it is not a whole number, we have leap years with 366 days, every 4 years. Today we use the **Gregorian Calendar**, which is very accurate and makes sure that every year whose hundreds are divisible by 4 are leap years, giving us an average of ==365.2425== mean solar days, pretty accurate! Up until then, every fourth year was a leap year, leading to a discrepancy of 12 days! 

There are actually 2 definitions of a year: **the tropical and sidereal year** of the Earth. The tropical year is based on the time interval between 2 successive passages through the vernal equinox. The sidereal year is the time it takes the Sun to make a complete circuit of the ecliptic, which depends upon [[Precession]]. $$\frac{1\;tropical\;year}{360º - 50"} = \frac{1\;sidereal\;year}{360º}$$
Finally, the **anomalistic year**, or the time between 2 successive passages of the Earth through its perihelion is around ==365.2596== days. 
## Time of stars
---
To avoid any errors between previous and current calendars and timekeeping, we use **Julian Day Numbers**, where the starting date was ==January 1st 4713 BC==, at mean noon, and the days are counted since then. For every normal date there are [[Julian Dates]]. 

### Dynamical time
---
Due to the Earth's rotation not being perfect, we have to take into account the slowing down or speeding up of Earth's rotation, called dynamical time. The relationship between Dynamical Time and the International Atomic Time is:$$TDT = TAI + 32.184s$$
# The seasons
---
> Thus, in spring, the Sun’s right ascension increases from 0h to 6h while its declination increases from 0º to 23º26' N. In summer, the RA increases from 6h to 12h, its declination decreasing from 23º26' N to 0º. In autumn, the RA increases from 12h to 18h, its declination changing from 0º to 23º 26' S. In winter, the RA increases from 18h to 24h, its declination changing from 23º 26' S to 0º, at which time spring begins again.

# Twilight
---
After the Sun sets, due to the Earth's atmosphere, some sunlight still passes to the observer, marking ==civil, nautical and astronomical twilight==. Civil is when the Sun is below 6º, nautical when 12º below and finally astronomical when its 18º below the horizon. 

![[timekeeping5.png]]
And we use the image above to calculate the time of twilight, and we of course use [[Spherical trigonometry]] for this. 


## Julian time
---
If we needed to transform time into the J2000.0 epoch of the Julian calendar, we need to adjust the right ascension and declination via:
- f $$\Delta \alpha = M + N\;sin\;\alpha\;tan\;\delta$$$$\Delta \delta = N\;cos\;\alpha$$
 Where M and N are:$$M = 1.º2812323T + 0.º0003879T^2 + 0.º0000101T^3$$, and $$N = 0.º5567530T - 0.º0001185T^2 - 0.º0000116T^3$$,where $T$ is:$$T = (t-2000.0)/100$$ and $t$ is the fraction of a year we are currently in, like the current date. If we know what the Julian Date (JD) is, then we can also say:$$T = (JD - 2451545.0)/36525$$


