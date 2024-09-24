---
tags:
  - astronomy
  - physics
  - star
  - matter
  - atom
  - mathematics
  - calculus
---
[[Plasma]] is a weird state of matter, consisting of free electrons and positive ions, and so when something happens in our plasma field, if [[Electron]]s are slightly displaced, an **electric field is created, which gives us motion in this field**. 
- eg These **oscillations** are what we call **plasma frequency**.

This frequency is derived from the motion of an electron in a field, where the **force of a field is equal to $-eE$, and due to newtons law of motion, $F = ma$.**:$$m_e\;\frac{d^2x}{dt^2} = -eE$$, where the fancy derivative is actually acceleration. Due to [[Gauss' law]], for small displacements which take place in plasma, the electric field is equal to:$$E = \frac{n_eex}{\epsilon_0}$$. Combining all of this together, we get:$$m_e\;\frac{d^2x}{dt^2} = - \frac{n_ee^2x}{\epsilon_0}$$, and dividing both sides by $m_e$, we get:$$\frac{d^2x}{dt^2} = -\frac{n_ee^2}{m_e\epsilon_0}\;x$$, which just means that acceleration is equal to *something* times distance, which is the same formula for **angular frequency**, as in [[Circular motion]]. And so:
- f $$\omega_p = \sqrt{\frac{n_ee^2}{m_e\epsilon_0}}$$


---

So, we can *imagine the universe as an enormous place of plasma with a certain dispersion of free electrons.* This can be calculated via the **plasma frequency**, or:$$\omega_p^2 = \frac{n_e e^2}{\epsilon_0m_e}$$, and the refractive index with an **angular frequency** is as such:$$n^2(\omega) = 1-\frac{\omega_p^2}{\omega^2}$$, where $\omega = 2\pi c/\lambda$. Now, if the plasma frequency is much, much smaller than the angular frequency of light, we can apply some fancy math to simplify:$$n(\omega) - 1 \approx \frac{1}{2}\frac{\omega_p^2}{\omega^2}$$, which we use to get the equation for distances to [[Pulsars]]. 

# Gauss' law
---
> Gauss' law essentially states that the total electric flux through a closed surface is proportional to the total charge enclosed within that surface. The flux is a measure of how much the electric field "flows" through the surface.

The general statement of the law is:$$\int_{surface} E\;dA = \frac{Q_{enclosed}}{\epsilon_0}$$
If we integrate Gauss' law for a sphere (most common use), we gain the following:
- f $$E = \frac{Q}{4\pi \epsilon_0 r^2}$$, where it is 0 inside the hollow sphere, and E = E on the sphere and outside.
- f $$E = \frac{Qr}{4\pi \epsilon_0R^3}$$, for inside the sphere if it is solid and conducting.

# Other electrical laws
---
1. **Torque of an electrical dipole** $$\tau = pE\sin\phi$$, where $p$ is the **electric moment**
2. **Potential energy of an electrical dipole**$$U = -pE\cos\phi$$
3. What is $k$ equal to:$$k = \frac{1}{4\pi \epsilon_0}$$
4. Magnetic force on a moving particle:$$F = q\vec{v} × \vec{B} = qvB\sin \phi$$
5. Gauss' law for magnetism: **the total magnetic flux through any closed surface is 0.** (net magnetic flux) - $$\Phi_B= BA\cos\phi$$
6. Motion of a charged particle through a magnetic field - circular motion:$$R = \frac{mv}{|q| B}$$
7. Magnetic torque:$$\tau = \mu B\sin\phi$$, where $\mu$ is the magnetic moment
8. Potential energy of a magnetic dipole:$$U = -\mu B\cos\phi$$
9. Magnetic field due to a point charge with constant velocity:$$B = \frac{\mu_0}{4\pi}\frac{qvr\sin\alpha}{r^2}$$, where $v, r$ are normally vectors and $\alpha$ is the angle between them, while $\mu_0$ is the magnetic constant.