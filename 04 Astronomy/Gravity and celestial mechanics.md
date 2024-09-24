---
tags:
  - physics
  - astronomy
  - mathematics
  - planet
  - motion
  - orbits
---
While we all know the universe contains 4 forces, the electromagnetic, weak, strong nuclear force and gravity, we readily see the effects of only the electromagnetic force and gravity. When it comes to the motions of the planets, we study gravity and its impact on the celestial bodies. 

# Newtonian mechanics
---


### Digression! Vectors!
---
Before we move on, it is important to note that we divide physical quantities into **vectors** and **scalars**. <mark style="background: #eaf2e3;">Scalars</mark> like temperature, mass, length, etc. are one-dimensional, since they have only a value like 27ºC, 56kg, 10cm, etc. <mark style="background: #f2e863;">Vectors</mark> are 2-dimensional, since they contain within them both *magnitude* (their actual value) and **direction**. Vectors are extremely useful for physics, since forces, velocity, acceleration, and lots of other quantities (fields) are represented with **vectors**, and not scalars. 

![[vector.jpeg]]

#### Addition of vectors
Since vectors are slightly different from scalars, we add them and subtract them, multiply them with special *geometrical* methods. 

![[vector addition.jpeg]]

- n We denote the magnitude of a vector like so:$$|\vec{a}|$$

So, the actual value of adding two vectors together requires a bit of [[Fundamental trigonometry]], where we look at the positions of the 2 vectors and using the **cosine law**, we can calculate the value of addition:
- f $$|\vec{a}| + |\vec{b}| = \sqrt{|\vec{a}|^2 + |\vec{b}|^2 - 2|\vec{a}||\vec{b}|cos\;\theta}$$

Subtracting is the same process as addition, however you **flip the b vector** so that its magnitude stays the same, but orientation is 180º different direction so it has a minus and then you add them together since + (-) is the same as -.

#### Multiplication of vectors
There are 2 different kinds of multiplication. There is the dot product which is essentially trying to see the *amount of each vector projected onto the other vector.*
![[product 1 vectors.jpeg]]

So here, the amount of $\vec{b}$ projected onto $\vec{a}$ is $cos\;\theta*|\vec{b}|$. Hence the amount projected is:$$\frac{|\vec{a}||\vec{b}|}{|\vec{a}|} = cos\;\theta*|\vec{b}|$$ so:
- f $$\vec{a}\;\vec{b} = |\vec{a}||\vec{b}|cos\;\theta$$

We also have the cross product, whose resulting vector is directly perpendicular to the 2 vectors and is equal to the area of the parallelogram they produce.

![[cross product vectors.jpeg]]

### Back to the 2nd law
---
Now that we know what vectors are, we can continue with seeing how the second law of motion really manifests. From now on, I will use [[Derivatives]] for explaining and proving everything, but all information will be provided in another script where derivatives and integrals are intuitively explained. 



## The universal law of gravitation
---
And now for the fun part. Newton thought about the Moon and apples, and he came up with a universal law of gravitation which is used extremely often in celestial mechanics because, well, everything is affected by gravity or well the gravitational field produced by every object with mass. 

- f $$F_g = G\frac{Mm}{r^2}$$

And with this law, he makes 2 extremely important assumptions (which can be proven, but its too complex for now):
1. The gravitational field created outside a spherically symmetric body is the same as if it were a point mass of the same mass placed at the centre. 
2. We can consider a surface such that only the mass inside it contributes to the gravitational field, while mass outside gives a net zero contribution. 

The first point allows us to say that the gravitational impact of a planet or star or rocket (a bit of a stretch but it still works) can be placed at its **centre of mass**. 

We can measure the strength of a gravitational field with the **gravitational acceleration**, where we coincide the weight of an object (the effect of the field) with the universal law:$$mg = G\frac{Mm}{r^2}$$
- f $$g = G\frac{M}{r^2}$$, and for Earth its value is 9.81 m/s2

# Circular motion
---
Now, planets are spherical, and they all *orbit* the Sun, right? A circle is the most basic and elementary form of *orbiting*, so we'll start off with some circular motion which will help us understand ellipses and more.

#### Drawing a circle
First, we need a circle to begin with. We can centre it in a coordinate system, where the Sun can be in the origin point. Let's imagine a cute little planet orbiting the Sun in a perfectly circular path. 

![[drawing a circle.jpeg]]

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

# Kepler's laws
---
Now that we know how circular motion looks like, we can apply the same principles onto more complex shapes, like the ellipse. Why ellipses? Well, a certain Johannes Kepler postulated 3 laws of planetary motion, where he changed celestial mechanics forever. From the notion of circles to ellipses.

