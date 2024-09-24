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
# Solar and sidereal time
---
There are 2 main ways of measuring time: if you look at the Sun and track the [[Motion of the Sun]], or if you look at the [[Stars]] and track Earth's rotation on its own axis. The former is perfect for day to day life, tracking time on Earth and keeping timezones intact, while the latter is perfect for astronomy.

<mark style="background: #f2cd60;">A solar day</mark> is the time it takes for the Sun to successively pass through the same meridian. This takes 24 hours or 86400 seconds on average. <mark style="background: #61e8e1;">A sidereal day</mark> is the time it takes a fixed star to successively pass through the same meridian, or the period of rotation of the Earth around its own axis. It is also defined as the *hour angle of the vernal equinox*. 

![[timekeeping1.png]]
Here we can see an illustrative form of the difference between a solar and a sidereal day, and why a sidereal day is **4 minutes shorter than a solar day**, since it take the earth an extra 1º to rotate fully to face the sun again. 

## Time on Earth
---
Moving on, we can see that the time between transits of a celestial object over the main meridian and the local meridian is actually **<mark style="background: #f2e863;">longitude</mark>**. 
![[timekeeping2.png]]
From this we can conclude the following:$$GST = HA_{vernal} + \lambda W$$, or in other words:
- f $$GAST = LST + \lambda W$$

but if the observer were east then: 

- f $$GAST = LST - \lambda E$$

## Mean solar time
---
The Sun used to be used extensively for timekeeping, with **sundials** being very fashionable. In that sense, the **apparent solar day** was the time between successive passages of the Sun across the observer's meridian, meaning that the Sun's hour angle had a value of 12 hours (which might be why the Romans used a 12 hour clock). And yet again we have a problem. The Sun isn't perfect, or well Earth's orbit isn't!

- !! The Earth's orbit around the Sun is elliptical so, taking into account [[Kepler's second law - the law of areas]], we can see how a day might vary throughout the year.
- !! The Earth's axis is also tilted, so the ecliptic is at an angle of 23,5º against the equator

So, we solve real problems by *inventing objects*, so we invented a **fictitious body called the Mean Sun**, and with it we measure ==mean solar time==. This body moves along the equator and not the ecliptic, keeping in touch with the mean angular velocity of our real Sun. A day of this time is called the **mean solar day**. 

In order to make our fictitious Sun a bit more useful, we need to align it with the real Sun, and this means we have to make it move so the right ascension increases at a constant rate. 
![[timekeeping3.png]]
We make this work by introducing another fictitious body! The <mark style="background: #f2cd60;">dynamical mean sun</mark>. Basically, we have the mean sun and the dynamical sun, where the dynamical one (*D on the image above*) moves along the ecliptic mimicking the motion of the sun but with a mean angular velocity instead of the actual one. Its motion is tracked by the mean sun, which travels along the equator. You can imagine M and B being projections of the motions of D and S on the equator for measurement of $\alpha$.

The average solar time or mean solar time $T_m$ is thus this:
- f $$T_{ms} = H_{ms} + 12h$$, so that every day starts at midnight.

We also have the true solar time, which is defined in the same way:
- f $$T_s= H_s + 12h$$

- eg BM is referred to as the **equation of time**, since it shows the difference between the RA of the mean and the real Sun:

- f $$equation\;of\;time= \alpha_{ms} − \alpha_s$$, where RAMS is the right ascension of the mean sun, and RA is of the Sun. Remembering our old equation:$$LST = H + \alpha$$, we can say that LST should be equal for both the real and the mean sun:$$LST = H_s + \alpha_s = H_{ms} + \alpha{ms}$$Using these two equations, we can conclude that the equation of time is also equal to $$equation\;of\;time= H_s - H_{ms}$$

Depending on the time of year, the equation of time changes in value (depending on the differences in the mean and actual angular velocity),  from -14.5 minutes to about 16.25 minutes. The following graph shows how much it fluctuates: ![[timekeeping4.png]]
## Universal time and Greenwich
---
We also have the concept of universal time, which is equal to Greenwich Mean Time, or:$$H_{GMS} +- 12h = H_{G} - equation\;of\;time\;+12h$$
We have the **ephemeris transit**, which is when the Sun transits the ephemeris meridian, very close to Greenwich, a bit to the east. We can approximate this time with:$$Ephemeris\;transit = 12h-\;equation\;of\;time$$

Greenwich is the standard meridian or the reference meridian for timekeeping on Earth. The hour angle of the mean sun is 0 when passing through Greenwich, so GHAMS is 0 at mean noon and 12 at mean midnight. 
But, we are mere mortals, and we use **greenwich mean time GMT** for our day to day timekeeping, which centers midnight at  12h. $$GMT = H_{GMS} +-12h$$
Since at every degree of the Earth timekeeping changes a little bit, (to be precise 4 minutes), we adopted **standard time zones** for people to be able to live their lives normally. This time is called **Zone Time or Standard Time ZT, ST** where each time zone is 15º or 1h wide! The zone separating the border between east and west is the **International Date Line**, where the day begins...

So, the time in a given place is$$GMT = ZT + \lambda$$, where $\lambda$ is the longitude. 

## What about a year?
---
We have only talked about days, but what about years of time? For normal people, we use the **tropical year** to measure 1 year of time, or 2 successive passages of the Sun through the vernal equinox. This equates to ==365.2422== mean solar days. Since it is not a whole number, we have leap years with 366 days, every 4 years. Today we use the **Gregorian Calendar**, which is very accurate and makes sure that every year whose hundreds are divisible by 4 are leap years, giving us an average of ==365.2425== mean solar days, pretty accurate! Up until then, every fourth year was a leap year, leading to a discrepancy of 12 days! 

There are actually 2 definitions of a year: **the tropical and sidereal year** of the Earth. The tropical year is based on the time interval between 2 successive passages through the vernal equinox. The sidereal year is the time it takes the Sun to make a complete circuit of the ecliptic, which depends upon [[Precession]]. 
- f $$\frac{1\;tropical\;year}{360º - 50"} = \frac{1\;sidereal\;year}{360º}$$ or $$\frac{1}{T_{tropical}} = \frac{1}{A} + \frac{1}{T_{precession}}$$, where A is the sidereal year of the Earth.

## Time of stars
---
To avoid any errors between previous and current calendars and timekeeping, we use **Julian Day Numbers**, where the starting date was ==January 1st 4713 BC==, at mean noon, and the days are counted since then. For every normal date there are [[Julian Dates]]. 