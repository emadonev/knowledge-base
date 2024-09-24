---
tags:
  - math
  - mathematics
  - numbers
  - algebra
  - coordinate_systems
  - complex_numbers
---
When thinking about [[Imaginary numbers]] and the complex plane, which is very similar to the [[Cartesian coordinate system]], just that one axis is replaced with the imaginary number line, we come to the realization that we can plot a [[Unit circle]] onto this plane. 

It looks something like this:
![[unit circle complex.jpeg]]
We also know that if we ==multiply a number by an imaginary number, we effectively rotate it by **90º**==, hence we can draw a unit circle effectively. Now, using a bit of [[Fundamental trigonometry]], we can plot every point on this circle using the **angle**, $\theta$. 
![[complex coords unit circle.jpeg]]
So, the x component is equal to the cosine of the angle, while the y component is equal to i times the sine of theta.
- n Why do we have the sine with i, while the cosine just as cosine? Well, if we look at the definitions of sine and cosine, the cos of theta is part of the real number line so it is just cosine (we multiply by 1), while sin theta is part of the imaginary number line, so we have to multiply by i since it is the length of the hypothenuse

And now, there is something called **Euler's formula** which ties everything together:$$e^{i\theta} = i \; sin\theta + cos\theta$$
where *e* is a special constant, 2.71828... and theta is in [[Radians]]. Now, this formula seems elusive and different, but it is probably most famous for its look if the angle theta is equal to pi. Then, we would have walked around **half** the unit circle, so, the cosine is -1, while there is no imaginary part, hence:$$e^{i\pi} = -1$$

## Let's dive deeper...
---
While e might seem like a constant, it really isn't. It is a shorthand way of writing the **exponential function**, which is defined as such:$$exp(x) = \sum_{n=0}^\infty \frac{x^n}{n!}$$
The exponential function is a **series** where we add up fractions of factorials. (more about its definition later)

Now, the exponential function has a very specific and unique property:$$exp(a+b) = exp(a) *exp(b)$$
While this fact might seem shocking *and it indeed is*, let's go ahead and prove this lovely little statement which will help us think about this all.

- eg Let's start off with writing $exp(a+b)$ in a mathematical way:$$exp(a+b) = \sum_{n=0}^\infty \frac{(a+b)^n}{n!}$$ What can we see? Well, we are all familiar with the algebraic expansion of $(a+b)^2$ or $(a+b)^3$, and we can actually expand any *binomial* using the **binomial theorem** which is as follows:$$(a+b)^n = \sum_{k=0}^n \begin{pmatrix}n\\k\end{pmatrix} a^k b^{n-k}$$ The weird parenthesis is the [[Binomial coefficient]], which we will proceed to expand later. Now, let's fill in the original exp(a+b):$$exp(a+b) = \sum_{n=0}^\infty \frac{1}{n!} \sum_{k=0}^n \begin{pmatrix}n\\k\end{pmatrix} a^k b^{n-k}$$ Now, expanding the binomial coefficient and cutting with n! we get:$$exp(a+b) = \sum_{n=0}^\infty \sum_{k=0}^n \frac{a^kb^{n-k}}{k!(n-k)!}$$ The first part of the proof is finished. Now, how do we tackle the multiplying part? Let's first write out each one separately:$$exp(a) = \sum_{k=0}^\infty \frac{(a)^k}{k!}, \; exp(b) = \sum_{j=0}^\infty \frac{(b)^j}{j!}$$ Since both a and b are part of the same series (the k and j go in the same order), we can combine them together in a way that $j = n - k$, using the *Cauchy product*, which is just a fancy way of saying that we multiply everything with everything. $$exp(a)*exp(b) = \sum_{n=0}^\infty \sum_{k=0}^n \frac{a^kb^{n-k}}{k!(n-k)!}$$ And as we can see, the expressions are equal for both, and hence:$$exp(a+b) = exp(a) *exp(b)$$

Using this lovely property, we can write the exp(x) for any number as a way of summing different values. 
- n For example: $$exp(5) = exp(1+1+1+1+1) = exp(1)^5$$ or: $$exp(\frac{1}{2} + \frac{1}{2}) = exp(1) = exp(\frac{1}{2})^2 => exp(\frac{1}{2}) = \sqrt{exp(1)}$$

So, we can really write any form of the exponential function as:$$exp(x) = exp(1)^x$$ Which is a very useful quantity. We usually write for shorthand what the exponential function of 1 is equal to, and that ==is e==. $e = exp(1)$, which is why e is not a number, but rather a function!

## What about complex numbers?
---
Okay, great. We know what it is like to take a power of something, but, what is the **power of an imaginary number? What does it mean?**
- !! What does $$i^2, i^3, i^4$$ really mean?

Well, we return to the unit circle and imaginary numbers. As you may recall ([[Imaginary numbers]]), multiplying something by $i$ has the effect of rotating it by 90º across the complex plane. So, really, powers of $i$ are **rotations of something around the unit circle**. 

So, calculating $exp(i\theta)$ where $i$ is the imaginary number and $\theta$ is our real component, we can see from the image below how the imaginary component acts as a way of rotating a series of vectors whose vector sum is the value of $exp(i\theta)$. It is actually quite genius!

![[vector sum exp.png|300]]

