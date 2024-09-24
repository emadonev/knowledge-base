TAGS: #mathematics #probability 

This theorem proposes that the ==sample mean==([[Collecting a sample]], [[Population and sample]]) of a large enough number of random variables is an approximately normal [[Distribution]]. This means that it looks like a perfect curve. 

How do we get to this? The step-by-step process
1. We start with a [[Random variables]]! (X)
2. We are taking N samples of this variable, and adding the result they give (eg. 1 or -1 if X has 2 choices)
3. From this we get that the [[Distribution]] of the sum approaches a [[Normal distribution]] as N approaches infinity. 

As we gather more samples (N approaches infinity), the mean([[Statistical functions]]) and the [[Standard deviation]] change. The more samples we gather, the mean is pushed to the centre, because it is equal to $Nµ$, where $µ$ is the mean of the original distribution for our [[Random variables]]. The standard deviation gets larger the more $N$ we have, because of the properties of [[Variance]]. Since the variance of 2 random variables together is the same as the independent variances, we know that the standard deviation of each of the samples, N times, is $std^2(x_1+...+x_N) = N*std^2x_1$, meaning that the standard deviation increases by a factor of $\sqrt{n}$! 

![[central_limit_1.png]]

## Unpacking the formula for the normal distribution!

If we take any number to the power of x, it is going to be exponential. If the exponent is **negative**, it is going to show exponential **decay.** In order to make it work on both sides **and** have a smooth curve at the top, we use **squaring!**. 
![[central_lim2.png]]
Now, we need to be able to change the graph so it fits the data! We can do this by adding a constant to e, and since the standard deviation changes with the normal distribution, the exponent now has $-1/2(x/std)^2$. In order to make the area under the curve 1, we need to divide this whole expression by $\frac{1}{std\sqrt{2π}}$. Why this? Because the area under the curve is actually $\sqrt{π}$ (explanation later),and we need to divide by $std\sqrt{2}$ because that is how the graph stretches. We also add $µ$ to the x component, because we want to be able to shift the graph according to the mean.

The official equation, or statement, for this theorem is the following:
$$lim_{N->∞} P(a < \frac{(x_1+...+x_N)-Nµ}{std*\sqrt{N}}<b) = \int^b_a \frac{1}{\sqrt{2π}}e^{\frac{-x^2}{2}}dx $$
>As the size of the sample approaches infinity, the probability of the sum of all the outcomes where the standard deviation is 1 falls between 2 values, then it is equal to the area under the curve of a standard [[Normal distribution]]. 

![[clt_3.png]]


### Why is pi in the formula?
So, let's take the equation $e^{-x^2}$. If we were to calculate the [[Integration]] in the image above, it is proven to be impossible. So we need another strategy. Let's add another dimension!

By adding another dimension, we get coordinates x, y and the radius r from the z axis.
![[clt4.png]]
![[clt5.png]]
Ok. Now let's try to calculate the volume beneath the sphere. So, the most logical way to do this is to separate the volume into a bunch of tiny cylinders where each one has volume. And, since we have a factor in the integral, we can solve it! After solving the integral, we get that the volume is π!
![[clt6.png]]
![[clt7.png]]
 So. Now let's get back to the volume calculation. There is another way to do this! instead of going about the vertical axis, let's go about the y axis. So we can divide this volume into slices which have a tiny thickness, and we get that it is the square of the area of each component. Hence, the area under the normal distribution is the square root of pi.
 ![[clt8.png]]
 ![[clt9.png]]
 
## Why is the function $e^{x^2}$?
We are going to show this via the Herschel-Maxwell derivation.
There are 2 properties which we want to achieve in this derivation. The first is that the probability density depends only on the distance from the origin (0,0). So, this is essentially the radius or $r$ from the previous section. This formula explains the concept before:
$$f_2(x,y) = f(r) = f(\sqrt{x^2 + y^2})$$
The second property is that both x and y are **independent of each other.** This means the following: each value (x and y) can be factored as a separate function!
$$f_2(x,y) = g(x)h(y) = g(x)g(y)$$
This is important, because separating the 2 coordinates is super useful later. Also, if we look at $f(r)$ and $g(r)g(0)$ we can notice that they are the same and the only difference is a constant. 
> A useful note and tip! When solving these types of problems, it is always useful to assume that the constant is some value which suits us (like 1 in this example) and then later we rescale so that the numbers work out! 

Using the tip above, we can say the following:
$$f(r) = f(x)f(y)$$
This is called a [[Functional equation]]. We can begin to solve this by using a helper function.
$$h(x) = f(\sqrt{x}),h(x^2) = f(x)$$
Okay, so let's write out the same thing for our r value:
$$h(x^2 + y^2) = h(x^2)h(y^2)$$
We can see that no matter how many variables we add in the first part, the behaviour stays the same.
$$h(x_1 + x_2 + ... + x_n) = h(x_1)h(x_2)...h(x_n)$$
Using this we can conclude that:
$$h(n) = b^n$$
Using this same logic, we can assume that this works for all rational numbers. And since rational numbers are continuous, it says that h is an exponential function. Now due to [[Euler's formula]], mathematicians love using the constant $e$ since in [[Calculus]] and in taking the [[Derivative]], it makes things a lot easier! So, instead of $b$ we write the following:
$$h(x)=e^{cx}$$
Where $c$ is some constant. Since $h(x^2)=f(x)$, then:
$$f(x)=e^{cx^2}$$
Now, since we assumed at the beginning that our constant is 1, we have to rescale it back so the volume under the curve is 1. If our constant, $c$ is a positive value, the function *blows up to infinity in all directions, meaning that the constant **must be negative.*** The value of this constant determines the spread of the distribution. 

## Why is the central limit a normal distribution?
Okay. We have finally reached the conclusion of the theorem! Why is it a normal distribution? This is the key question, and [[Convolutions]] might help :)

Let's start with the same process as in convoluting 2 random variables together. So, we draw the x and y axis, and we get that the graph is **rotationally symmetric, meaning that we only need r to graph it because both functions are normal distributions.**
![[clt_why.png]]
So, now let's work on a little visual trick. If we take a slice of this, we can see that it is $s√2$ distance from the centre. We can rotate this, so that we can calculate the area **only depending on the y axis!!** This makes things so much easier, since the x part is constant.
$$Area = \int_{-∞}^∞ e^{-x^2}e^{-y^2} dy = \int_{-∞}^∞ e^{-(s/√2)^2}e^{-y^2} dy =  e^{-x^2}\int_{-∞}^∞e^{-y^2} dy$$
Now, due to the Herschel-Maxwell derivation, we know that:
$$Area = e^{-(s/√2)^2} √π = Area = e^{-s^2/2} √π$$
What this formula says that the **product of 2 normal distributions gives a normal distribution!!** 

### Assumptions which make this possible
1. All of the variables we are adding together **are independent of one another!**
2. Each variable is drawn from the same distribution.
3. The variance we computed has to be finite!