### 1st law of planetary motion
---
> All planets move in elliptical orbits, with the Sun at one focus.

So, he said that instead of circles, planet's move in ellipses. But how did he discover that? He compared angles of the planet's as they traveled from one point to another, after an equal time interval. If the angles were the same, the path would be circular, <mark style="background: #f2cd60;">but they weren't</mark>! And so, planetary orbits are ellipses after all. 

![[basics of ellipse.jpeg]]

Using the ellipse above, let's define some properties which are super useful for elementary orbital mechanics. 

All ellipses have 2 focci: in the case of planets, they orbit around one focus, [[The Sun]]. The 2 most famous positions are **aphelion** - the point closest to the Sun, and **perihelion** - the point farthest from the Sun. 

The *semi-major axis*, $a$ is the distance from the centre of the ellipse to either the perihelion or aphelion. It is kind of like the "average" distance of the planet from the Sun. $b$ is the semi-minor axis, and $c$ is the distance from the centre to the Sun. We use $c$ and $a$ to define **eccentricity**, a quantity which tells us how elliptical an orbit is.
- f $$e = \frac{c}{a}$$, or the numeric eccentricity

We can also see that: $$a^2 = b^2 + c^2$$, which comes in handy.

Calculating the distance from the Sun in perihelion and aphelion is:$$A = a-c, \;\;P = a+c$$ and we can describe c with eccentricity:$$A = a-ae, \;\;P = a+ae$$ and the final expressions are:
- f $$A = a(1-e), \;\;P = a(1+e)$$

