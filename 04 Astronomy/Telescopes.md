---
tags:
  - "#telescope"
  - physics
  - astronomy
  - mathematics
  - star
  - obervation
  - light
---
# Observing through the atmosphere
---
Even though we can send probes and telescopes into space where there are very few problems, we still choose to have most of our observatories here, on [[Earth]]. However, multiple issues arise because of the atmosphere.

The atmosphere has many layers of varying temperatures and densities, and they are also never still. This means that when [[Light]] from [[Stars]] tries to come in through the atmosphere, it varies or **scintillates.** Stars, since they are point sources *scintillate a lot*, while planets shine more steadily. 

Another phenomenon due to the atmosphere is called **seeing**. Its when telescopes collect a lot of light to diminish scintillation, but the moving atmosphere causes refractions of light paths in certain areas, smearing point sources into *vibrant speckles*. 

**Extinction** is the scattering of light in the atmosphere, which is important to take into account when we measure the brightness of objects ([[Photometric quantities]]). It is also the reason why the sky is blue, and why it is red upon sunset. This specific scattering is called **Rayleigh scattering.** 

When it comes to the [[Electromagnetic spectrum (EM)]], different areas of the atmosphere absorb different wavelengths, so some are off limits to Earth telescopes. The optical band passes through, from 300 to 800 nm, but any wavelength lower than 300 nm gets absorbed by either the **ozone layer** or the upper layers of the atmosphere, where $O_2, N_2$ and free atoms are the absorbants. For wavelengths larger than 800 nm, it is transparent up to 1.3 $\mu m$. As we can see from the image below, microwaves can enter in a few specific windows, while radio waves have a much wider window of observation. 

![[windows_of_observation.png|600x500]]


# About telescopes
---
Telescopes are amazing tools that are essential to astronomers for observing the universe. Without them, we wouldn't be able to find out so many things which we know today. Telescopes observe **light across the whole [[Electromagnetic spectrum (EM)]]**, in order to get as much information about [[Stars]] and other space objects. A telescope image is made from the light from countless point-sources of light whose photons have managed to reach our telescopes. 

The 2 main parts of a telescope are:
- !! **Light gathering power:** how good is a telescope at scooping up light and looking at faint objects
- !! **Angular resolution:** how well can a telescope look at details on an object

![[ight gathering.jpg]]
So, we can conclude that the larger out **aperture is**, or the surface area of the objective, **we can gather more light and hence see objects better.** 
# Types of telescopes
---
Since we observe throughout the spectrum, we have [[Optical telescopes]], [[Infrared telescopes]], [[Ultraviolet telescopes]], [[Radio telescopes]], [[X-ray telescopes]] and [[Gamma ray telescopes]], all designed to look at specific properties of objects. 

# Optical telescopes
---
Optical [[Telescopes]] observe a portion of the [[Electromagnetic spectrum (EM)]] which is the **visual part**, or the part we see with our eyes. We differ 2 main types of optical telescopes: [[Reflectors]] and [[Refractors]].  We use a large set of equations for optical telescopes in order to determine their optimal quality and how well they can observe the universe.

### Angular size
---
The first quantity that we can calculate is the <mark style="background: #f2e863;">angular size</mark> of an object we are trying to look at better. It is the size of an object in degrees, as seen from Earth. 

![[angular size.jpeg|200x200]]


We can see a right triangle forms between half of the angular size, the distance to the object $d$ and half the diameter of the object $h_0$. Using trigonometry we can see that:$$tg \frac{\alpha}{2} = \frac{h_0}{2d}$$
With $\alpha$ then being:
- f $$\alpha = 2 \;arctg(\frac{h_0}{2d})$$, which is the general formula. However, for *reallly small angles*, we can use the small angle approximation where $tg(\alpha) = \alpha$ and then the 2s would cancel out and we get an approximative formula of:$$\alpha = tg\frac{h_0}{d}$$

The thin lens equation
---
![[thin lens equation.jpeg|400x300]]

We can construct a lens which makes an image of an object by using 2 circles with radii $R_1, R_2$. The lens has its own refraction index $n$, and we want to know the distance $q$. The focal distance $f$ is the distance from the centre of the lens to the point where the ray hits the straight line going through the centre of the lens. 

The thin lens equation is:
- f $$\frac{1}{p}+\frac{1}{q} = \frac{1}{f}$$

If we take that p, the distance to the object is in infinity, we see that the image of a distance object is formed within the focal plane of the lens, since $\frac{1}{p} -> 0$. 
## Reflectors
---
These types of telescopes use the principle of **reflection** in order to bounce light around for us to be able to see it. They can support large diameters of objectives, shorter lengths of the tubus, we don't have chromatic aberration or some other types of aberrations, and they are easier to use!

The first reflector made was **Newton's telescope**, but many other designs followed, including ones ==with both mirrors and lenses==. It is called the Newtonian telescope.

![[reflectors.png]]

The second way of building a reflector is with the Cassegrain focus, where we reflect light of a primary mirror into a hyperbolic mirror and through a hole in the primary one. 
![[cassegrain focus.png|400x200]]

