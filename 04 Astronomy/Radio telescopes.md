---
tags:
  - observation
  - telescope
  - astronomy
  - light
  - physics
  - math
---
We observe in the radio part of the spectrum ([[Electromagnetic spectrum (EM)]]) where limiting factors are the ionosphere of the Earth and the absorption from oxygen and nitrogen. We started observing in radio when Karl Jansky discovered radio waves from the centre of our galaxy, and later this knowledge was used by others to study the night sky in radio waves. For example, we use the 21 cm neutral hydrogen line to study our galaxy using *radio spectroscopy*. 

We build large radio [[Telescopes]], which have very large diameters since radio waves have large wavelengths. These telescopes are cooled for noise, located in remote environments, and since the wavelength is so large, they don't have to be completely solid, but mesh like. The telescope itself isn't here to form an image, it just collects light into a detector and the image is constructed by a computer. 

While a telescope on its own can have a pretty good resolution, if we want a great image of an object, we need a large **array of telescopes**, which act together as **interferometers** ([[Detectors and instruments]]). 

When light comes in perpendicular to the baseline, $D$, due to interference the wavelengths will sum together. If they don't come in perpendicular, the cancel each other out.
![[interferometer principle.png|350x200]]

However, since the Earth rotates around its axis, the baseline moves around forming a sinusoidal pattern. The distance between the peaks is:
- f $$\theta D = \lambda$$, $\theta$ is the angle the baseline has turned, $\lambda$ is the wavelength and $D$ is the length of the baseline.

Another thing to note is that if *the object the telescope is observing **isn't a point source**, then light from different parts of that object **have different phases when entering the telescope***. So, we define a quantity called **fringe visibility**:$$\frac{P_{max}-P_{min}}{P_{max} + P_{min}}$$, where $P_{max}$ is maximum value of the interference pattern and $P_{min}$ is the minimal value of the interference pattern.

We orient telescopes together (like VLA in new mexico) in a way such that they create **aperture synthesis**. This uses the baselines of multiple telescopes to extend the field of view:
![[aperture synthesis.png|400x450]]
The diameter of each circle is the wavelength divided by the distance between 2 radio telescopes. So, when we have more than 2, they can cover different radii together. 

---

Here is an example of an image where the green part is optical, and the blue is radio, and we can see that the resolution is very good!

![[ngc4038_small.jpg]]
