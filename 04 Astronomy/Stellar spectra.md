---
tags:
  - spectra
  - star
  - astronomy
  - mathematics
  - physics
  - data_analysis
---
As we have discussed in [[Radiation mechanisms]], the **spectra** of light of [[Stars]] is **continuous**, with absorption lines ==where the atmosphere of the star absorbed certain elements==. These lines tell us about the composition of a star, its temperature and **spectral type.** 

We take "photos" of spectra with a slit spectrograph, which has a small dispersion factor, to gain a line spectrum:
![[absorption_pic.gif]]

Then, the photograph of the spectrum is converted to an intensity tracing showing *the flux density as a function of wavelength*. This is done using a **microdensitometer**, measuring the amount of light transmitted by the recorded spectrum. In CCD cameras measurements of line strengths of the spectrum are usually rectified by dividing by the continuum intensity.
![[graph spectrum flux density.png|400]]

We also talked about the **line profile** and how the shape of the line tells us about stellar composition. The wider the **equivalent width** of a line is, the more atoms of that particular element are in the star. 

# Harvard classification system
---
How do we classify stellar spectra? It seems that certain stars have different spectra, but that we can make general categories from this data. The Harvard classification is based on *lines that are mainly sensitive to the stellar temperature*, rather than to gravity or luminosity.

There are a few distinct lines which tell us about the spectral type of a star:
- the Balmer series
- lines of neutral helium
- iron lines
- H and K doublet of ionized calcium at 396.8 and 393.3 nm
- G band due to the CH molecule and some metals around 431 nm
- neutral calcium line at 422.7 nm
- lines of titanium oxide (TiO)

We have: **OBAFGKM** and then later **LTY**, with subtypes of **M** being **C and S**, **Q** are for novae, **P** for planetary nebulae, and **W** for [[Wolf-Rayet stars]]. We can use the classical mnemonic for this: *Oh, be a fine gal kiss me*, or for a more ominous tone (my own mnemonic): **Obviously, because any friends gladly kills monsters**. Each of these big case letters is also further ground down to 10 sub categories, like A0, B2, etc. 

Let's go through each star, one by one:
## O-type stars (blue stars)
---
- TEMP: 20000-35000 K
- they have lines from multiple ionized atoms
	- $HeII$,
	- $CIII$, 
	- $NIII$, 
	- $OIII$, 
	- $SiV$. 
	- $HeI$, visible, 
	- $HI$ lines, weak

## B-type stars (blue-white)
---
- TEMP: above 15000
- $He I$ (403 nm) lines are strongest at B2, then get weaker and have disappeared at type B9
- $K$ line of $Ca II$ becomes visible at type B3
- $HI$ lines
- $O II$, 
- $Si II$
- and $Mg II$

## A-type stars (white)
---
- TEMP: 9000 K
- $H I$ lines strong, dominate most of the spectrum
- $H$, $K$ and $Ca II$ lines stronger
- $He I$ not visible anymore
- **metal lines begin to appear**

## F-type stars (yellow-white)
---
- TEMP: 7000 K
- $H I$ getting weaker
- $H$, $K$ and $CaII$ getting stronger
- $Fe I, \;FeII,\;CrII,\;TiII\;$ begin being visible

## G-type stars (yellow)
---
- TEMP: 5500 K
- $H$ and $K$ lines super strong, $H I$ still declining
- $G$ band visible
- metal bands getting stronger
- $CN$ lines in giant stars

## K-type stars (orange-yellow)
---
- TEMP: 4000K
- dominating metal lines
- $Ca I$ very visible
- strong $H$, $K$ and $G$ band
- $TiO$ band becomes visible at K5

## M-type stars (red)
---
- TEMP: 3000 K
- many neutral metal lines, $TiO$ getting stronger, $CaI$ as well

## C-type stars - carbon stars
---
- TEMP: 3000 K, very red
- strong molecular bands:
	- $C_2$, $CN$, $CH$

## S-type stars - low temperature stars
---
- TEMP: 3000 K
- very clear $ZrO$ bands, $YO,\;LaO,\;TiO$ bands

## L-type stars - dark red
---
- TEMP: 2000 K
- no more $TiO\; and\; VO$ bands
- very broad and strong $NaI,\;KI$ lines

## T-type, brown dwarfs
---
- TEMP: 1000 K
- very strong lines of $CH_4$ and $H_2O$ 

---
From these stars, we can notice that we **only need their temperature to be classified,** since other properties don't really affect stellar spectra. Another interesting fact is that due to these temperatures, **we get different spectra** due to the ==ionization of various atoms and molecules==.

- n Molecules cannot be absorbed or exist at extremely high temperatures, so they are only present in low temp stars. Too high temperature ionizes atoms, making it harder for them to get excited, a high temperature gives many neutral atoms a chance to get excited, etc.

![[spectral lines.png]]

# The Yerkes Spectral classification
---
Other than temperature, we need another factor to differentiate stars. 2 stars of the same spectral class can have veeeery different **Luminosities!** ([[Photometric quantities]]) So, a special classification system is devised for luminosity classes:
1. $Ia$ - most luminous supergiant
2. $Ib$ - less luminous supergiant
3. $II$ - luminous giant
4. $III$ - normal giant
5. $IV$ - subgiant
6. $V$ - main sequence star/dwarf

How do we determine which star goes into which category, though?
> We look at **lines which strongly depend on stellar surface gravity**, since it is very related to luminosity (radius being the key factor for luminosity). The difference between radii of stars give rise to **luminosity effects**!

- eg **The Stark effect** - a crucial luminosity effect, neutral hydrogen lines in hot stars are deeper and narrower for high luminosity stars. The reason is that *metal ions create fluctuating electric fields near the hydrogen atoms*, developing a shift in the energy levels - broadening the line.
- eg **Ionized lines** are more present in high luminosity stars, due to their larger density and atmospheres.
- eg For giant stars, **the stronger their color**, the more luminous they are. For a dwarf and a giant star, the giant is going to have a slightly lower temperature, so its going to be *more red.*
- eg $CN$ lines are only present in giant stars since cooler atmospheres of giants are more suitable for the formation of this molecule.

# The HR diagram
---
Arguably the most important diagram in astronomy, the Hertzsprung-Russel diagram which explains the relationship between absolute magnitude/luminosity with the color index/temperature. Most common diagrams are mag/temp. There are a few structures on the diagram, including the ==white dwarfs, dwarfs, main sequence, giants section, red giants branch and supergiants==. 

![[fancy hr diagram.png|400]]

These diagrams are extremely useful for studying stellar evolution and other properties of [[Stars]]. 

---
But, what can we find out from stellar atmospheres, the HR diagram, and spectra? 

We obtain a **mass-luminosity relationship**, which states:
- f $$L ∝ M^{3.8}$$