And to get the effective focal length of a cassegrain focus, we use the equation:
- f $$f_e = \frac{b}{a}f_p$$

The final focus is the Coude focus, which is used for spectrography since it is super precise, however a big drawback is that only 30% of the incoming light actually gets detected, the rest reflected away. 

However, reflectors aren't problem-free. They have some issues, but they can be resolved. The first one is **coma**, where light rays do not converge at one point, but rather form a *comet-shaped* object. This makes the actual field of view of the telescope much much smaller than its apparent view - there is a small window where coma doesn't affect the image. 

We can avoid coma if the **primary mirror is spherical**. But this just leads to another problem - ==spherical aberration==. Light rays from the centre and edges converge at different points due to the spherical surface. This can be fixed using a **Schmidt lens**, which corrects the converging points. Because of this, **Schmidt cameras** are amazing and have excellent quality, with sharp stars.

![[schmidt camera.png|400x200]]

It is important to note here that then the:
- f $$R = 2f$$, or the radius on the image is equal to twice the focal length.

And, in order to build even bigger telescopes, we can put mirrors together into an array so that we have a huge surface area of collection, without mirror sagging. 
## Refractors
---
The earliest and simplest [[Telescopes]] were **refractors**, a type of [[Optical telescopes]] whose main property is the ==use of lenses for bending [[Light]] and focusing it.== They are pretty easy to build and cheap, however have many many drawbacks. 

