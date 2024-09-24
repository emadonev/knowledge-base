---
tags:
  - star
  - astronomy
  - structure
  - physics
  - mathematics
---
Models for stellar structure are important, as they help us understand stellar evolution and how stars work and fit into the HR diagram. 

##### How do we study a star?
---
Well, [[Stars]] are very simple - they are spherical! This means that we can only use the <mark style="background: #F0F6F6;">distance from the centre as our dependent variable</mark> to create a stellar structure. We of course use [[Calculus]] and [[Derivatives]] to model a star by dividing it into **shells**, with each shell being thick $dr$. So, the density of a co-centric sphere from the centre is dependent on the volume and mass, then:$$dM = \rho(r)\;dV$$
And well, volume of a spherical layer is the area of that layer multiplied by its thickness (an approximation), $dV = 4\pi r^2 \;dr$, so:$$dM = 4\pi r^2 \rho(r)$$, and if we get the rate of change of mass by the distance from the centre:

- f **Mass continuity**$$\frac{dM}{dr} = 4\pi r^2\;\rho(r)$$ 

Mass continuity is very important for stellar structures, as it tells us about the **gravitational force on a specific layer** ([[The universal law of gravitation]]). 

### Hydrostatic equilibrium
---
An extremely important aspect of the star is that it is **stable**. It is a constant sphere which doesn't collapse in on under itself. While the force of gravity **does** pull towards the centre, there *must be another force keeping it from collapse*. This force is the **pressure difference** of the shell of the star. The delicate balance between pressure and gravity is called <mark style="background: #EA63Ac;">hydrostatic equilibrium</mark>. 

Let's look a bit closer into this.
![[hydrostatic equilibrium.png]]

Let's analyze a specific cylinder inside a shell of a star. The cylinder has an area of $dA~$ and a height of $dr$. Its mass is then:$$dm = \rho(r) \;dr\; dA$$
Gravity, $F_g$, acts upon the cylinder, and it depends on $M(r)$. We can calculate this by integrating up until $r$. 
- f $$M(r) = \int_0^r 4\pi r'^2\;\rho(r') \;dr' =4\pi \int_0^r  r'^2\;\rho(r') \;dr' = 4\pi \int_0^r \frac{1}{3}r'^3 \;\rho(r') = 4\pi \;\frac{1}{3}\;r^3\;\rho(r) = \frac{4\pi}{3}\;\rho(r)\;r^3$$
The force is then given by:$$F_g = - \frac{GM(r)dm}{r^2}$$, where the - indicates that it is heading downwards. Let's substitute:$$F_g = - \frac{GM(r)\rho(r)dr\;dA}{r^2}$$ Now, we have **buoyant force**, which is commonly noticed on Earth as a force which drives objects in water upwards. (uzgon). It is the opposite direction of gravity, and it is the difference between the upward force on the bottom and the downward force on the top. $$F_B = P(r)\;dA - P(r+dr)\;dA = [P(r)- P(r+dr)] dA$$, and so we can say that:
- f $$dP = P(r+dr) - P(r)$$, which is the **pressure difference**. Then:$$F_B = -dP\;dA$$

Based on the fact that **gravity and pressure are equal:** $$F_B + F_g = 0$$$$-dP\;dA\;-\;\frac{GM(r)\rho(r)dr\;dA}{r^2} = 0$$
What we want to get from this equation is **how the pressure changes with radius**, so we divide everything by $dr$. $$-\frac{dP\;dA}{dr} = \frac{GM(r)}{r^2}\;\rho(r)\;dA$$$$-\frac{dP}{dr} = \frac{GM(r)}{r^2}\;\rho(r)$$
And we can see that actually $\frac{GM(r)}{r^2}$, is the same as the **gravitational acceleration at $r$**. So:

- f $$\frac{dP}{dr} = - g(r)\;\rho(r)$$

#### Equation of state
---
Other than just hydrostatic equilibrium, gases are constantly moving around, and especially in high temperature places like [[The Sun]] and stars, we need to thermally model it as well. We define a gas by its **pressure, temperature and density**. We can use the$$pV = nkT$$ formula. ([[The ideal gas law]]) (In this case, n is the particle density of the gas)*:
- f $$P = (\frac{\rho}{m})kT$$, where $m$ is mass per particle, and $\rho$ is the overall density
 
### Energy transport
---
Resolving the gases inside a star, **how does energy get around?**

- !! The **temperature of every layer in the star remains constant, since it stays in hydrostatic equilibrium**. This means that *the amount of energy leaving the shell is the same as the amount of energy entering the shell*.

We can then say the flux of radiation of energy is:$$f(r) = \sigma T(r)^4$$, and if we want to find the rate of change depending on $T$:
- f $$df = 4\sigma\;T(r)^3\;dT$$

, but the amount of energy absorbed can depend on the **absorption coefficient of the gas**, which we express per density of the material. So:

- f $$df = -\kappa'(r)\rho(r)\;f(r)\;dr$$, where the - means that flux decreases with absorption. 

Putting these together, and substituting **luminosity** in the mix, ($L(r) = 4\pi r^2\;f(r)$):
$$4\sigma\;T(r)^3\;dT = \frac{-\kappa'(r)\rho(r)\;L(r)\;dr}{4\pi r^2}$$
Doing a lot of tedious math results in the final formula:
- f $$L(r) = - \frac{16\sigma\pi r^2 T(r)^3}{\kappa'(r)\rho(r)} \;\frac{dT}{dr}$$

In a star, the change in temperature with the distance is negative, so temperature drops, which means that **luminosity is positive**, and stars shine. We can also notice that the absorption coefficient is really the **opacity of a star**, which is crucial for stellar models and [[Variable stars]]!!!! 

The final aspect would be how much the luminosity changes in a particular shell via energy generation:
- f $$dL/dr = 4\pi r^2\;\rho(r)\;\epsilon(r)$$, where epsilon is the *energy generated per unit mass within the shell at radius r*. 


