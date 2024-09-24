TAGS: #variable_star #star #astronomy #computer_science #programming #mathematics 

There are numerous ways to classify variable stars, and here we explore *all of the methods recommended by top scientists*, which are covered in various research papers and/or textbook chapters. 

# PCA ANALYSIS
--------
<mark style="background: #FA9500;">Unsupervised learning</mark> is a type of computer learning where we have a set of inputs $X, X_1, X_2, ... X_n$, and an $m$ amount of observations. We are not looking for predictions of something, rather we are trying to *find interesting trends in the data* using [[Statistics]] and [[Statistical thinking]]
$\ce{->}$ this kind of learning contains 2 major methods: **PCA analysis** and **Clustering**.

Links: [Medium](https://towardsdatascience.com/principal-component-analysis-pca-explained-visually-with-zero-math-1cbf392b9e7d), [Satorious](https://www.sartorius.com/en/knowledge/science-snippets/what-is-principal-component-analysis-pca-and-how-it-is-used-507186#:~:text=Principal%20component%20analysis%2C%20or%20PCA,more%20easily%20visualized%20and%20analyzed.),  [In depth: PCA](https://jakevdp.github.io/PythonDataScienceHandbook/05.09-principal-component-analysis.html)

### PCA Analysis
------
In PCA analysis we have elements called<mark style="background: #F2DDA4;"> principal components</mark>, which summarize all of the correlated variables (datapoints) into a small set of trends. 
- pr being able to visualize very complex data, let's say 7010 light curves where each one has around 200 or 500 observations would require an enormous amount of plots and I wouldn't get much out of it. So, finding a way to reduce the number of dimensions in this data so I can just have a 2D plot of everything would be invaluable. This is exactly what PCA does

- eg The first principle component is a normalized linear combination of the starting features: $$Z_1 = \phi_{11}X_1 + \phi_{21}X_2 + ... \phi_{p1}X_p$$, where $$\sum_{j=1}^p \phi_{j1}^2 = 1$$$\phi$ is called a *loader*, and all of the phi's together make up a *loading vector*. We normalize these loading so the variance would not become arbitrarily large. Each one of the loadings define how much the original variables contribute to the first component, they define the direction of the vector and how each point shapes the components. 

	- n "*The constraint ensures that the loadings are normalized, meaning their squares sum up to one. This constraint is important because it prevents the trivial solution where the loadings could grow arbitrarily large, leading to an artificial increase in explained variance. Normalizing the loadings makes sure that the variance of each principal component is the actual variance along that direction in the space.*" - chatGPT
- we always make sure that the original datapoints are normalized so their mean is 0. This way we maximize the variance, and nothing else. 

- eg The second principle component is a linear combination of our starting features that has an uncorrelated maximum variance with $Z_1$. 

Both of the principal components try to measure the [[Variance]] of the data, and then remove anything which doesn't give a lot of information. **Variance is key information**, and it is extremely useful for this stuff. 

![[PCA.png]]
Here we have the first principal component (longer line), and the second principal component (shorter line).
- n *"These vectors represent the _principal axes_ of the data, and the length of the vector is an indication of how "important" that axis is in describing the distribution of the data—more precisely, it is a measure of the variance of the data when projected onto that axis. The projection of each data point onto the principal axes are the "principal components" of the data."* - [In depth: PCA](https://jakevdp.github.io/PythonDataScienceHandbook/05.09-principal-component-analysis.html)

# Active learning to overcome sample selection bias: application to photometric variable star classification
-------
> *Joseph W. Richards, Dan L. Starr, Henrik Brink, Adam A. Miller, et al.*

The researchers in this paper state that there is a very big problem when it comes to [[Machine learning]], that many models are <mark style="background: #A3C4BC;">biased</mark> because their training data is only comprised of high-brightness, close [[Variable stars]], while the testing data comprises of deeper surveys. Since many don't use <mark style="background: #F2DDA4;">deep surveys for training the model</mark>, they are not very good models. 
-  remedies to <mark style="background: #EB6424;">Sample selection bias</mark>
	- eg when our sample isn't representative of our population! ([[Population and sample]])
	1. Importance weighting
		1. eg This is when you give different weights to different elements in your sample so they can be more representative of the population if you know the [[Probability distributions]] of each.
	2. Co-training
		1. n "Let's say you're trying to classify web pages, and you have both the text of the page and the links on the page as separate views. You might have a small set of web pages that are labeled as either "sports" or "not sports". You can train one classifier on the text and another on the links. Each classifier can then label the unlabeled pages, and the most confident labels can be added to the training set of the other classifier." - ChatGPT
	3. [[Active learning]]

# Automated classification of variable stars for All-Sky Automated  Survey 1-2 data
-------
> L.Eyer & C.Blake

In this research paper, the researchers used [[Fourier transforms]], or well the Fourier decomposition coefficients and a <mark style="background: #F2DDA4;">Bayesian classifier</mark>, to automatically classify large numbers of light curves. In another research paper [[Light curve analysis of variable stars using Fourier decomposition]], it was said and shown that Fourier decomposition is much, much slower for PCA, and the accuracy is only very slightly better, so we should use **PCA** instead of **Fourier** for this project (Since there are around 5024 stars to work with). 

- n "*We used the algorithm given by Press et al. (1992), in its fast version called <mark style="background: #BABD8D;">FASPER</mark> . The algorithm has two parameters, which fix the resolution in frequency and the highest frequency searched. The first, OFAC , was set to 6 while the second, HIFAC , was changed according to the properties of the light curve and of the sampling. In FASPER , the highest frequency searched is computed given the time intervals, the number of data points and the ad hoc factor multiple (HIFAC ) of Nyquist frequency, as defined by Press et al. (1992). This factor is needed because short periods can be detected even if the data have large time gaps between measurements.*" - Eyer and Blake

A great way to find out how many <mark style="background: #F2DDA4;">harmonics are needed for a light curve fit</mark> is to determine the first solution using 1 harmonic - then we up it to 2 harmonics, compare the 2 models, and if inadequate, we add another harmonic, etc. until we reach the desired amount of harmonics needed. 

- eg The researchers use a **Bayesian classifier**, which requires an input of the [[Probability distributions]]. 

They managed to classify 5 different types of stars, but they classified only little due to the significant errors in the samples. They mention that a **logAmplitude and logPeriod graph** is very insightful! 

# Automated supervised classification of variable stars
--------
> J. Debosscher et al.


# Improved methodology for the automated classification of periodic  variable stars
-------
> J. Blomme, L.M. Sarro, et al.

The researchers in this paper claim to have found a new methodology for classifying variable stars using Bayesian statistics and a multistage approach. 

- n *"The aim of supervised classification is to assign to each variable target a probability that it belongs to a particular pre-defined variability class, given a set of observed parameters."* - the paper

What is different in this algorithm is that the categories of light curves are made into a tree format, thereby being more efficient as each light curve follows a path down the tree to a specific category or class. 

The authors use a **Gaussian mixture classifier**, which uses [[Bayes's theorem]] as a base. 
$$P(C=c_i | A=a) = \frac{L(A=a | C=c_i)P(C=c_i)}{\sum_{i=1}^{N_c} L(A=a|C=c_i)P(C=c_i)}$$
And we can simplify this expression where $C=c_i \ce{->} A$ and $A=a \ce{->} B$ .
$$P(A|B) = \frac{L(B|A)P(A)}{\sum_{i=1}^{N_c} L(B|A)P(A)}$$
- eg what this formula is trying to sat that the probability of a light curve to be part of a class $c_i$ with observational evidence $a$, is the conditional likelihood of our attribute $a$ to belong to a variability class $c_i$ and the probability of the light curve being part of $c_i$ divided by the sum of the numerator for every classification class.

- n *"The EM algorithm is an iterative method for calculating maximum likelihood estimates of parameters in probabilistic models, where the model depends on unobserved latent variables. EM alternates between performing an expectation (E) step, which computes the E of the log-likelihood evaluated by using the current estimate for the latent variables, and a maximization (M) step, which computes parameters maximizing the expected log-likelihood found in the E step. These parameter estimates are then used to determine the distribution of the latent variables in the next E step".*

The researchers trained the multistage tree using previously confirmed light curve types. There were many categories, some with a lot of examples and some with few.

![[improved_meth_lc_class.png]]
$\ce{->}$ the multistage tree

- n "*We only computed up to two significant frequencies with each up to three harmonics, which in our experience is sufficient for classification purposes. "* - paper
- eg **Significant frequencies** are all frequencies in the [[Lombe-Scargle periodogram]] which are significantly higher than the other frequencies
- eg **Harmonics** of light curves are all the other frequencies which build up the fundamental frequency. They add nuance to the light curve shape.

The classifier was succesful, and the researchers were happy with the results. They noted that some star types could not be found because no color information was provided, which might also cause a problem in the [[VARIABLE STAR PROJECT]]. 

# ON MACHINE-LEARNED CLASSIFICATION OF VARIABLE STARS WITH SPARSE AND NOISY  TIME-SERIES DATA
---------
> Joseph W. Richards, Dan L. Starr, et al.


# Random forest automated supervised classification of Hipparcos periodic variable stars
--------
> P. Dubath, L. Rimoldini, et al.


# PCA analysis and Fourier decomposition
-------
> Sukanta Deb, Harinder P. Singh

[[Light curve analysis of variable stars using Fourier decomposition]]

# PCA analysis of RR Lyrae stars
-------
> S.M. Kanbur and H. Mariani - [[PCA of RR Lyrae.pdf]]

- the researchers found that the PCA method is supremely better than the fourier method
	- it is faster
	- there are less errors
	- less computation power is needed

- n "*An adequate Fourier description requires, at best, a fourth-order fit or nine parameters, whilst a PCA analysis requires only three or four parameters with as much as 81 per cent of the variation in light-curve structure being explained by the first parameter.*" - from the research paper

- using fourier transforms we can reconstruct the light curve using Fourier coefficients:
$$V = A_0 + \sum_{k=1}^{k=N} [a_k cos(k\omega t) + b_k sin(k\omega t)]$$
- using PCA analysis we build the light curve based on *elementary light curves*:
$$V(t) = PCA1 L_1(t) + PCA2 L_2(t) + ...$$
- PCA is determined via the whole database, while Fourier has to be individual light curve analysis: this is one of the many benefits of PCA
- the first 4 components should be enough to explain almost 99% of the light curve data.
- PCA curve is smoother than the Fourier curve describing light curves