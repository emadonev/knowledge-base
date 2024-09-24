TAGS: #astronomy #time_series #data #data_analysis #programming 

The **Lomb-Scargle** periodogram uses [[Fourier transforms]] in order to fit sine and cosine waves to light curve data ([[Variable stars]],[[Analyzing light curves]]). This periodogram is the almost the same as the power spectrum of a Fourier transform, however it works for un-evenly spaced data. The reciprocal of the frequency of the highest power is usually taken as the period. 

$$P(ω)= \frac{1}{2σ^2}​*(\frac{[∑y_k cosω(t_k−τ)]^2}{∑cos^2 ω(t_k−τ)} + \frac{[∑y_k sin ω(t_k−τ)]^2}{∑ sin^2 ω(t_k−τ)})$$
This is the formula for the LS periodogram. The tau in the formula represent the delay-shift. 

>"*This shift can enhance the sensitivity of the periodogram, especially when dealing with unequally spaced data. In other words, it fine-tunes the phase of the sinusoid to get a better match to the data.*"
>- ChatGPT

- n Sometimes, due to signals or noise in the data, the periodogram might give false power to harmonics which do not contribute to the actual shape of the light curve (hence they will give a false period). We can calculate the *false-alarm probability (FAP)* of that happening by the following equation $$Q = 1 - [ 1-(1-\frac{2P_n}{N_t})^{(N_t-3)/2}]^{N_f}$$, where $P_n$ is the height of a normalized periodogram, $N_t$ is the number of points in the time-series, $N_f$ is the number of independent frequencies calculated by the algorithm. $1-\frac{2P_n}{N_t}$ gives the strength of the peak relative to the number of data points. We raise this to a very specific power regarding the number of points (specifics are too complicated, yet). When we subtract 1 the first time, we see the probability of how rare the peak of hight $P_n$ would be present with noise. Raising everything to the power of $N_f$ tells us how likely this is compared to the number of frequencies present. Finally, we subtract 1 to gain the final probability.

# Optimizing the LS periodogram ([[Fast calculation of the Lomb-Scargle periodogram using GPU]])
------
The standard computation of the LS periodogram is very slow because it requires you to go through the data twice and you have to calculate trigonometric function evaluations every time. So, we use the following equations to do the job quicker by a factor of 2. So the first and second equations are responsible for shortening the time for the actual calculation, while the remaining equations are precalculated so we don't have to repeat the calculation every single time. 
$$P_n(f) = \frac{1}{2}[\frac{(c_\tau XC + s_\tau XS)^2}{c_\tau^2 CC + 2c_\tau s_\tau CS + s_\tau^2 SS} + \frac{(c_\tau XS + s_\tau XC)^2}{c_\tau^2 SS + 2c_\tau s_\tau CS + s_\tau^2 CC}$$
$$tan 2\omega\tau = \frac{2CS}{CC-SS}$$
$$c_\tau = cos\omega\tau, s_\tau = sin\omega\tau$$

$$XC = \sum_j X_j cos\omega t_j$$
$$XS = \sum_j X_j sin\omega t_j$$
$$CC = \sum_j cos^2 \omega t_j$$
$$SS = \sum_j sin^2 \omega t_j$$
$$CS = \sum_j sin\omega t_j * cos\omega t_j$$
- ! **IMPORTANT NOTE**: the above equations work only for the **single-term LS algorithm!** For the multi-term new equations would have to be derived. 


