TAGS: #color #astronomy #physics #light #energy 

When discussing [[Photometric quantities]], we covered absolute and apparent magnitude. In that note, we covered the **Bolometric magnitudes** of both, meaning that they *covered all wavelengths.* However, there are different color indexes and filters we use in astronomy! 

We use the standard *UBV* system, measuring the star's apparent brightness through 3 filters:
- [[UBV photoelectric magnitudes]]
	- Ultraviolet, Blue and Visual,
however scientists have recently transfered to a more diverse system with more filters, called the UBVRI system.
![[ubvri.png|350x200]]

## Color indexes
------
We can quantify the "color" of stars by measuring with [[Photometric quantities]] the magnitude or flux of light coming from stars with different **filters**. These filters can be <mark style="background: #fefae0;">green, blue, visual, ultraviolet</mark>, etc. We can measure this as the energy per tie unit surface area within a wavelength range:
$$I(\lambda) d\lambda  \; - \; (\lambda + d\lambda)$$
This intensity shows as [[Spectra]] with a few 'jaggs' which are *spectral lines*.

- n How exactly do we quantify color though? Let's look at 2 wavelength ranges that we want to look at (filters). We can take a look at their ratio of brightness to see which one has more light emitted:$$\frac{b_1(\lambda_1)}{b_2(\lambda_2)}$$And now, we can see that the ratio of fluxes is actually the subtraction of their magnitudes: $$m_2 - m_1 = 2.5 log_{10}(\frac{b_1(\lambda_1)}{b_2(\lambda_2)})$$ From this we can conclude that as temperature rises, that the flux ratio rises also but the magnitude difference goes down, so **brighter stars have a lower index**. 

Here is a small table of handy peak wavelengths for popular filters:

| **Filter** | **Peak $\lambda$** |
| ---------- | ------------------ |
| U          | 350                |
| B          | 435                |
| R          | 680                |
| V          | 555                |
| I          | 800                |

- eg We can measure the color index of stars (the most famous being the BV index (blue, visual)): $$BV = m_{blue} - m_{visual}$$ or $$BV = M_B - M_V$$ because color doesn't change depending on if it is apparent or absolute magnitude. $\ce{->}$ from this we can conclude that the lower the value of BV that the blue part of the magnitude is higher hence the **star is hotter**, and the opposite is also true.

A problem with color is that due to scattering of light, we have **color extinction.** Now, the observed color index is:$$B − V = M_B − M_V + A_B − A_V$$, or$$B − V = (B − V )_0 + E_{B−V}$$, where the first term is the intrinsic color of the star, and the second is color excess. The ratio between the visual extinction and color excess is always around 3.0, so we can find V and $M_V$ quantities. 

![[bv nd color.png|400]]

We can see that the lower the B-V index, the higher the temperature. 

## Bolometric correction
------
In order to account for the difference between a bolometric and visual magnitude we use the following:
$$BC = m_{bol} - V = M_{bol} - M_V$$
## Color-color diagram
------
This diagram shows the relationship between the U-B and B-V color indices for main sequence stars. We can see that stars actually don't really behave like blackbodies, but they try 😉

![[color-color.png|400]]

