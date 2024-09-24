---
tags:
  - observation
  - math
  - telescope
  - astronomy
  - physics
  - light
---
Optical [[Telescopes]] observe a portion of the [[Electromagnetic spectrum (EM)]] which is the **visual part**. or the part we see with our eyes. We differ 2 main types of optical telescopes: [[Reflectors]] and [[Refractors]].  We use a large set of equations for optical telescopes in order to determine their optimal quality and how well they can observe the universe.

# F-number
---
The f-number is a simple quantity of a telescope:
![[f-RatioDiagram.gif]]
$$f-number = \frac{F}{D}$$
# Magnifying power
---
![[magnification.gif]]
The main principle behind magnification are the 2 angles, $\theta_F$ and $\theta_f$, because the larger either angle is, the larger the image is and the better the magnification will be. So, since they both form a right angled triangle, where$$tan \; \theta_F = \frac{x}{F}, \; tan\;\theta_f = \frac{x}{f}$$
- eg And since $x = x$, we can rewrite this equation using the small angle approximation as:$$M = \frac{\theta_F}{\theta_f} = \frac{F}{f}$$

### Field of view
---
Related to magnification we have the **field of view**. When we look at 2 images like in the example below, if we just look at something we have a very large field of view, since we see a lot of background.
![[EffectOfEyepiece.jpg]]
However, if we zoom in a lot, we don't see a lot of background. We magnified by a certain **magnification**, hence the formula is:
$$M = \frac{PVP}{SVP}$$, where $PVP$ is the apparent field of view, and $SVP$ is the real field of view.

### Image resolution
---
So, with a particular magnification what is the smallest detail I can see? This is a very important question when it comes to telescopes, and we can answer the question by looking at the capabilities of the eye. So, a 20/20 eyesight can tell apart 2 stars which are 120 arcseconds apart, which is pretty good. So, our image resolution is really with how close can my "2 stars" be? What is the necessary resolution which when magnified will be 120 arcseconds?$$Resolution = \frac{120}{M}$$
# The exit pupil and increase in brightness (izlazni otvor)
---
![[exit pupil.gif]]

A downside to constantly increasing the magnitude is that then the object covers a larger area of our field of view and then the ==surface brightness or the brightness of the image drops==, which may hinder some of the details in the image. We can reduce the magnification to a limit, and that limit is the exit pupil (izlazni otvor), which is the maximum "length" that light rays form in an image. Using similar triangles and the fact that $f<<F$, we get that:$$\frac{D_{ep}}{f} = \frac{D_o}{F+f} \ce{->} D_{ep} = \frac{D_o*f}{F} = \frac{D_o}{M}$$
However, we can't keep on making the exit pupil larger and larger, since we would start ==wasting light when the exit pupil is bigger than the eye pupil!== Hence, the minimum magnification for the maximum exit pupil which is the same as the eye is: $$M_{min} = \frac{D_o}{7 mm}$$
# Light gathering power - *light grasp*
---
But, what about the different objects we can look at in the night sky depending on their [[Photometric quantities]]? Let's first discuss normal light coming to the telescope, and the **light grasp** or the amount of light reaching our pupils based on the amount we collected with our telescope:$$G_l = \frac{D_o^2}{D_{eye}^2}$$
If we want to look at the magnitudes involved, we can apply the equation used for *flux differences between stars of different magnitudes*:$$G_{mag} = 2.5\;log(\frac{D_o^2}{D_{eye}^2}) = 5 \; log(\frac{D_o}{D_{eye}})$$ $$= 5\;(log(D_o) - log(D_{eye})) = 5log(D_o) - 5log(7) = 5log(D_o) - 4$$
So, in order to see what is the faintest magnitude we can see, since this is just **the gain in magnitudes we can see**, and we just add 6 since that is the faintest the eye can see: $$L_{mag} = 2 + 5\;log(D_o)$$
- !! An interesting result is that the magnitude of objects our telescope can look at **depends only on the diameter of the objective!**

And finally, the surface brightness is the same as the exit pupil squared times 2: $$SB = 2D_{ep}^2$$
- n From this we can conclude that a larger exit pupil will give us more light, but a less sharp image while a smaller exit pupil will give us more sharpness but a dimmer image. 

Using some equations from above, we can get a nice equation which ties together the focal lengths without the magnification:
$$M = \frac{F}{f}, M = \frac{D_o}{D_{ep}}$$
$$\frac{F}{f} = \frac{D_o}{D_{ep}}$$

$\ce{->}$ $f-number = \frac{F}{D_o}$
- !! $$f = D_{ep} * f-number$$

