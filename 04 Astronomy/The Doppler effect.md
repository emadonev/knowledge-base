---
tags:
  - astronomy
  - velocity
  - physics
  - star
---

![[the doppler effect.png]]

The Doppler effect is an effect of light where as an object travels towards us, it becomes slightly blueshifted, and if the object is going away from us, it is slightly redshifted. Measuring these shifts, we can accurately determine the velocity of an object.

> The effect works in a way such that when a signal has to travel a longer distance, **more time is needed for that signal to travel**, hence:$$\Delta P = \frac{v_r\;P_0}{v_s}$$, where $P' = P_0 + \Delta P$. Since $\lambda = vP$, then:$$\lambda' = P'v_s = (P_0 + \Delta P)v_s = P_0v_s + \Delta Pv_s = v_sP_0 + v_rP_0 = (v_s+v_r)P_0 = \lambda_0 + v_rP_0$$, or finally $$\frac{\Delta \lambda}{\lambda_0} = \frac{v_r}{v_s}$$

For light, we apply the speed of an object and the *speed of light:*
$$z = \frac{\Delta \lambda}{\lambda_0} = \frac{v}{c}$$
$\ce{->}$ the *z* index of a star or object

So, the Doppler effect is the apparent wavelength dependent on the original wavelength based on the recession speed versus the speed of light in a vacuum. The formula is as such:
$$\frac{\lambda_{app}}{\lambda_{true}} = 1 + \frac{v_{rec}}{c}$$
- !! An important note! it is very important that in Doppler shift calculations ==6 decimals== are used, since the change in speed and wavelength is so small it is barely noticable

Another form of the equation above is when we rearrange the above equation:
$$\frac{∆\lambda}{\lambda_{true}} = \frac{v_{rec}}{c}$$
But what if we don't have the wavelength but frequencies? As we discussed in [[Light]], frequency and wavelength are connected by a very simple formula, which when applied to formula (2) looks like this:
$$\frac{f_{true}}{f_{app}} = 1 + \frac{v_{rec}}{c}$$
---

Using the Doppler effect, we can actually define **time-dilation**. This happens when we have a source moving away from us, and the wavelength gets shifted by $$\lambda' = \lambda + vT = (c+v)/f$$
Ergo:$$f' = \frac{1}{1+v/c}f$$
The time difference between those 2 points in space (due to movement) are:
- f $$\Delta t' = \frac{1}{\sqrt{1 - (v/c)^2}}\Delta t$$

Due to time dilation, when an object moves away from us, it is **redshifted**, and the wavelength appears to be longer. Combining time dilation with the Doppler effect, we get:$$f' = f\sqrt{\frac{1-z}{1+z}}$$, or:$$\lambda' = \lambda\sqrt{\frac{1+z}{1-z}}$$

The luminosity of a star which we see compared to the actual luminosity is:
- f $$L_0 = L_e\frac{f'}{f}$$