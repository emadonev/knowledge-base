---
tags:
  - math
  - trigonometry
  - calculation
  - triangle
  - circles
---
# The basic 3 functions
---
Let's say we have a triangle with sides a, b, c and a right angle in point C. 
1. SINE (opposite over hypothenuse)
$$sin θ = \frac{b}{c}$$
2. COSINE (adjacent )
$$cos θ = \frac{a}{c}$$
3. TANGENT
$$sin θ = \frac{b}{a}$$

# Unit circle
---
However, other than representing sine, cosine and tangents as only the relationship of sides of a triangle, let's relate that to the [[Unit circle]].

![[unit circle trig.jpeg]]

A unit circle is a circle centered around the origin of a cartesian coordinate system. Its radius is 1, to make calculations simple (hence the name, *unit*). 

Let's imagine a point $T$ next to the unit circle, and an infinite number line is passing through point $T$. We pick a point $A$ on the number line, and it has some value. Now, let's say we want to map that point $A$ onto the circle. We map it to point $A'$, so that the arc length $a$ is equal to $|A|$. Now how do we define the position of this new point $A'$?

If we connect it to the origin of the unit circle, $O$, we realize its length $|OA| = 1$. It forms an angle $\theta$ with the x axis. 

We can define point $A'$ with its x and y coordinates. $x$ is the distance from $A'$s orthogonal projection onto the x-axis to the origin, while $y$ is the distance from $A'$ to its orthogonal projection to the x-axis. We can express these lengths in terms of sine and cosine:
- f $$x = cos\;\theta,\;\;y = sin\;\theta$$

>So, if we want to know the sine and cosine value of a particular number (angle in degrees or radians), they are the coordinate values of that value projected onto the unit circle.  

This is also why the following 2 statements are true:
- f $$sin(180º-\theta) = sin(\theta), \;\;cos(180º-\theta) = -cos(\theta)$$

They are true since if we look at the angle formed by $180º-\theta$ we get another angle $\theta$ in the blue dotted line in the picture! The height stays the same, but the x coordinate is the same with a flipped sign. These insights are necessary to understand the *sine and cosine law*, which come in extremely handy for lots of tough mathematical spots!

### Tangent on the unit circle
---
But what about the ==tangent==? We have mapped everything on the unit circle but the tangent! Where is it?
If we look at the unit circle from image (1), we can see that actually
$$tan(\theta) = \frac{y}{x}$$, where $x,y$ are coordinates ([[Cartesian coordinate system]]). 

- f However! We have just discovered one of the most important theorems in trigonometry! $$tan (\theta) = \frac{sin(\theta)}{cos(\theta)}$$
# Arch functions
---
But there are arch-versions of the trig functions! The ==cosecant, cotangent and secant!==
We can take the reciprocal of any function, as well as the trigonometric functions. 
![[all trig functions.png]]
- n All of these functions can be written as the reciprocals of the regular trigonometric functions!

If we want to calculate the ==degrees from the function values==, we can use the *arcsine, arcosine and arctangent* functions on the calculator (or use a [[Unit circle]]). If we take the cosine of arccosine, we just get the cosine! These are the ==inverse [[Functions]]== of trigonometry!

# The law of sines
---
But what if we don't have enough information about a triangle? What if we don't have enough sides? Thankfully, the law of sines comes in. We can divide every triangle into 2 parts by drawing a vertical line. 

![[sine law.jpeg|400]]

# Law of cosines
---

(proof in progress)
![[law of cosines.png]]

# Plotting sine and cosine
---
What if we wanted to represent sine and cosine and [[Functions]] on a graph? We could plot them on a [[Cartesian coordinate system]], and we would get something like this:
![[sine and cos graph.png]]
As we can see from the graphs, they are periodic, so they repeat periodically! 
For the function

$$f(\theta) = a \; sin(b(\theta - h)) + k$$
with positive values of $a$ and $b$:
- $a$stretches or compresses the graph vertically, affecting the **amplitude**.
- $b$ stretches or compresses the graph horizontally, affecting the **period** and **frequency**.  
- $h$ produces a horizontal shift, also known as a **phase shift**.
- $k$ produces a vertical shift, affecting the **midline**.

# Phase shift
---
This is when in our original function be it either sine or cosine, we add a number which shifts the number of complete cycles in trigonometric functions. 

Some important phase shift formulas to know:
$$sin(-x) = - sin(x)$$
$$cos(x) = cos(-x)$$
$$sin(x+\phi) = -sin(x), \; \phi=\pi$$
$$sin(x+\phi)= cos(x), \; \phi=\frac{\pi}{2}$$
#### Adding sine functions
----
- if we want to get 2 angles which are opposite from one another, all we need to add is π. 
- when adding sine functions together:
	- we can cancel the waves when the peaks align with the throughs
	- we can add the waves by summing their corresponding y axes
	- we can represent sound waves (and really any sine function) as:
	- eg $$y = A\:sin(\omega x)$$

## Other trigonometric graphs
---
![[cosecant.png]]
- the **cosecant**: trigonometrically inverse function of sine and cosine.
	- a unique feature are ==vertical asymptotes==, since at some points we divide by 0

![[secant.png]]
- this is the **secant**: it also has vertical asymptotes, has the same period as the cosecant and has no 0! (because of division)

#### Transformations of these functions
----
$$a \; sec(b(\theta - h)) = \frac{a}{cos(b(\theta-h))}$$
- a controls the amplitude, or the distance from the x axis of points
- b controls the frequency, or the period of the graph
- and h controls the x-axis shift, or the phase shift

The same equation works for cosectant!!
$$a\;csc(b(\theta-h)) = \frac{a}{sin(b(\theta-h))}$$
## Defining the tangent function
---
So, we all know that the ratio between sine and cosine is the tangent. 
![[tangent.png]]
Here are both the tangent (blue) and cotangent (red) plotted, with a period of π. 

We can describe the occurance of 0 value for cotagent, secant and cosecant by the following:
$$\frac{\pi}{2} + \pi k$$, here $k$ is an integer.

- !! IMPORTANT! Let's say we want to transform the tangent graph into the cotangent graph. The first thing we would need to do is flip the graph via the y axis, which is achieved by simply $-tan(\theta)$, since this creates a negative output. Then we need to shift the axis by $\frac{\pi}{2}$, since the 0th points aren't aligned. And so we have: $$g(\theta)= -tan(\theta - \frac{\pi}{2})$$







