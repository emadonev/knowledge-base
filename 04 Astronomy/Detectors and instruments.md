---
tags:
  - observation
  - astronomy
  - physics
  - mathematics
  - telescope
---
Other than just [[Telescopes]], we observe the universe via the [[Electromagnetic spectrum (EM)]] in other ways. We need a way to capture the information gathered by telescopes, so we developed different **detectors and instruments** to catch this information.

# 01 Photography and photographic plates
---
While these may seem ancient, they were the main stars back in the day of astronomy. These plates, which were cheap and easy to manufacture, would contain silver atoms ready to be excited by photons and form a normal silver atom, which when *treated with various chemicals, form silver bromide crystals (development) and then excess is scraped off (fixing)*. Unfortunately, the **quantum efficiency** of these plates is generally less than 5%, since not many photons actually excite the plate and once a certain saturation is reached it is reached. Its not a surprise we aren't really using these anymore. If for nothing else, they are great for *tracking objects in the sky*.

# 02 Photocathodes, photomultipliers, photometers and polarimeters
---
While these are not used for actual sky imaging, they are absolutely great for **photometry and brightness measurements**, since we can reach an accuracy of around 0.1-1%! Now, they work based on the [[Photoelectric effect]]. Electrons get excited, and move across to the positive charge, creating a current inside a photocathode. These cathodes light up dipoles in a photomultiplier, which releases more dipoles and causes an even stronger current. We can reach around 30% quantum accuracy with these instruments. 

But, how do we put them into practice?

![[photometer.png]]

[[Light]] from a telescope enters through the diaphragm, goes into the collimator and continues to pass through semitransparent mirrors, but some light does get reflected into separate photocathodes and into a photomultiplier, effectively splitting the beam into multiple different filters and measuring every filters brightness. This is very effective in [[The color index]] of [[Stars]] or [[Photometric quantities]]. 

# 03 CCD cameras
---
Since nobody knows what the acronym stands for, it is Charge Coupled Device. What does it do though?

![[CCD camera.png]]

Each pixel on the CCD camera (containing silicon) has an electron which can be released upon a photon strike, and the release of electrons creates a flow of electricity which can be read on a computer into an image. The quantum efficiency is typically 80-90%, and **it is the best in infrared and red spectrum (800-900 nm)**, while for shorter wavelengths it is less efficient due to properties of silicon. 

We use **flat fields** and **dark currents** to callibrate images we get from CCD cameras to remove bad pixels, background thermal radiation, etc. 

# 04 Spectrographs
---
These fantastic instruments are used for [[Spectroscopy]], a really useful branch of astronomy used to analyze the [[Spectra]] of stars and other objects. 
![[spectrograph.png]]
We focus light through a slit, differentiate into the colors using a prism and focus the image with a camera lens onto a detector, nowadays CCD. Using this, we can differentiate light and look at absorption spectra to look at different aspects of space objects.

Another method is using a **diffraction grating**, where we use grates to differentiate the light:
![[simple_grating.gif|450x400]]
# 05 Interferometers
---
These devices are actually pretty simple in practice, and they enable us to study [[Binary star system]]s, positions of objects in the sky, their sizes, etc. They use the interference patterns of [[Light]] to gather information about orbits, sizes, etc. 



