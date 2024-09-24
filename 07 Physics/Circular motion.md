---
tags:
  - circles
  - motion
  - physics
  - astronomy
  - orbits
  - mathematics
---

Now, planets are spherical, and they all *orbit* the Sun, right? A circle is the most basic and elementary form of *orbiting*, so we'll start off with some circular motion which will help us understand ellipses and more.

#### Drawing a circle
First, we need a circle to begin with. We can centre it in a coordinate system, where the Sun can be in the origin point. Let's imagine a cute little planet orbiting the Sun in a perfectly circular path. 

![[drawing a circle.jpeg|300]]

Now, the radius is also a vector, which we can define with its x and y components, and **unit vectors**, which just give a notion of direction and have no real value (well, the value of 1). So, -
- f $$\vec{r} = r_x\vec{i} + r_y\vec{i}$$, where $$r_x = r\;cos\;\theta, \;\;r_y = r\;sin\;\theta$$


#### Velocities around the circle
We can track the orbit of our little planet with its **angular velocity**:
- f $$\omega = \frac{360º}{T} = \frac{2\pi}{T}$$

Even though r is constant, it is still a function of time, as the angle $\theta$ depends on the angular speed and time:$$\theta = \omega\;t$$

So, we can rewrite $r$ as:
- f $$r = (r\;cos\;\omega t)\vec{i} \;+ \;(r\;sin\;\omega t)\vec{j}$$


We also have **tangential velocity**, which is <mark style="background: #f2cd60;">perpendicular to the path of motion.</mark> We can prove this statement actually, but it requires lots of math, and isn't instrumental to understanding. (I can provide the proof if somebody is super interested). 

However, what is instrumental is the fact that if it is tangential, we can divide it into its x and y components! And since it is a right triangle, we can use the pythagorean theorem to get to the tangential velocity. 

So, our velocity can be divided into its $v_x$ and $v_y$ components. Let's first tackle the x component.
We can write velocity as *a change in x-position over time*, like so:$$v_x = \frac{dr_x}{dt}$$
We know what the value of $r_x$ is, so let's substitute it in:$$v_x = \frac{d}{dt}(r\;cos\;\omega t)$$
Now, we can separate this derivative into **2 derivatives**, where we first track the change in position over the **angle**, and then the *change in that angle over time*, like so:$$v_x = \frac{d(r\;cos\;\omega t)}{d\omega t} * \frac{d\omega t}{dt}$$
Now we have 2 derivatives which we can solve separately and then combine them together again. Since r is constant, we can move it out of the first derivative, and knowing that the derivative of $d\;cos\;\theta = -sin\;\theta$, we get the following (the proof for why this is true is long, but it is in the calculus files): $$\frac{d(r\;cos\;\omega t)}{d\omega t} = r\frac{d}{dt}(cos\;\omega t) = -r\;sin\;\omega t$$
And now, with the second component, it is very simple, as the change in the angle is equal to the angular velocity (intuitive on its own):$$\frac{d}{dt}\;\omega t = \omega$$
Combining the two together, we get:
- f $$v_x = -r\;\omega\;sin\;\omega t$$

Now we repeat the exact same process just for $v_y = \frac{dr_y}{dt}$, where now instead of $cos$ we have $sin$, where the $d\;sin\;\theta = cos\;\theta$: 
- f $$v_y = r\;\omega\;cos\;\omega t$$

Now that we know how to express the components, let's put them together to form the final expression for the tangential velocity:$$\begin{align}v = \sqrt{v_x^2 + v_y^2} \\ v = \sqrt{(-r\;\omega\;sin\;\omega t)^2 + (r\;\omega\;cos\;\omega t)^2} \\ v = \sqrt{r^2\omega^2\;((-sin\;\omega t)^2 + (cos\;\omega t)^2)} \\ v = 
\sqrt{r^2\omega^2}
\end{align}$$
We got rid of the sin and cos terms due to the Pythagorean identity of trigonometry, where the square of sin and square of cosine give 1. And we have the final formula:
- f $$v = r\;\omega$$

#### The need for acceleration
Now, when an object is moving around a circle, it is **constantly changing direction** in order to keep its path around the circle. Which means that ==there must be a force keeping it from going off at its tangential velocity - **the centripetal force**==. And by Newton's second law: <mark style="background: #f2e863;">if there is a force, there is acceleration</mark>. This means that even though velocity is constant, there is acceleration keeping the body in motion. Let's figure out how to describe this quantitatively. 

We know that acceleration is the change in velocity over time. So, we can break up velocity into its x and y components (which we already did) and evaluate acceleration:$$\vec{a} = \frac{dv_x}{dt}\vec{i} \;+\;\frac{dv_y}{dt}\vec{j}$$, where $i$ and $j$ are unit vectors. 
Let's tackle each derivative separately. We already know what $v_x$ is, so let's plug it in:$$\frac{dv_x}{dt} = \frac{d}{dt}(-r\;\omega\;sin\;\omega t)$$ Again, we can split this into 2 derivatives to make the work much easier, first as a change in angle and then as that angle changes with time. $$\frac{d}{dt}(-r\;\omega\;sin\;\omega t) = \frac{d(-r\;\omega\;sin\;\omega t)}{d\;\omega t} * \frac{d\omega t}{dt}$$
By evaluating the first derivative, we can see that $r$ and $\omega$ are constant, so they don't change, while the derivative of the sine of the angle is equal to the cosine of that angle. Meanwhile, for the second derivative, the change in angle over time is the exact definition of angular velocity. So, our final formula is:
- f $$\frac{dv_x}{dt} = -r\omega^2\;cos\;\omega t$$

Analogous to this process, we get the derivative of the y component, which is exactly the same except for the cos and sin. We then get:
- f $$\frac{dv_y}{dt} = -r\omega^2\;sin\;\omega t$$

Putting these 2 together into our original formula:$$a = (-r\omega^2\;cos\;\omega t)\vec{i} + (-r\omega^2\;sin\;\omega t)\vec{j}$$
We have a constant term here, and we can take the minus out. But, let's leave $r$ in, even though it appears in both. Something interesting happens. $$a = -\omega^2[(r\;cos\;\omega t)\vec{i} + (r\;sin\;\omega t)\vec{j}]$$
We realize that the expression in the parentheses is the **exact definition of r** we wrote up previously! Substituting that in, we get:$$a = -\omega^2\;r$$
This tells us that acceleration is in colinear with position (obviously), and that it has the opposite direction (again, logical as it points towards the centre of the circle while r is pointing outwards). So, our final expression (magnitude wise) is:
- f $$a = r\;\omega^2$$

Now, we know the value of $\omega$ in terms of the tangential velocity. It is:$$\omega = \frac{v}{r}$$ So, if we plug that in:$$a = r\;\frac{v^2}{r^2}$$, and the final expression is:
- f $$a = \frac{v^2}{r}$$

Combining these with Newton's second law we get:
- f $$F_{cp} = \frac{mv^2}{r}$$
