TAGS: #variable_star #star #astronomy 
[[Variable stars]]

A *light curve* is a type of [[Timeseries data]] where we measure the change in the magnitude of a star over time. The best way to analyze variable stars is to see the shape of our light curve. The best way to calculate the period and minimum and maximum magnitude is with **fitting polynomials to our light curve.** 

We analyse the shapes and the periodicity of our light curves in order to categorise them and infer more data from them. Both the period and the light curve shape **are crucial in categorisation and identification of light curves.** It is important to have a **phased light curve**, because we can infer waaaaay more from that light curve than from the standard input lc. 

The **phase** of a variable star(which fraction of the star's variability has elapsed) is calculated as so:
$$
phase = \frac{t - t_0}{P}
$$
Where $t$ is the time of measurement, $t_0$ is an arbitrary *epoch*: a time of minimum or maximum brightness, and $P$ is the period.

There are a couple of ways to fit a light curve, or well find a period:
1. **String length minimization method**
	1. First we try a number of different periods, and we pick one and draw a phase diagram.
	2. Then, we join each data point with a line, and calculate the lengths of the lines.
	3. If the lengths are short enough, it means that the period is better since there is less data scatter.
$$length =\frac{\sum_i (m_i - m_{1+i})^2}{\sum_i (m_i - M)^2}$$
2. **Fourier analysis**
	1. This method uses many trial periods for fitting different order sine waves together in order to fit the light curve.
	2. The formula for fitting a set of sine waves:
$$V(t) = \stackrel{-}V + \sum^n_{l=t}[A_l sin((\frac{2πl}{P})(t-t_0))+B_lcos((\frac{2πl}{P})(t-t_0))]$$
- $\stackrel{-}V$ is the mean magnitude of the light curve
- $A_l, B_l$: the fourier coefficients, they tell us the amplitudes of the sine and cosine waves at each frequency that, when added together, reconstruct our original function (chatGPT)
- $P$: trial period
- $t$: time
- $t_0$: zero-point time
- $n$: number of orders to be included in the building of the wave.
	3. The smallest root-mean-squared difference indicates the best fit!
3. **Fourier power spectrum of the light curve**
	1. In this method we use the [[Fourier transforms]] to break the light curve down into each of its sine waves and from the determine which one resonates with the period of the light curve.
	2. The frequency with the most power from the power spectrum might be the true frequency! The power of a frequency is the measure of how much this frequency contributes to the overall signal. The more it contributes, the more power it has!
	3. This method, however, requires evenly spaced data. This is impossible for astronomical data! This is why we commonly use the next method
4. **Lomb-Scargle periodogram**
	1. This periodogram is the almost the same as the power spectrum of a fourier transform, however it works for un-evenly spaced data. The periodogram give s the best estimate of the fourier transform, so its almost the same!
	2. This works by fitting sine waves to the data, and determining how well does it fit at each frequency. The frequency of the highest power is usually taken as the period.
	3. We can calculate the period by calculating the reciprocal of the frequency.

![[analysing_lc.png]]
It is important to know that sometimes we have **alias periods**, where this one is related to the true period. Commonly it is 1/2 or 2x the size of the true period. 

Standard fourier transforms for light curve analysis are *not particularly suitable for large amounts of data!*  

One thing to note is that there may be more than one peak in the periodogram.
>There may also be peaks in the spectrum which are purely due to the ‘noise’ in the data. How can one tell which peaks, if any, are real, that is statistically significant? Two elegant discussions of this issue are by Scargle (1982) and by Horne and Baliunas (1986), who present formulas for the false alarm probability for any peak.
>Some types of variable stars, mostly pulsating variable stars, exhibit [[Chaos theory]], a form of irregularity which can arise from a simple [[Dynamical system]] behaving in a [[Non-linearity]] way. (Buchler et al., 2004)
>- taken from Understanding variable stars by John R. Percy

