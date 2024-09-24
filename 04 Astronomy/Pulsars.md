---
tags:
  - variable_star
  - star
  - astronomy
  - physics
  - quantum_physics
  - mathematics
---
These [[Stars]] are objects in the universe which pulsate at irregular intervals (most of the time). They only follow their cycle, called the **duty cycle** around 5% of the time, and sometimes there is a tiny pulse in the middle of a cycle, called an **interpulse**, and only 1% have it.

But, what are pulsars, really?
There were 3 options for the mechanism behind the pulses:
1) Pulsation (as seen in [[Variable stars]])
2) Orbital motion (they are orbiting another body which causes them to pulsate)
3) Rotation (the extreme rotation of a body could cause energy releases)

And there were 3 options for the **type** of star at play:
1) Normal star 
2) [[White dwarf]]
3) [[Neutron stars]]

So, which one is it?

### What is a pulsar?
---
#### 1) Pulsation
We are aware of [[Pulsation principles of stars]] in [[Variable stars]], and this mechanism only accounts for hours to days of periods. But, pulsars pulsate in **fractions of a second, around 0.1**. From previous analysis, we discovered that the period of pulsation is $$T = \frac{9}{8\pi} (G\rho)^{-1/2}$$
(*probably, ChatGPT says so, but check somewhere else to be sure, Note: i derived the formula*)

And, in order for a pulsating star to have such a short period, it would need an immense density, around $10^9$ g/cm3. This is much larger than the density of a white dwarf, but also much smaller than the density of a neutron star. There is **no star in between.**
- !! **Pulsation** is not the mechanism for pulsars!

#### 2) Orbital motion
What if our mystery star orbits another body?
Well, if we take equations for [[Binary star system]]s and [[Kepler's laws]], we would get that:$$\frac{4\pi^2 R^3}{G} = (m_1+m_2)P^2$$
And for a very, very short period, the distance necessary would have to be so small, that only 2 neutron stars could orbit each other for this to work. However, since pulsars slowly slow down after a while, this contradicts the formula! By the conservation of energy, *as pulsars give off radiation, the orbital energy has to decrease, or well R needs to become smaller*. Another issue are [[Gravitational waves]], which form as a result of such high energy orbiting of 2 neutron stars. 
- !! Orbital motion is not the mechanism for pulsars!
#### So, it must be rotation!
For rotation to be responsible for such extremely short pulsation periods, the gravitational force would have to be larger than the force required to keep a point moving in a circular path. 

This constraint on size only enables **neutron stars to be the best candidates for pulsars**. 

- n While the mechanism for pulsation is not fully understood, we think that the *extreme magnetic fields* around neutron stars accelerate electrons, causing [[Synchrotron radiation]], which makes them even brighter, and the flashes even brighter.

![[pulsars_mag.png]]

Since we cannot actually see the pulsation  of a pulsar unless we can see the radiation beam, we **only see around 20% of the total amount of pulsars in our galaxy**. 


## Period changes...
---
As rotation is the way pulsars pulsate, *over time, they give off energy, meaning that they have to slow down.* The [[Kinetic energy]] for a rotating sphere is analogous to the kinetic energy of a linearly moving body, however with rotational momentum applied ([[Neutron stars]]):
- f $$E_k = \frac{1}{2}I\omega^2$$

Now, we need to find how much does the energy change with respect to time. This is an easy [[Derivatives]] setup. After some tedious math and clever manipulation of the $\omega$ value, we get:
- f $$\frac{1}{E}\;\frac{dE}{dt} = -2\frac{1}{P}\;\frac{dP}{dt}$$

And, there is another thing pulsar do. They **glitch.** These are sudden decreases in period, and then they spike back up to their normal period, which continues to decline. 
- n A possible theory for the glitching is that the extreme magnetic fields and rotation put a huge strain on the solid crust of a neutron star, which causes it to crack, and then reconfigure into a stable configuration. 

Using our trusty angular momentum formula, we can derive using [[Calculus]] that:
- f $$\frac{dP}{dr} = 2\frac{P}{R}$$, or in fractional form: $$\frac{dR}{R} = \frac{1}{2} \frac{dP}{P}$$

## How far away are these pulsars?
---
As was already mentioned, [[Synchrotron radiation]] is all over the [[Electromagnetic spectrum (EM)]], meaning that different wavelengths of [[Light]] travel towards us, and they *will not arrive at the same time.* We call this **dispersion.** We know that:$$c(n) = c/n(\lambda)$$, where $c$ is the speed of light, $n$ is the index of refraction, and $\lambda$ is the wavelength. So, the time it takes for 2 signals to come is:$$t_1 = dn(\lambda_1)/c,\;\;\;t_2 = dn(\lambda_2)/c$$
And taking their time difference:$$\Delta t = (d/c)(n(\lambda_1) - n(\lambda_2))$$
Now, since all light travels through the universe, the index is the same, and it is equal to the **electron density of the universe,** since that is what light interacts with. From this, we can say that (while skipping a lot of math, [[Plasma frequency]])$$n(\lambda) - 1 \propto n_e$$
And then:$$\Delta t \propto d\;n_e$$
So, we can calculate the distance to any pulsar by their dispersion time, and the electron density is approximately constant throughout the universe!



