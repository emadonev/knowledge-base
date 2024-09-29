---
tags:
  - energy
  - physics
  - astronomy
  - mathematics
  - calculus
---
Thinking of charged particles and space around us, we can place them in a field, the **electromagnetic field**, where the [[Electromagnetic force]] acts upon it. Each charge has a certain energy in the field, which we can sort of say is analogous to kinetic energy. But:
- eg **The electric [[Potential energy]]**  is defined as the negative of the work required to bring a charged particle from infinity to a specific distance r from a reference charge. 

The image below describes this: ![[electric potential energy.jpeg]]
So, how would we derive the formula?

### 1) The force
The first step is to think about charged particles in a field. They all exhibit [[Coulomb's law]], or Coloumb's force which is:$$F = k\frac{Q_1Q_2}{r^2}$$, and it is extremely similar to [[The universal law of gravitation]], since they both <mark style="background: #61e8e1;">describe the same thing but in different fields</mark>. Since we are in the electromagnetic field, *every point in this field has a defined value*, so we can track the strength of this force with its dependence from the $Q_1$ charge. 

### 2) Work
We know from classical physics that:$$W = F * s$$, where F is a force doing the work over a certain distance, s. We can calculate the work by integrating ([[Integrals]]) Coloumb's force from infinity to a certain distance r. $$W = \int_{r_0}^r F \;dr = \int_{r_0}^r k\frac{Q_1Q_2}{r^2}\;dr$$
### 3) Solving the integral
We now proceed to solve the integral and then evaluate it:$$W = kQ_1Q_2\int_{r_0}^r \frac{1}{r^2} dr$$
We search for the *antiderivative* of $\frac{1}{r^2}$ by the power rule of integration:$$\int r^n\;dr = \frac{r^{n+1}}{n+1} + C$$, where C is the constant of integration. 
- n Why do we write this in the form we do? Because of derivatives, the power rule states that:$$\frac{d}{dx} = nx^{n-1}$$, so the first step is to take x to the power of n+1 (since we get n by subtracting 1), and then we have to divide by n+1 to regain the constant n.

And so, the antiderivative is:$$W = kQ_1Q_2[\frac{-1}{r}]_{r_0}^r$$
And now we evaluate the integral:$$U = -W = -kQ_1Q_2 (-\frac{1}{r} + \frac{1}{r_0}) $$ but since $r_0 = \infty$, then:
- !! $$U = k\frac{Q_1Q_2}{r}$$

