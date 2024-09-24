TAGS: #frequency #data #programming #computer_science #physics 

The Fourier transform is designed to make out specific frequencies out of a mesh of frequencies, which is especially useful in time series data. It decomposes a wave into a sum of *sine waves of varying frequencies*. There are obviously different types of transforms, based on the data given.

1. **Continuous-Time Fourier Transform (CTFT)** - input signal is continuous and defined for all time
2. **Discrete-Time Fourier Transform (DTFT)** - discrete but infinite
3. **Discrete Fourier Transform (DFT)** - discrete and finite
4. **Fast Fourier Transform (FFT)** - most common, computing DFT efficiently
5. **Short-Time Fourier Transform (STFT)** - frequencies vary a lot over time
6. **Quantum Fourier Transform (QFT)** - linear transformations on quantum bits

> *"By applying a Fourier transform to the time-series data of a star's brightness, we can convert the time-domain data (brightness as a function of time) into frequency-domain data (showing the strength of different frequencies within the data). Peaks in the frequency-domain data represent the dominant frequencies or periods in the brightness variations. This is particularly helpful in cases where the brightness changes are not obviously periodic, or where there are multiple overlapping periods."*
> - ChatGPT

So, the way this works, is actually quite simple. We have a wave, which is composed of many frequencies. If we were to wrap this wave around a circle, and the tightness of the wrapping is determined by different frequencies we try out, we can model the original wave. If this wrapped component had a centre of mass and we tracked the x position of this centre, we can plot all of the distances that centre of mass is away from the origin. In this way, we see that at the frequency of the wrapping which is the same as some frequency which is in the original wave. Each of these peaks in the graph when the centre of mass diverges from the origin is the period or frequency of one of the waves in the mix of the original wave.

The formula is:
$$\int_{-∞}^∞ f(t)e^{-2πift} dt$$
-> what this does is first wrap our starting signal around a circle, since circles are the empirical way of describing cyclical and periodical facts. This way, mapping them into a complex plane, allows us to draw a circle and wrap the function $f$ over time around the circle. Then we use [[Integration]] to find the right frequencies for our starting signal. The reason why we use the "centre of mass analogy" is because it represents the average frequency present at the time. 

![[fourier transform.png]]

