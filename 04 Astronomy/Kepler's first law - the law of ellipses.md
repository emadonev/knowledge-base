---

---
TAGS: #kepler #law #ellipse #physics #astronomy #planet #planetary_science #solary_system 

Kepler's first law states that:

>"*All planets orbit their host stars in an elliptical path with 2 focci, one of which is the host star.*"

So, he said that instead of circles, planet's move in ellipses. But how did he discover that? He compared angles of the planet's as they traveled from one point to another, after an equal time interval. If the angles were the same, the path would be circular, <mark style="background: #ccd5ae;">but they weren't!</mark>
![[comparing circles and ellipses.png|200]]

---

There are some basic properties of ellipses which are elementary to orbital dynamics which shall be used again, and again! 

![[basics of ellipse.jpeg|400]]

Using the ellipse above, let's define some properties which are super useful for elementary orbital mechanics. 

All ellipses have 2 focci: in the case of planets, they orbit around one focus, [[The Sun]]. The 2 most famous positions are **aphelion** - the point furthest from the Sun, and **perihelion** - the point closest to the Sun. (ignore the inaccuracy of the picture :FarFaceSmileWink:) 
	Another property is that $$r + r' = 2a$$, or the distance from the focci are always equal to the length of 2 semimajor axes. 

The *semi-major axis*, $a$ is the distance from the centre of the ellipse to either the perihelion or aphelion. It is kind of like the "average" distance of the planet from the Sun. $b$ is the semi-minor axis, and $c$ is the distance from the centre to the Sun. We use $c$ and $a$ to define **eccentricity**, a quantity which tells us how elliptical an orbit is.
- f $$e = \frac{c}{a}$$, or the numeric eccentricity

We can also see that: $$a^2 = b^2 + c^2$$, which comes in handy.

Calculating the distance from the Sun in perihelion and aphelion is:$$A = a-c, \;\;P = a+c$$ and we can describe c with eccentricity:$$A = a-ae, \;\;P = a+ae$$ and the final expressions are:
- f $$A = a(1-e), \;\;P = a(1+e)$$

Finally, the area of an ellipse is$$P = ab\pi$$ (this can be proven, but with some integrals so we're not going to get into it here)

We have the semi-major axis, or *a*, and the semi-minor axis, b. Connecting them with the Pythagorean theorem, we get that$$a^2 + b^2 = c^2$$
So, the distance from the center of the ellipse to one of the focci, is equal to c.
- eg We define **eccentricity**, *e*, as: $$e = \frac{c}{a}$$, or as the focus distance divided by the semi-major axis. 

From this relationship, we can derive that:
$$\begin{aligned}
c = e*a \\
a^2 = b^2 - c^2 \\
b^2 = a^2 - c^2 \\
b^2 = a^2 - e^2a^2 \\
b^2 = a^2(1-e^2) \\
\end{aligned}$$
- f $$b = a\sqrt{1-e^2}$$


- !! When it comes to the area of an ellipse, it is $\pi ab$, but the circumference of an ellipse is undefined!!!

- eg Another important thing about ellipses, is a theorem where if we connect 2 focci to one point on the ellipse, the tangent line's perpendicular line divides the connecting angle into 2 equal pieces: very important for later!

![[ellipse 3.png|300]]

A fun fact relating to ellipses and other orbits which we will talk about later, is that <mark style="background: #fefae0;">they are all a conic section, and the shape of each orbit depends on the eccentricity or the slope of the plane cutting the conic sections!</mark>

---
#### Defining r of an ellipse
Defining coordinates to use for plotting the path of an ellipse can be a challenge. A way we are familiar with is with the [[Cartesian coordinate system]], however, a more natural coordinate system for ellipses and generally rotating shapes is the [[Polar coordinate system]]. This is a system ([[Transformations of astronomical coordinates]]) where you have an angle which defines the $x$ coordinate in a way, and the distance from the origin. However, we can convert one into another super easily!

Firstly, let's think of a circle. We know that if we have a unit circle, that:$$x^2 + y^2 = r^2$$
However, for ellipses it is slightly different, since we don't have only $r$. Using the [[Distance formula]], and some useful properties of ellipses we can derive a general formula for coordinates of an ellipse.

![[ellipse 6.png|300]]
This is the setup.

$$
\begin{align}
b^2 = a^2 - c^2 \\
d_1 = \sqrt{(x-(-c))^2 + (y-0)^2} \\
d_1 = \sqrt{(x+c))^2 + y^2} \\
d_2 = \sqrt{(x-c))^2 + y^2} \\
d_1 + d_2 = 2a \\
\sqrt{(x+c))^2 + y^2} + \sqrt{(x-c))^2 + y^2} = 2a \\
\sqrt{(x+c))^2 + y^2} = 2a - \sqrt{(x-c))^2 + y^2} \\
(x+c))^2 + y^2 = 4a^2 - 4a\sqrt{(x-c))^2 + y^2} + (x-c))^2 + y^2 \\
a \; bit \; of \; algebra... \\
4cx - 4a^2 = -4a\sqrt{(x-c))^2 + y^2} \\
a^2 - cx = a\sqrt{(x-c))^2 + y^2} \\
a^4 - 2a^cx +c^2x^2 = a^2((x-c))^2 + y^2) \\
a \; bit \; of \; algebra... \\
a^2x^2 - c^2x^2 + a^2y^2 = a^4 - a^2c^2 \\
x(a^2-c^2)+a^2y^2 = a^2(a^2-c^2) \\
b^2x^2 + a^2y^2 = a^2b^2 \\
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1 \\
done!
\end{align}
$$

