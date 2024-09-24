TAGS: #magnitude #light #star #physics #math #astronomy 

[[Light]] is an essential part of astronomy. It is the only information we gather about the universe around us since everything is so far away! So, we must be very careful in analyzing the brightness of stars. 

# Intensity, Flux density, Luminosity
---
Let's say we are trying to determine the amount of energy passing through a certain area, $dA$. 
![[intensity.png|350x300]]

$$dE_\nu = I_\nu\cos\theta \;dA\;d\nu \; d\omega \;dt$$, where $I$ is the **intensity at a specific wavelength,** A is the area, $\theta$ the angle between perpendicular axis and axis of interest, $\nu$ is the frequency, $\omega$ is the solid angle and t is time. 
The total intensity of light from an object can be integrated for all frequencies:$$I = \int I_\nu d\nu$$
The **flux of an object** means that power goes through some surface, expressed in watts. **Total flux** is the flux passing through a closed surface encompassing the source, or in other words, the [[Luminosity]] of an object. Using calculus we can prove that the amount of energy, or the intensity of radiation is **uniformly spread out in space**, enabling luminosity to be:
- f $$L = 4\pi r^2 F$$

- eg **Radiant Flux** is the total amount of light energy in every wavelength which crosses a unit area oriented perpendicular to the direction of the light's travel per unit time. (Watts received by $1m^2$) (a slightly more precise definition)

The **energy density of radiation** can also be expressed, if we have a solid angle developing into a volume:
![[volume energy density.png|300x100]]

Where:$$u = \frac{1}{c}\int_S I\;d\omega$$, but now that energy fills a volume, we have:$$dE = I\;dA\;d\omega\;dt = \frac{1}{c} I \;d\omega\;dV$$ (the one over $c$ factor is necessary since light travels at the speed of light, necessary for time transformations in the calculations)

Since energy density is the change in energy by change in volume, we get:
- f $$u = \frac{4\pi}{c}I$$

# Apparent magnitude
-----
The first astronomer to every catalogue stars was Hipparchus. He tracked 850 stars, and he also devised a system of magnitudes to characterize their brightness. $m=1$ for the brightest, and $m=6$ for the faintest. He devised a **logarithmic scale**, where every brightness is a ratio of the previous one.
- n The differences between the magnitudes were simple. The difference between a 1st magnitude and a 5th magnitude was exactly 100 times fainter, so the difference between 1 magnitude is **around 2.5, or Pogson's number.** We also extended the scales in both directions to accompany the plethora of objects we found in space.

We can compare the fluxes of 2 stars using Pogson's number and the fact that it is a logarithmic scale.
$$\frac{F_2}{F_1} = 100^{(m_1-m_2)/5}$$
Or in other words:
- f $$m_1 - m_2 = -2.5 log_{10}(\frac{F_1}{F_2})$$

Other than point sources, objects in the sky can appear as **integrated magnitudes**, where we take into account their surface area and as light hits it. So, the difference between the integrated magnitude and surface one is the flux difference of both. Since the integrated magnitude is really the area times surface flux, we get:
- f $$m_{int} = m_s - 2.5\log A$$, where $A$ is the area, $m_{int}$ is the integrated magnitude and $m_s$ is the surface magnitude.

# Types of apparent magnitudes
---
However, we can observe flux at *any frequency we like*, so a star can have **different values for apparent magnitude depending on which frequency range we are focusing on.** For wavelengths of about 550 nm, it is called ==the visual band==, $m_v$. The ==apparent magnitude of all the frequencies combined is called== the ***bolometric magnitude.*** Bolometric values are very difficult to measure because of the atmosphere and the fact that observing different wavelengths of light is difficult ([[Electromagnetic spectrum (EM)]], [[Telescopes]]), but if we know the *bolometric correction*, which is specific for specific types of stars, we can say:$$m_{bol} = m_v - BC$$
The bolometric correction for the Sun is 0, and the more a star deviates from the Sun in radiation form, then the correction value is greater as well. 
# Absolute magnitude
-------
Using the aforementioned law, we can assign the **absolute magnitude** of a star, meaning the brightness of a star (apparent) if it were at a distance of 10 pc from the Earth.

So, if we want to combine the distance and flux together to calculate the absolute magnitude at 10 pc, we combine this last formula and the formula for flux:
$$m-M = -2.5log_{10}(\frac{\frac{L}{4\pi d^2}}{\frac{L}{4π10^2}})$$
$$m-M = -2.5log(\frac{d}{10pc})^2$$
$$100^{(m-M)/5} = (\frac{d}{10pc})^2$$, which gives $$m−M=5\;log\frac{r}{10pc}$$
If we want to compare luminosities of a star and our sun, then we would apply a very similar formula to the 3rd formula in this note:
 $$M = M_{sun} - 2.5log_{10}(\frac{L}{L_{sun}})$$
 In the study of [[Variable stars]], we actually don't need to know the distance to determine the luminosity or magnitude! We use the star to actually [[Calculating distances in astronomy]].

# Extinction and optical thickness
---
There is a slight issue with all of these formulas. 
- !! They **assume** that all light from our chosen object **comes to the Earth, unharmed**. In reality, some of it is absorbed by [[The Interstellar medium]], or scattered away, or something happened to it. This is called ***extinction***.

![[extinction.png]]

$$dL = -\alpha L\;dr$$, where $\alpha$ is the opacity of the medium, it tells us how much it can absorb light. Let's define a new quantity! **Optical thickness** ,$\tau$, as such:$$d\tau = \alpha \;dr$$ So, now:$$dL = -L \;d\tau$$ We can integrate this from the source to the observer, so from $L_0$ to $L$. $$\int_{L_0}^L \frac{dL}{L} = - \int_0^\tau d\tau$$
Which means that:
- f $$L = L_0 \;e^\tau$$

If we reevaluate the absolute magnitudes function using this new found knowledge, we get:
- f $$m-M = 5 \;log\frac{r}{10pc}+A$$
,where A ≥ 0 is the extinction in magnitudes due to the entire medium between the star and the observer. How do we then define $A$? Well:$$A = m' - m = 2.5 \log (I_0/I)$$, or:
- f $$A = 2.5 \log (e^\tau) = 2.5\log(e)\;\tau = 1.086\tau$$

If the extinction was for the atmosphere of Earth for example, we would take into account the height of the atmosphere and the zenith distance of the light hitting an observer, and have the most general formula:
- f $$M = m_{surface} - 5\log d + 5 - 2.5\log e^{kd} - 2.5\log e^{k_a h/\sin z}$$

