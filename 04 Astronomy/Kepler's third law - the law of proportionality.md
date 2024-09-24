---
tags:
  - astronomy
  - motion
  - orbits
  - mathematics
  - physics
  - planet
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

## Another way to look at it...
---
Other than this proof via Newton's law of gravity, we can revisit [[Kepler's second law - the law of areas]] and use it to prove Kepler's third law. We consequentially use every preceding law to prove the next. Let's revisit the concept of [[Angular momentum]] from [[Kepler's first law - the law of ellipses]]. We know that the rate of change of angular momentum based on the reduced mass is:$$\frac{dA}{dt} = \frac{L}{2\mu}$$, and if we integrate that, we get:$$A = \frac{1}{2}\frac{L}{\mu} P$$, where $P$ is the period. (This seems fairly obvious). Now, we know that $A = ab\pi$, and we know what $L$ is equal to. However, let's square the equation first, and during the process it will be obvious which mathematical trick we will use:$$ab\pi = \frac{1}{2}\frac{L}{\mu} P$$ Rearanging:$$P = \frac{2ab\pi \mu}{L}$$, and squaring things:$$P^2 = \frac{4a^2b^2\pi^2 \mu^2}{L^2}$$, and now, we know what $L$ is equal to, especially to $L^2$:$$P^2 = \frac{4a^2b^2\pi^2 \mu^2}{\mu^2 GMa(1-e^2)}$$, and now the $\mu^2$ cancel out! Now, let's think about $b$. From the first law and properties of an ellipse, we saw that $b = a\sqrt{1-e^2}$. If we square that, we get:$$P^2 = \frac{4a^2(a^2(1-e^2))\pi^2}{GMa(1-e^2)}$$
Canceling out things and rearanging, we finally get:
- f $$P^2 = \frac{4\pi^2}{G(m_1+m_2)} a^3$$