Finally, the area of an ellipse is$$P = ab\pi$$ (this can be proven, but with some integrals so we're not going to get into it here)
#### Defining r of an ellipse
Defining coordinates to use for plotting the path of an ellipse can be a challenge. A way we are familiar with is with the [[Cartesian coordinate system]], however, a more natural coordinate system for ellipses and generally rotating shapes is the [[Polar coordinate system]]. This is a system ([[Transformations of astronomical coordinates]]) where you have an angle which defines the $x$ coordinate in a way, and the distance from the origin. However, we can convert one into another super easily!

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

### 2nd law of planetary motion
---
> The radius vector joining any planet to the Sun sweeps out equal areas in equal times.

This basically translates to the fact that speed is **not** constant around an ellipse, and that if we are closer to the Sun we revolve faster than if we were further away. 

Here we introduce a new quantity, **angular momentum**. Remember regular momentum? It is like the "amount of motion", however in this case, this amount of motion is also rotating around some point, in this case around the Sun. We know that:$$\vec{p} = m\vec{v}$$
![[angular momentum ellipse.jpeg]]

Since the radius vector and velocity are well, vectors, the angular momentum is regular momentum multiplied by the radius:
- f $$\vec{L} = m\;\vec{v}\;×\vec{r}$$

Remembering properties about vectors, we can see that we have a **cross product**, which accounts for the area these 2 vectors produce. Looking at the ellipse (picture on the right) we can see that r changes with respect to $\theta$, and the velocity is not always perpendicular to the radius. Magnitude wise, angular momentum is equal to:
- f $$L = mvr\;sin\;\theta$$

> The second law of planetary motion states that angular momentum **is always constant in an orbit**.

This is a huge takeaway! It means we can compare any 2 points on the ellipse and calculate other properties.

And in the case of **perihelion and aphelion**, the only 2 points where velocity is 90º agains the radius, $sin\;90º = 1$, and so $$\begin{align} L_a = L_p \\ mv_a\;r_a\;sin\;90º = mv_p\;r_p\;sin\;90º \\ v_a\;r_a = v_p\;r_p\end{align}$$
- f $$v_a\;r_a = v_p\;r_p$$, for aphelion and perihelion.

### 3rd law of planetary motion
---
> The square of the orbital period of any planet is directly proportional to the cube of the semi-major axis of its orbit. 

This is a very concrete law that is easy to prove, at least for circular orbits. In order to prove this statement for elliptical orbits, it requires integrals and calculus, which I will not be diving into at the moment. (it is connected to angular momentum and the second law) 

#### Digression: the first cosmic speed
Before we can get into the proof of this law at least for circular orbits, we need to think about the velocity of an object **orbiting a body.** We will only consider a circular orbit. 

If we launch a satelite from Earth and want it to orbit it from a height, $h$, (which we will say that $R = r+h$, where $r$ is the radius of the Earth), it is interacting with the gravitational field of the Earth. The Earth and the satelite are exerting an equal and opposite force on one another. However, the satelite also has to orbit the Earth, requiring centripetal force. One can conclude that then:$$F_{cp} = F_g$$
We can then substitute our values inside:$$\frac{mv^2}{R} = G\frac{Mm}{R^2}$$
And after some algebraic fixing:
- f $$v = \sqrt{G\frac{M}{R}}$$

#### Back to the proof
Now, we can say that a planet is orbiting on a circular path a distance $a$ from the Sun. Its velocity is then:$$v = \sqrt{\frac{GM}{a}}$$
But, since it is a circle and velocity is constant, it is also equal to the circumference divided by the period of orbit. Hence:$$\frac{2\pi\;a}{T} = \sqrt{\frac{GM}{a}}$$ We can now square the terms: $$\frac{4\pi^2\;a^2}{T^2} = \frac{GM}{a}$$
With some algebraic manipulation, we get the following:
- f $$\frac{T^2}{a^3} = \frac{4\pi^2}{GM}$$

# Energy of orbit
---
We have looked at velocities, accelerations and covered the three fundamental laws of planetary motion. Another extremely important aspect of orbits is the **energy of an orbit.** 

- !! Warning! This section will contain integrals for the proofs of every equation, as the integrals are in themselves very easy to understand. I will provide a general intuition about integrals to make the process easier.

We divide energy into 2 categories: <mark style="background: #f2e863;">kinetic energy</mark> and <mark style="background: #61e8e1;">potential energy</mark>. **Kinetic energy** is the work done by a force in order to increase the velocity of a body from 0 to some velocity $v$. Basically, it is the energy of movement. We define it as:$$\Delta K = \Delta W$$
- n It is important to note that we define energy as the **change in energy**, and not as a definite quantity.

 **Potential energy** is slightly more complex, but easy to understand. Imagine 2 bodies a distance $r$ away from each other. We want to bring body $Q_2$ to body $Q_1$, from infinity, at a constant velocity (so that we isolate potential from kinetic energy) . This means that it is the *work done by a force to bring one body a distance $r$ from the other body.* Since our reference point is infinity, the sign of potential energy **is always a minus.**  ![[electric potential energy.jpeg]]
$$\Delta U = -\Delta W$$
The total energy of any body, but in our case orbiting bodies, is the sum of all of their kinetic and potential energy:$$\Delta E = \Delta K - \Delta U$$
### Kinetic energy
---
Let's first derive the formula for kinetic energy. We know that work is defined as:$$W = F\;x$$, where F is a force and x is the distance covered. **An Integral** is a tool in calculus used to calculate the **area under a curve**. More intuitively, we can track infinitesimally small changes we describe with derivatives and sum them on an infinite scale to gain a whole body again. For example, we divide a circle into an infinite amount of co-centric rings, and integrating each of their areas brings back the area of a circle. 

In this situation, we are taking infinitesimally small steps with a force F (since there is acceleration, a change in velocity from o to $v$), and then we are integrating in order to get $W$. $$\Delta W = \int F\;dx = \int ma\;dx = \int_0^v m\frac{dv'}{dt}v'\;dt = \int_0^v mv'dv' = [\frac{1}{2}mv'^2]_0^v = (\frac{1}{2}mv^2 - 0) = \frac{1}{2}mv^2$$
What did we do here? We defined an integral of F over small increments of space, $dx$. We then rewrote F as $ma$, via Newton's second law of motion. We then realized that we could express acceleration as the *change in velocity over time*, denoting it with $v'$ to differentiate from the limit, $v$. We integrate over a range form 0 velocity to our desired velocity $v$, which are the limits. We also realized that we could express our **infinitesimally small change in space as the velocity times an infinitesimally small increment of time**. Next, we see that $dt$ and $dt$ cancel out, and we remain with only $mv'\;dv'$. 

Now, here comes the hard part. We need to **reverse engineer the integral**, and find some function, $f$, which when derived, would give $mv'dv'$. Knowing the [[Power rule]] in calculus:$$ \frac{d}{dx}ax^n = an\;x^n-1$$ we reverse engineer and realize that if we multiply by half and square we get no exponent for $v'$ and no constant in front. The final step is using the **fundamental theorem of calculus** which states that you can just subtract the value of this **antiderivative** at the upper limit and subtract from the bottom limit. This gives us the final equation:
- f $$K = \frac{1}{2}mv^2$$

### Gravitational potential energy
---
We apply similar reasoning for the gravitational potential energy, using the same integral principles by integrating the work over an infinitesimally small increment of space, but instead of Newton's second law, we use the law of gravitation (since we are dealing with gravitational energy). $$\Delta W_g = -\int_{\infty}^r F_g\;dx = -\int_{\infty}^r \frac{GMm}{x^2}\;dx = -GMm\int_{\infty}^r \frac{dx}{x^2} = -GMm[-\frac{1}{x}]_r^{\infty} = -GMm(0 + \frac{1}{r})$$
And the final form is:
- f $$U = -\frac{GMm}{r}$$

### Summing the energies
---
Now that we know the kinetic and potential energy of a body in orbit, we know that:$$E = \frac{1}{2}mv^2 - \frac{GMm}{r}$$
By looking at the energy of an orbit, we realize that there actually exist 4 types of orbits:
1. Circular: $E$ is minimal, the smallest value it can be
2. Elliptical: $E < 0$
3. Parabolic: $E=0$
4. Hyperbolic: $E > 0$

When it comes to planets, the orbit of a planet is elliptical, but orbits of comets can be parabolic or hyperbolic (special mathematical functions). 

## Closed orbits
---
**Closed orbits** are orbits where a body periodically rotates around a centre of attraction, so basically any body orbiting another in a system. They can either be circular or elliptical. First, we'll look at the circular case, which if you replace $R$ with $a$ are equivalent. 

So, we know that the potential energy in a circular system is constant, and we know the velocity of an orbiting body. Pluging that into the kinetic energy equation:$$K = \frac{1}{2}mv^2 = \frac{1}{2}m\frac{GM}{R} = \frac{GMm}{2R}$$
And we also know the total energy of the system is the sum of its potential and kinetic energy:$$E = K + U = \frac{GMm}{2R} - \frac{GMm}{R}$$, and so:
- f $$E = -\frac{GMm}{2R}$$, and for elliptical orbits:$$E = -\frac{GMm}{2a}$$

### The escape velocity
---
The final important aspect of energy is the **second cosmic speed** or the **escape velocity**. It is the velocity needed to escape the gravitational pull of a body and go of into infinity. It is super simple to set up, since energy is always conserved:$$K + U = K' + U'$$$$\frac{1}{2}mv^2 - \frac{GMm}{R} = \frac{1}{2}mv'^2 - \frac{GMm}{R'}$$
Now, we want our object to stop at some point in infinity, so $v' = 0$. And also, since $R \ce{->} \infty$, then the fraction also approaches 0, or well is 0 for our intents and purposes. So:$$\frac{1}{2}mv^2 - \frac{GMm}{R} = 0$$ $$\frac{1}{2}mv^2 = \frac{GMm}{R}$$
And we get that:
- f $$v = \sqrt{\frac{2GM}{R}}$$


# Motion of the planets
---
Now that we understand **why and how** planets move, let's take a look at how we can put things into perspective for Earth and how planets move with respect to the Earth. 

We distinguish 2 types of planets: **inferior and superior**. Inferior are the ones before Earth, and superior the ones after. All of the planetary positions are denoted in the image below:
![[planetary positions.jpeg]]
#### Inferior planets
They are Mercury and Venus, and they move really close to the Sun, however never exceeding their **maximum elongation.** The angle E2S (the sun is point S) is a right angle, hence the maximum elongation can never exceed:
- f $$\epsilon_{max} = \frac{d}{d_s}$$, where $d$ is the distance from the planet to the Sun, and $d_s$ Earth-Sun distance.

- n For Venus, the values range from 45º to 48º, and for Mercury from 18º to 28º. 

The motion of the inferior planets is described as such:
1. At point of maximum eastern elongation, it is visible shortly after sunset.
2. The Sun sets earlier than the planet, making it visible during twilight. 
3. At point of inferior conjunction it is directly in line with the Sun, and a **transit** might occur. 
4. It then moves retrogradely to the west, and is visible just before dawn.
5. It appears to be stationary at its western maximum point.
6. It then reverses motion, faster and faster reaching the Sun.
7. At upper conjunction it disappears behind the Sun.
8. The cycle continues.

#### Superior planets
These are Mars, Jupiter, Saturn, Uranus and Neptune, and they are more free to move, and can reach a maximum elongation of any value. Here is the motion of these planets:
1. In conjunction they are barely visible as they rise and set with the Sun.
2. They move until the point of eastern quadrature and stay there.
3. it then moves away, faster and faster until opposition, when it is best seen.
4. it moves again until western quadrature, and appears stationary. 
5. The cycle repeats.


## Periods of orbiting
---
We differentiate 2 different kinds of periods, just like in [[Time systems]]. We have the **synodic period** - interval of time between 2 successive conjunctions/oppositions of a planet. We also have the **sidereal period** or the interval of one complete orbit around the Sun. 

Looking at the angular velocities of the planets, the angular velocity of inferior planets is larger than the Earth, hence:$$\omega_{diff} = \omega_{planet} - \omega_e$$

For superior planets, the Earth's angular velocity is bigger, and so:$$\omega_r = \omega_e - \omega_p$$
Since the numerator of each fraction is the same, we get the final equations:

- f For **inferior planets**: $$\frac{1}{S} = \frac{1}{T} - \frac{1}{A}$$, and for the **superior planets**: $$\frac{1}{S} = \frac{1}{A} - \frac{1}{T}$$

### Phase of a planet
---
An interesting property of the planets and [[Light]] is the **phase of a planet**, which we can observe in eg. [[Venus]] and the [[Moon]]. And we can use some simple geometry and [[Fundamental trigonometry]] to get to the answer. 
![[phase of planet.png]]
From the position of [[The Sun]], the light part of the photo is visible, but from the [[Earth]]'s perspective, only above line CD is everything visible, meaning that PBD is going to be dark - the phase of the planet. 

So, the phase of a planet is really:$$phase = \frac{CF}{CD} = \frac{CP + PF}{CD}$$ and using some trigonometry, 
- !! $$phase = \frac{CP + cos\;\phi\;CP}{2CP} = \frac{1}{2}(1+cos\;\phi)$$

--- 
However, we want to find the phase of the planet depending on its position around the Sun. For that, we need the angle theta in the drawing above to see what's what. Using the sine formula:$$\frac{SE}{sin\;\phi} = \frac{SP}{sin\;(180-(\theta+\phi))}$$ So we can get that:$$SP\;sin\;\phi = SE\;sin\;(\theta+\phi)$$ where we can use the fact that the tangent is equal to the sine over cosine, we can get:$$tan\;\phi = \frac{SP\;sin\;\theta}{SE - SP\;cos\;\theta}$$ and we can calculate theta by:$$\theta = 360 \frac{t}{S}$$, where $t$ is the time which has passed since the beginning of the cycle, an $S$ is the *synodic period*

# Motion of binary stars
---
The final component of celestial mechanics is the understanding of **binary star systems**. They are systems where 2 stars orbit each other around a **common centre of mass**. 

![[binary system.jpeg]]

The 2 stars orbit in a straight line connecting the 2 stars, meaning that **they have the same period of orbiting**. In this case, $a$ is the distance between them:$$a = r_1+r_2$$
And since they orbit along a straight line:
- f $$m_1\;r_1 = m_2\;r_2$$

#### Kepler's third law with binary stars
Now, we can apply Kepler's third law with binary stars as well! Let's go through this step by step.
First, we know that the 2 stars exhibit a force of gravity, in equal magnitude one upon the other.$$F_{g, 1} = F_{g, 2} = \frac{Gm_1m_2}{(r_1+r_2)^2}$$
Now, in order for them to stay in a, well, circular orbit (I know they don't orbit in circles, but we are oversimplifying everything), and so their centripetal forces have to have a constant magnitude, and since they are orbiting in a straight line, ==their angular velocities must stay the same as well!== $$F_{c, 1} = m_1\omega^2\;r_1, \;\;\;F_{c,2} = m_2\omega^2\;r_2$$
And we also know that the centripetal force and force of gravity are equal in orbits:$$\begin{align} \frac{Gm_1}{(r_1+r_2)^2} = \omega^2\;r_1 \\  \frac{Gm_2}{(r_1+r_2)^2} = \omega^2\;r_2\end{align}$$
Adding the  equations together yields the following result:$$\frac{G(m_1+m_2)}{(r_1+r_2)^2} = \omega^2\;(r_1+r_2)$$
And, knowing the definition of $a$, we can substitute that in our equation. Finally, since $\omega = 2\pi / T$, we get that:
- f $$T^2 = \frac{4\pi^2}{G(m_1+m_2)}a^3$$

Great! Now, it turns out that this equation also works for elliptical orbits, except in this case, $a$ is defined as the sum of the semi-major axes $a_1$ and $a_2$, and not the total distance between them. 

### The Doppler shift and binary stars
---
We can discover binary stars in multiple ways, and one of them is with [[The Doppler effect]], where the shift in wavelengths of light can be seen due to the gravitational tug of each star. 
![[binary star radial motion.png]]
We can see that the tangential velocity is always constant, but the **radial velocity** due to the effect of the Doppler shift is constantly changing due to the angle, $\theta = \omega \;t$. And so, with trig, we get:
- f $$v = v_r \;cos\;\omega t \ce{->} z = \frac{\Delta \lambda}{\lambda_0} = \frac{v_r}{c} cos\;\omega t$$




