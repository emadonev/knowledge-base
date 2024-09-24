---
tags:
  - rocket
  - energy
  - orbits
  - planet
  - solary_system
  - satellite
---
While we talked extensively about [[Planetary orbits]] and [[Planetary properties]], [[Kepler's laws]], [[The universal law of gravitation]], etc. we haven't really talked about putting a **satellite in orbit with a rocket.** Now, a rocket is very complex, but we can make some simplified assumptions about its functionality, to get a basic understanding.

# The rocket equation
---
A rocket starts out with a certain mass $m$, moving at a speed $v_e$, which depends on the chemical energy burning. To us, the observer, it is moving at $v$. As some mass, $-dm$ gets expelled, the rocket moves at $v-v_e\;+dv$. For the conservation of [[Momentum]]:$$mv = (m+dm)(v+dv) - (-dm)(v_e - v)$$
Or:$$dv = -v_e\frac{dm}{m}$$
Integrating this, we get:
- f $$\Delta v = v_f - v_i = v_e\ln \frac{m_i}{m_f}$$

- n The fact that the velocity of the rocket doesn't depend on the initial velocity of the rocket, only on the exhaustion speed and amount of fuel burned. This way, $$\Delta K \approx mv\Delta v$$

# Hohmann Transfer Orbit
---
![[hohmann.jpeg|400]]

This manoeuvre is the most efficient manoeuvre, the transfer between 2 circular orbits. It consists of first, the probe given an impulse to bring it into an intermediate elliptical orbit at point P (tangent of course). Second, at point A we are given the second impulse, tangential, to form the final circular orbit. 

1. After impulse #1, the probe moves into an orbit with the semi-major axis, $2a = R_1 + R_2$. Thus, we can find the energy of that orbit:$$E = -\frac{GmM}{R_1 + R_2}$$
2. The **kinetic energy** here is the *total energy minus the potential energy*, hence:$$K = E - U = \frac{-GmM}{R_1 + R_2} +\frac{GmM}{R_1} = \frac{GmM}{R_1}(1 - \frac{1}{1 + R_2/R_1})$$
3. Remembering that $K = \frac{1}{2}mv^2$, we can calculate the velocity at point $P$, $v_P$:$$v_P = \sqrt{\frac{2GM}{R_1}(1 - \frac{1}{1 + R_2/R_1})} = v_0\sqrt{\frac{2R_2/R_1}{1 + R_2/R_1}}$$
4. The change in velocity is then simply:
- f $$\Delta v = v_0(\sqrt{\frac{2R_2/R_1}{1 + R_2/R_1}} - 1)$$

5. Since point $P$ is perihelion and $A$ aphelion, we can use the conservation of [[Angular momentum]] to calculate:$$mv_PR_1 = mv_AR_2\;\ce{->} v_A = \frac{R_1}{R_2}v_P$$
6. The final velocity must be that of a circular orbit, or $v_f = \sqrt{GM/R_2}$. So, the difference is:$$\Delta v_A = \sqrt{\frac{GM}{R_2}} - \frac{R_1}{R_2}v_0\sqrt{\frac{2R_2/R_1}{1 + R_2/R_1}}$$ or 
- f $$\Delta v_A = v_0\sqrt{\frac{R_1}{R_2}}(1-\sqrt{\frac{2}{1+R_2/R_1}})$$
7. And finally, the time it takes for all of this magic to happen is:
- f $$T^2 = \frac{\pi^2(R_1+R_2)^3}{8GM}$$

