---
tags:
  - law
  - physics
  - planet
  - orbits
  - astronomy
  - math
  - dynamics_p
  - motion
  - geometry
  - ellipse
---
 >The radius vector joining any planet to the Sun sweeps out equal areas in equal times.

This basically translates to the fact that speed is **not** constant around an ellipse, and that if we are closer to the Sun we revolve faster than if we were further away. 

Here we introduce a new quantity, **angular momentum**. Remember regular momentum? It is like the "amount of motion", however in this case, this amount of motion is also rotating around some point, in this case around the Sun. We know that:$$\vec{p} = m\vec{v}$$
![[angular momentum ellipse.jpeg|400]]

Since the radius vector and velocity are well, vectors, the angular momentum is regular momentum multiplied by the radius:
- f $$\vec{L} = m\;\vec{v}\;×\vec{r}$$

Remembering properties about vectors, we can see that we have a **cross product**, which accounts for the area these 2 vectors produce. Looking at the ellipse (picture on the right) we can see that r changes with respect to $\theta$, and the velocity is not always perpendicular to the radius. Magnitude wise, angular momentum is equal to:
- f $$L = mvr\;sin\;\theta$$

> The second law of planetary motion states that angular momentum **is always constant in an orbit**. (As we saw in [[Kepler's first law - the law of ellipses]])

This is a huge takeaway! It means we can compare any 2 points on the ellipse and calculate other properties.

And in the case of **perihelion and aphelion**, the only 2 points where velocity is 90º agains the radius, $sin\;90º = 1$, and so $$\begin{align} L_a = L_p \\ mv_a\;r_a\;sin\;90º = mv_p\;r_p\;sin\;90º \\ v_a\;r_a = v_p\;r_p\end{align}$$
- f $$v_a\;r_a = v_p\;r_p$$, for aphelion and perihelion. (This is a nice simplification, however more complex approach follows)

# Proving Kepler's second law
---
How can we prove that this is true? What else can we gain from this law?
![[proving sceond law.png]]
Here we have a circular wedge, which when we make it super super small, can approximate the shape of an ellipse. The change in area corresponds to the change in radius as such:$$\frac{dA}{dt} = \frac{1}{2} r^2\;\frac{d\theta}{dt}$$
![[velocity of orbit.png]]

[[Velocity]] has 2 components, the x and the y. We can say that we have a radial and angular component, with unit vectors for r and $\theta$. $$\vec{v} = \vec{v_r} + \vec{v_{\theta}} = \frac{dr}{dt}\vec{r} + r\frac{d\theta}{dt}\vec{\theta}$$
Coming back to the original $dA/dt$, we can substitute:$$\frac{dA}{dt} = \frac{1}{2}rv_{\theta}$$
Since the radial component is **always perpendicular to the angular component**, (revisiting [[Kepler's first law - the law of ellipses]]$$rv_{\theta} = |\vec{r} × \vec{v}| = |\frac{\vec{L}}{\mu}| = \frac{L}{\mu}$$
Finally, the change in area over time is equal to:
- f $$\frac{dA}{dt} = \frac{1}{2}\frac{L}{\mu}$$

This rate of change is constant, as we previously established that angular momentum is conserved in an orbit. 

Using this knowledge, we can calculate the [[Energy in orbits]], and we can use this energy to  calculate **the velocity of a planet at any point in the orbit.**
$$-G\frac{M\mu}{2a} = \frac{1}{2}\mu v^2 - G\frac{M\mu}{r}$$, and simplifying that $M = m_1 + m_2$, $\mu$ can be canceled out into $m_1m_2$, We multiply everything by 2:$$-\frac{Gm_1m_2}{a} = \frac{m_1m_2}{m_1+m_2} v^2 - \frac{G2m_1m_2}{r}$$We can cancel everything by $m_1m_2$, and rearange so that $v^2$ is on one side:$$\frac{v^2}{m_1 + m_2} = G(\frac{2}{r} - \frac{1}{a})$$, and finally:
- f $$v = \sqrt{G(m_1 + m_2)(\frac{2}{r}-\frac{1}{a})}$$

VOILA! This is also called the *vis-viva equation* for orbital velocity. 