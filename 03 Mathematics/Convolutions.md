TAGS: #mathematics #convolution #probability #statistics 

# Adding random variables together
*QUICK NOTE: all the [[Random variables]] are independent.*

## Discrete random variables
Adding 2 [[Random variables]] with different [[Distribution]]s is actually not that hard! With some simple [[Probability]] rules, we could have an answer in no time! 

There are 2 possible ways at going at this, the easier to maybe understand, but harder computationally way (with diagonals and 2D plots) but this gets complicated with more than 2 random variables. We also have a much **simpler and more efficient solution: *convolutions!*** 
![[convo_eg.png]]
Let's say we have 2 random variables written as functions: $P_X, P_Y$. When we add them together we get $P_{X+Y}$. Now, each function has a different distribution, where every possible value has some probability. If we want to go over all the possible combinations, we first flip the distribution of the second variable, and then we start doing a **dot product**, in other words we multiply each probability from X to one in Y, and then add them all together. 
![[convo.png]]
This process of adding them all together is called a **==convolution!!==**

But how would we write this down mathematically? 
$$P_{X+Y} = [P_XP_Y]$$
Or, if we were to expand this we could write it as so:
$$P_{X+Y} = [P_XP_Y](s) = \sum^n_{x=1}P_X(x)*P_Y(s-x)$$
This makes a lot of sense! So we have an $n$ number of options to begin with (like rolling dice, we have 6 options), and then we start from 1 and we go to the max number in the distribution. We sum every product of 2 probabilities for every column. The first factor is $x$, or the roll of the $X$ die, and then the $Y$ die must roll some value which when added to $x$ produces the desired sum $s$. 

> Quick note! You might notice that in this formula, if the sum is sufficiently low, then we get negative values for $s-x$, which is impossible if it is not one of our starting options. In this case, we assume that all values which we cannot get *get a value of 0, so the probability is in turn 0.*

## Continuous random variables
In these cases, our random variable can take up **any number!** Since this is a continuous infinity, it can take up any number.  
![[convo_expo.png]]
So the formula for the continuous case is almost the same as for the discrete case, however since we are dealing with a continuum, we use integrals. So, the formula is like so, and we shall break it down.
$$[f*g](s)=\int_{-∞}^∞ f(x)g(s-x)dx$$
So, the first part, $f$ is the [[Probability density function]] of the first distribution. Analogously, $g$ is the PDF of the second distribution. So, if we were to graph this stuff:
![[convo_expo2.png]]
So, the input to the final function would be s, and the output the product in the last graph!

But what if we want to add more than 2 random variables? Let's start with 3. So, we can add the first 2 and then let's add that to the 3rd function. We can repeat this process many, many times, and the more iterations it has **the more it approaches the [[Normal distribution]]**! This **is the [[Central limit theorem]]!!!** 

But, how do we apply the diagonal situation for the discrete case to the continuous case? Well, we can think of plotting the x and y coordinates on a 2D plane and then graphing into 3D space the probability density. 
![[convo_3.png]]
We can look at our desired sum to *be the diagonal here!*
![[convno_5.png]]
And now, if we look at the slice, or the area under the curve, **we see that it is exactly the same as the product of the 2 functions (just larger by a factor of √2, but that's just due to the rescaling in a 2D graph.)** 
	![[convo_4.png]]
And that's it!


