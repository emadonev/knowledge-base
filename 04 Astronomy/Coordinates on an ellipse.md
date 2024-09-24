---
tags:
  - coordinate_systems
  - ellipse
  - orbits
  - physics
  - math
  - astronomy
  - planet
  - planetary_science
---
Defining coordinates to use for plotting the path of an ellipse can be a challenge. A way we are familiar with is with the [[Cartesian coordinate system]], however, a more natural coordinate system for ellipses and generally rotating shapes is the [[Polar coordinate system]]. However, we can convert one into another super easily!

Firstly, let's think of a circle. We know that if we have a unit circle, that:$$x^2 + y^2 = r^2$$
However, for ellipses it is slightly different, since we don't have only $r$. Using the [[Distance formula]], and some useful properties of ellipses we can derive a general formula for coordinates of an ellipse.

![[ellipse 6.png]]
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
And that's it! The correct way to define the path of an ellipse using polar coordinates by using the semi-major axis, eccentricity and theta!