Alrighty! Now that we have an equation which takes in the semi-major and minor axis and converts them into cartesian coordinates, it is time to convert these into polar coordinates!

First, we need to move the ellipse, or center the ellipse to one of its foccii, which is simply done by adding $c$ to the $x$ coordinate. Using basic elliptical properties ([[Kepler's first law - the law of ellipses]]) and some [[Fundamental trigonometry]], we can easily derive a formula. 
- !! A very important fact we use is that we can literally convert from $r$ into $x,y$ by using some trig: $$x = r\;cos\theta, y=r\;sin\theta$$

$$
\begin{align}
\frac{(x+c)^2}{a^2}+\frac{y^2}{b^2}=1 \\
\frac{(x+ae)^2}{a^2}+\frac{y^2}{a^2 - a^2e^2}=1 \\
\frac{(x+ae)^2}{a^2}+\frac{y^2}{a^2(1-e^2)}=1 \\
(x+ae)^2(1-e^2) + y^2 = a^2(1-e^2) \\
(r\;cos\theta+ae)^2(1-e^2) + r^2sin^2\theta = a^2(1-e^2) \\
r^2cos^\theta + 2aer\;cos\theta + 2a^2e^2 - r^2r^2cos^2\theta - 2ae^3r\;cos\theta - a^2e^4 + r^2sin^2\theta = a^2 - a^2e^2 \\
r^2(cos^2\theta + sin^2\theta)+2aer\;cos\theta + 2a^2e^2 - e^2r^2cos^2\theta - 2ae^3\;cos\theta - a^2e^4 = a^2 \\
r^2 = a^2-2aer\;cos\theta-2a^2e^2+e^2r^2cos^2\theta + 2ae^3r\;cos\theta + a^2e^4 \\
r^2 = ((a-er\;cos\theta)-ae^2)^2 \\
r = (a-er\;cos\theta)-ae^2 \\
r+er\;cos\theta = a-ae^2 \\
r(1+e\;cos\theta) = a(1-e^2)\\
r = \frac{a(1-e^2)}{1+e\;cos\theta}\\
done!
\end{align}
$$

- f $$r = \frac{a(1-e^2)}{1+ e \cos\theta}$$

And that's it! The correct way to define the path of an ellipse using polar coordinates by using the semi-major axis, eccentricity and theta! This equation is also used to describe an ellipse as a [[Conic sections]]. 

# But, how did we get to here?
---
How can we generalize this and make Kepler's laws seem like they came out of something that isn't thin air? 

We have 2 points of mass (the Sun and a planet), and they are orbiting a **centre of mass**. Here is a [[Cartesian coordinate system]] which shows how an orbit as such works:
![[centre of mass cartesian.png]]
$m_1$ is one body, $m_2$ is the second body, and $M$ is the centre of mass. The vector difference between $\vec{r_1}$ and $\vec{r_2}$ is: $$\vec{r} = \vec{r_2} - \vec{r_1}$$ $R$ is the *weighted average of the position vectors of the individual masses*, since its length and orientation depend on the masses! $$\vec{R} = \frac{m_1\vec{r_1} + m_2\vec{r_2}}{m_1 + m_2}$$, which we can generalize for any number of **n** objects:$$\vec{R} = \frac{\sum^m_{i=1} m_i\vec{r_i}}{\sum^n_{i=1} m_i}$$, and if we rewrite it, we get that:$$\vec{R}\sum^n_{i=1} m_i = \sum^m_{i=1} m_i\vec{r_i}$$
And let's say that $M$ is the total mass of the system, or the sum of all masses, then:$$\vec{R}M = \sum^m_{i=1} m_i\vec{r_i}$$
**If we differentiate this expression by time, we can extrapolate this to [[Velocity]]**. $$M\vec{V} = \sum^m_{i=1} m_i\vec{v_i}$$
We can now define this as the sum of all momenta, and then differentiate **again** by time, and we would get that the force is change in momentum over time. However, because of [[Newtonian mechanics]] and his third law, the total force is 0! $$F = \frac{d\vec{P}}{dt} = M\frac{d^2\vec{R}}{dt^2} = 0$$This means that we can simplify every orbit problem so that the centre of mass at rest is at $\vec{R} = 0$. We can simplify any binary orbit or 2 body problem:$$0 = \frac{m_1\vec{r_1} + m_2\vec{r_2}}{m_1 + m_2}$$
We can define a new property, **the reduced mass of the object** to be:$$\mu = \frac{m_1m_2}{m_1+m_2}$$, and now$$\vec{r_1} = -\frac{\mu}{m_1}\vec{r}$$$$\vec{r_2} = \frac{\mu}{m_2}\vec{r}$$
We can use the reduced mass for many things, including simplifying [[Energy in orbits]] with:$$E = \frac{1}{2}\mu v^2 - G\frac{M\mu}{r}$$, where $r = |\vec{r_2} - \vec{r_2}|$, and $v = d\vec{r}/dt$. The total [[Angular momentum]] can also be simplified as:$$\vec{L} = \mu \vec{r} × v = \vec{r} × \vec{p}$$, where $p$ is the reduced mass times velocity. 

---
If we use the knowledge gathered from this, we can investigate Kepler's laws in more detail! In tackling the first law, let's take a closer look at the momentum and differentiate it ([[Derivatives]]). $$\frac{d\vec{L}}{dt} = \frac{d\vec{r}}{dt} × \vec{p} \;+\;r ×\frac{d\vec{p}}{dt} = \vec{v} × \vec{p} + \vec{r} × \vec{F}$$, and we can notice that all of these products are 0 since they are **in the same direction**, and well the sine of 0 is 0. So, we have discovered that:
- !! **The angular momentum of a system is constant for a central force law! - The angular momentum in an orbit is conserved.**

Doing a lot of complicated math with lots of advanced vectors yields:
- f $$r = \frac{L^2/\mu^2}{GM(1+e\cos \theta)}$$
Or,
- f $$L = \mu \sqrt{GMa(1-e^2)}$$


 
 
