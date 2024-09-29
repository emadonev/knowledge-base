---
tags:
  - physics
  - electricity
  - charge
  - calculation
  - mathematics
---
As discussed in [[Coulomb's law]], 2 charged particles exert a *force* on each other. But what is **force really?** 

The weird thing about forces is that they kind of *act at a distance*. Its as if 2 object which are super far away somehow have an influence on each other. The further away they are, the influence is less (by the $1/r^2$ proportionality). How do we explain this?

A force is not really a force. At least not in the conventional sense. Its not really something acting on something else, but rather the *end result of a process, we mask the **effect of a ==field== with force***. 

A **field** is a part of space where every point has 2 quantities - magnitude and direction - a [[Vectors]] quantity. So, if we have an **electric field**, its a part of space where every point has some *charge value and the direction of that charge ==depending on if its + or -.==* If the field is empty (there are no charged objects in the field) then it only contains **tiny quantum fluctuations** where particles pop in and out of existence - since fields don't have 0 energy.

However, if we put a point charge in the field, **it will have an influence on space itself.** The points around the charge will gain a certain magnitude and direction. Now, if we put *another charge*, the underlying field will influence that charge, and that charge will influence the starting field, so ***a force is nothing more than the effect of the field on objects.*** We can measure the *strength* of fields by dividing this force by the starting charge, and we get for electric fields:

>$$\vec{E} = \frac{\vec{F_0}}{q_0} = \frac{q}{4\pi\epsilon_0 r^2}\vec{r}$$>, where $\vec{E}$ is the strength of the electric field, $\vec{F_0}$ is Coulomb's force and $q_0$ is the reference charge, and $\vec{r}$ is the unit vector for direction.

![[electric field.jpg]]

> If a point charge is positive, the vectors at every point in the field will point ==away== from the charge, while if it is negative, they will point ==towards== the charge.

Now, coming back to the fact that we are currently in the realm of **electrostatics** (not dynamics), a cardinal rule is that ***==the electric field at every point within the material of a conductor must be zero==*** - **no net motion!**

---

```
How do we calculate the unit vector?
```

Well, the $\vec{r}$ is composed of real **unit vectors of the x,y and z plane**, and they are $\vec{i}$, $\vec{j}$, and $\vec{k}$. So, the unit vector $\vec{r}$ is composed of:
> $$\vec{r} = \frac{x\vec{i} + y\vec{j} + z\vec{k}}{r}$$
> , where $$r = \sqrt{x^2 + y^2 + z^2}$$

---

Now that we know how electric fields function, how can we apply this knowledge? 

The first law we need is the **principle of superposition of electric fields**. Its not unique to just electric fields, its valid for any field, since it states that the *total field at a point is the vector sum of the field due to an object influencing the field*. In other words, everything has an effect on everything, and we have to sum up *every influence* in a field. $$\vec{E} = \sum_{i=1}^n \vec{E_i}$$
#### Field lines
---
These are imaginary lines drawn to show the direction of the electric field.
![[electric field lines.png]]

### Electric dipoles
---
These are pretty important, as they are made of one positive, and one negative side, and they show up a lot in nature!

Their **[[Torque]]** or amount of rotation??? is equal to:$$\tau = qEd\sin\phi$$, since dipoles have a tendency to rotate clockwise, and its equal to the force of the charges onto each other (coulomb's force) in the horizontal direction, so we need the sine of the angle between the 2 charges and their distance.

We can also calculate the potential energy of a dipole by calculating the **amount of work needed to turn the dipole**, and so $$U = -qEd\cos\phi$$ (since the integration of $\sin\phi$ is $\cos\phi$.)

We also define $p$ or the electric dipole moment as $qd$, so we can substitute that in if we'd like.



