---
tags:
  - physics
  - charge
  - mathematics
  - electricity
---

A long time ago, Charles Augustin de Coulomb went ahead and explored [[Electric charge]]s. He put them a certain distance away and calculated the force between them using a torsion balance (used later for the gravitational constant [[The universal law of gravitation]]). He discovered that the force is *remarkably similar to gravity*, in fact:
>$$F = k\frac{|q_1q_2|}{r^2}$$

Where $k$ is *a constant*, $q_1,q_2$ are the 2 charges (parallel to 2 masses) and $r^2$ is the square distance between them. Now, an interesting side question. Why do all forces (including now both $F_c$ and $F_g$) vary with $1/r^2$? 

---
Let's imagine for a moment that space is 2D. This would mean that if we have an object in a field, it would influence the field a certain way - it would **enact a force**. We can illustrate this with a dot, and little *lines*, which really *simulate the effect of a force on the field.*

Now, what we see is that the further we go from that dot, $r$ gets bigger, **and the density of lines is smaller**. This means that the strength of the force is proportional to the *amount of lines* divided by the *circumference of the circle of effect*. This gives us:$$F \propto \frac{N}{2\pi r}$$
Moving back to 3D. We have a dot, but this time **the space of influence is a *sphere***. This means that lines extend outwards from a point, equally in all directions. Again, the further away we are, $r$ is bigger and the line density is smaller. But this time, it is dependent on *the area of the sphere*:$$F \propto \frac{N}{4\pi r^2}$$
> And this is why there is always a $1/r^2$ proportionality constant. If we lived in 4D, it would be $1/r^3$, etc. 

---

Back to our force of choice, Coulomb's force for electric charges. Just like gravity, it acts between 2 objects (which we can approximate as points), along their line of sight, in *equal and opposite magnitude* ([[Principles of mechanics]]). 

What about the constant? It is obviously a proportionality constant, but it has a slightly deeper meaning. In its plain value, it is simply equal to:$$k = 8.988 * 10^9 Nm^2/C^2$$, where $C$ is 1 coulomb. The standard **electric charge** for an electron or proton is:$$e = 1.6022*10^{-19} C$$, which is *realllllyyyy small*. 

Now, when Coulomb's force, and generally in electrostatics, is acting in the field, **depending on the medium we are observing in our system**, the forces (just as the speed of light) is *different.* In order for us to measure the difference, we put in the *dielectric constant of a medium*. It is defined as:$$\epsilon_r = \frac{\epsilon}{\epsilon_0}$$, where $\epsilon_r$ is the *relative* constant used in equations since $\epsilon$ is actually ==unattainable==, and $\epsilon_0$ is important since it is the **dielectric constant for a *vacuum***, or simply ***the electric constant***. From this we get that:$$k = \frac{1}{4\pi \epsilon_0}$$, where $\epsilon_0 = 8.854*10^{-12} C^2/Nm^2$. 


---
Another interesting thing about the electric force is how **powerful it is.** When discussing the **4 fundamental forces of the universe**, it is always mentioned how *weak gravity is.* For example, what is the ratio of the electric force and the gravitational force between 2 [[Alpha decay]] particles?

![[electrovsgravity.png]]

$$\frac{F_e}{F_g} = \frac{\frac{g^2}{4\pi\epsilon_0 r^2}}{G\frac{m^2}{r^2}} = \frac{q^2}{4\pi\epsilon_0 G m^2} = 3.1 * 10^{35}$$
This is insane!!!! The electrostatic force is incomprehensibly stronger than gravity!!!

---