There are 2 types of refractors: the astronomical (Kepler's) and terrestrial (Galilean) telescopes. Astronomical telescope is the one that has a *convergent eyepiece*, while for a terrestrial telescope they have *divergent eyepieces*, which 

The total distance of the telescope depends on the types of lenses, and for the astronomical telescope where both the objective and eyepiece are convergent, their focal lengths together give the length of the telescope:
- f $$L = F + f$$

On the other hand, Galilean telescopes (terrestrial) have one convergent lens for the objective and one divergent for the eyepiece. Since the focal length of the eyepiece is **negative**, since it doesn't focus light but scatters light, the length is:

- f $$L = F - f$$

![[distance and angle telescope.jpeg|400x200]]

A big problem for these kinds of telescopes is **chromatic aberration**, or when colors of different wavelengths focus at different points through glass of a lens. Lenses are generally impractical, expensive, have limited diameter and a very impractical length.

![[refr_2.gif]]
A cool thing about telescopes is that we can **combine refractors and reflectors to make** ==catadiopters==, which have both mirrors and lenses. Common ones are Schmidt-Cassegrain, Maksutov and Ritchey-Chretien. 


### Ratios of distances
---
We can relate the height of the image (or the size) and the real life size of an object using simple geometry of a telescope with the refraction of light. In the image above, we can see that the height of the image and the focal distance from the objective can be analogous to the real life "height" or radius of object and the focal distance to the real distance! Hence:

- f $$\frac{h_I}{F} = \frac{r_0}{d_0}$$

### Magnification 
---
The main principle behind magnification are the 2 angles, $\alpha_0$ and $\alpha_I$, because the larger either angle is, the larger the image is and the better the magnification will be. So, since they both form a right angled triangle, where$$tan \; \alpha_0 = \frac{x}{F}, \; tan\;\alpha_I = \frac{x}{f}$$
- f And since $x = x$, we can rewrite this equation using the small angle approximation as:$$M = \frac{\alpha_0}{\alpha_I} = \frac{F}{f}$$


- !! Since light is refracted, the tube has to be **very long** for larger lenses, which is hard to build and manouver
## Angular resolution
---
<mark style="background: #eaf2e3;">Angular resolution</mark> is the smallest angle needed to be able to differentiate 2 stars in the sky. When talking about light in this context, we think about **waves** and the specific distance/frequency of wave. When 2 waves are **in phase**, meaning that they have the same frequency, their wave values align and we have *constructive interference*. Meanwhile, if 2 waves have to travel slightly different distances or have a slightly different frequency, their values don't align and they *destructively interfere*. What we get is a very bright point in the centre, and then less and less bright circles around it with missing circles in between. This is called *Fraunhofer diffraction*. 

![[rayleigh criterion good.jpeg|250x200]]

If the separation between the 2 peaks of waves of the 2 stars is larger than the minimum distance, or the wavelength of the first star, we can differentiate them!

![[rayleigh criterion bad.jpeg|200x200]]

 If not, we are unable to resolve them. This is called the <mark style="background: #f2e863;">Rayleigh criterion</mark>. 

Using some fancy math and physics, we can arrive at the formula which depends on the wavelength of the light (which is intuitive, different wavelengths have different frequencies), and the diameter of the telescope (larger diameter, more light, more interference because of differing frequencies):

- f $$\Delta \theta (rad) = 1.22\frac{\lambda}{D}$$

, where $\lambda$ is the wavelength of observation (since the intensity varies with the wavelength of light), and $D$ is the diameter of the aperture. If we have degrees (or well, arcseconds), we can define the **Dawes limit**, which is the resolving limit of a telescope in arcseconds:

- f $$P_R = \frac{120}{D_o(mm)}$$, where $D_o$ is the diameter of the objective.

### F-number or aperture ratio
---
The f-number is a simple quantity of a telescope:
![[f-RatioDiagram.gif]]

- f $$R_f = \frac{F}{D}$$

### Field of view
---
Related to magnification we have the **field of view**. When we look at 2 images like in the example below, if we just look at something we have a very large field of view, since we see a lot of background.
![[EffectOfEyepiece.jpg]]
However, if we zoom in a lot, we don't see a lot of background. We magnified by a certain **magnification**, hence the formula is:

- f $$M = \frac{PVP}{SVP}$$, where $PVP$ is the apparent field of view, and $SVP$ is the real field of view.

### Image resolution
---
So, with a particular magnification what is the smallest detail I can see? This is a very important question when it comes to telescopes, and we can answer the question by looking at the capabilities of the eye. So, a 20/20 eyesight can tell apart 2 stars which are 120 arcseconds apart, which is pretty good. So, our image resolution is really with how close can my "2 stars" be? What is the necessary resolution which when magnified will be 120 arcseconds?

- f $$Resolution = \frac{120}{M}$$

## The exit pupil and increase in brightness (izlazni otvor)
---
![[exit pupil.gif]]

A downside to constantly increasing the magnitude is that then the object covers a larger area of our field of view and then the ==surface brightness or the brightness of the image drops==, which may hinder some of the details in the image. We can reduce the magnification to a limit, and that limit is the exit pupil (izlazni otvor), which is the maximum "length" that light rays form in an image. Using similar triangles and the fact that $f<<F$, we get that:

- f $$\frac{D_{ep}}{f} = \frac{D_o}{F+f} \ce{->} D_{ep} = \frac{D_o*f}{F} = \frac{D_o}{M}$$

However, we can't keep on making the exit pupil larger and larger, since we would start ==wasting light when the exit pupil is bigger than the eye pupil!== Hence, the minimum magnification for the maximum exit pupil which is the same as the eye is:

- f $$M_{min} = \frac{D_o}{7 mm}$$

## Magnitudes of objects
---
But, what about the different objects we can look at in the night sky depending on their [[Photometric quantities]]? Let's first discuss normal light coming to the telescope, and the **light grasp** or the amount of light reaching our pupils based on the amount we collected with our telescope:$$G_l = \frac{D_o^2}{D_{eye}^2}$$
If we want to look at the magnitudes involved, we can apply the equation used for *flux differences between stars of different magnitudes*:$$G_{mag} = 2.5\;log(\frac{D_o^2}{D_{eye}^2}) = 5 \; log(\frac{D_o}{D_{eye}})$$ $$= 5\;(log(D_o) - log(D_{eye})) = 5log(D_o) - 5log(7) = 5log(D_o) - 4$$
So, in order to see what is the faintest magnitude we can see, since this is just **the gain in magnitudes we can see**, and we just add 6 since that is the faintest the eye can see: $$L_{mag} = 2 + 5\;log(D_o)$$
- !! An interesting result is that the magnitude of objects our telescope can look at **depends only on the diameter of the objective!**

### Intensity of image
---
We know that the radius of the image in our telescope is:$$h_I = F\;tg\;\alpha_0$$
And so if the image is circular (most stars are), the area it covers is:$$A = \pi F^2\;tg^2\alpha_0$$
Now, only a small portion of the distant light of a star comes in. The flux of a star is how much of the luminosity of the star gets to Earth, or:$$F = \frac{L}{4\pi d^2}$$
This is per $m^2$ or cm or any measuring unit we want. And depending on the diameter of our telescope, a part of this light gets to it:
$$P = F * \pi(\frac{D}{2})^2 = F * \pi\frac{D^2}{4}$$
Finally, the *intensity* of our image is the amount of light we get from the image divided by the area: $$I = \frac{P}{A} = \frac{F\;\pi\;D^2}{4\pi F^2tg^2\alpha_0}$$, now for a given object the intensity is only dependent on 2 things: the diameter and the focal length. 

- f $$I \propto \frac{D^2}{F^2}$$

Which is coincidentally related also as:

- f $$I \propto \frac{1}{R_f^2}$$

# Telescope mounts
---
How we mount a telescope and correct callibration of coordinates so we can find stars is crucial! There are a couple of mounts, the 2 most important being the **azimuthal and equatorial** mounts, where the first corresponds to the horizontal coordinate system, and the second to the equatorial one. 

The equatorial mount is more stable and it is easier to track celestial objects, however, with the polar axis and declination axis it becomes increasingly harder to observe certain parts of the sky, plus the process of alignment is tedious. Nowadays that we have super precise computers and programs we can program telescopes to track objects with azimuthal mounts. The problem with this mount is that the field of view constantly changes, and we cannot really observe objects around the zenith.

Other mountings include the *Dobson mount*, used in amateur telescopes, its azimuthal but super easy to adjust by hand. Another type, used in **solar telescopes** is the *coleostat*, which uses mirrors to guide a telescope into a stable state. 

![[telescope mounting.png|500x300]]

---

- n One of the most influential telescopes built was the **Hubble space telescope**, launched in 1990. 