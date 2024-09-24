---
tags:
  - energy
  - physics
  - orbits
  - motion
  - planet
  - astronomy
  - mathematics
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

- !! It is important to note that **for ellipses**, energy is always **negative**, for a **parabola**, it is always **zero**, and for **hyperbolae** it is **always positive** ([[Conic sections]])

