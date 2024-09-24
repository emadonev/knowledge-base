TAGS: #astronomy #variable_star #programming #computer_science 

> John Hoffman, Jake VanderPlas, Joel Hartman and Gáspár Bakos [[A fast template periodogram.pdf]]

-------
In this research paper researchers present an *[open source code available on GitHub](https://github.com/PrincetonUniversity/FastTemplatePeriodogram)_* for optimization of periodograms called <mark style="background: #A3C4BC;">template periodograms</mark>.  

- eg **Template fitting or periodic matched filtering:** technique for identifying, classifying and characterizing periodic variability for noisy light curves ([[Timeseries data]]). 
$\ce{->}$ however, they require a lot of computational power, a lot more than a [[Lombe-Scargle periodogram]].
$\ce{->}$ the template fitting is much more precise, however it takes much more than LS depending on the number of data points. This is especially relevant for my [[VARIABLE STAR PROJECT]] since I have up to 2000 observations in a single light curve!
$\ce{->}$ template fitting only has 3 parameters: **amplitude, phase and a constant offset**, rather than **2H+1** parameters, where H is the number of harmonics!

- pr *"The multiharmonic periodogram is designed to find non-sinusoidal periodic signals in irregularly spaced time series data. However, as shown in, increased flexibility comes at a cost – the noise level of the periodogram relative to the maximum peak height tends to increase as the number of free parameters in the model $y^-$ increases, and in some cases the best frequency can tend to a harmonic or a subharmonic of the true frequency." * - from [[A fast template periodogram.pdf]]

# Programming aspect
-------
#### Installation
```Terminal
$ pip install ftperiodogram
```


