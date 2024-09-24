TAGS: #mathematics #arithmetic #algebra 

So, we can start thinking about the [[Quadratic equation]] in terms of factoring numbers.

If we have a number, which is very close to a square, let's say 35, we can factor it as 5•7. And, if we notice that 36=6•6, we can see that 36-1=35, and (5+1)•(7-1) = 36. So:
$$n^2-x = (r+x)(s-x)$$
So, thinking about the quadratic equation where r and s are the solutions of the equation, or:
$$ax^2 + bx + c = 0$$
r and s are the x-intercepts, meaning they are on the x-axis of the [[Cartesian coordinate system]]. If we scale this equation down by dividing everything by a, and we look at the 2 solutions as r and s, we can see:
$$x^2 + b'x + c' = 0$$
And we can also see that putting in the r and s solutions:
$$x^2 - (r+s)x + rs$$
By this, we can see a few things:
1. $b'=-(r+s)$
2. $c'=rs$
If we go back to our starting example, we can notice that if we have a midpoint between r and s(let's call it m), it is equal to:
$$m=-\frac{r+s}{2}$$
And, if we think of r and s as distances from this midpoint, and their distance is d, we can think of this as the following:
$$r = m-d, s = m+d$$
$$c' = rs = (m-d)(m+d) = m^2 - d^2$$
$$d = \sqrt{m^2 - c'}$$
$$r, s = m±\sqrt{m^2-p}$$, where $p=c'$.

This is the **simple quadratic formula, because it gives the result we need without having to memorise everything!**

Okay. But let's try and derive the **normal quadratic formula**

$$ax^2 + bx + c = 0$$
$$x^2 + \frac{b}{a}x + \frac{c}{a} = 0$$
$$m = \frac{-b}{2a}$$, this is the midpoint from the previous derivation.
$$d =\sqrt{ m^2 - p} = \sqrt{(\frac{-b}{2a})^2 - \frac{c}{a}}$$
So, the quadratic equation is:
$$m±d =  \frac{-b}{2a} ± \sqrt{(\frac{-b}{2a})^2 - \frac{c}{a}}$$
$$m±d =  \frac{-b}{2a} ± \sqrt{\frac{b^2}{4a^2} - \frac{c}{4a^2}*\frac{4ac}{1}}$$
$$m±d =  \frac{-b}{2a} ± \frac{1}{2a}\sqrt{b^2 - 4ac}$$
$$m±d = \frac{-b±\sqrt{b^2-4ac}}{2a}$$

And this is it!!


