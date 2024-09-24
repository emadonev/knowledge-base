TAGS: #probability #mathematics #statistics #random 

## Standard definition
This quantity of both [[Statistics]] and [[Probability]], tells us how spread out the [[Distribution]] of values of our random variable is. When using various [[Data types]], we can describe their distribution and their variance. This is accomplished by the following formula:
$$S = \frac{\sum (x- µ)^2}{n} $$
It sums up all of the squared differences between the current value and the Arithmetic mean([[Statistical functions]]), dividing it by the number of data points for an average value. The square root of variance is the [[Standard deviation]]. 

## Random variables
Formally, it is described as:
$$Var(x) = E[(X-E[X])^2] $$
Average value of the squared difference between the random value and it's expectation or average. You can notice the striking similarity between the standard definition and the [[Random variables]] definition! So what variance basically does it calculates the average distance between X and it's mean. 

If we were to calculate the **running average** as we go along our probabilistic settings, we can see that over many, many trials, the running average of squared distances begins to resemble the **true variance**. 

### Properties of variance
1. $Var(X) ≥ 0$
- *proof*: self explanatory. it is always positive because of the square!
2. $Var(cX) =  c^2Var(X)$ 
- *proof:*
$$Var(cX) = E[(cX − E[cX])^2] = E[(cX − cEX)^2] = E[c^2(X − EX)^2] = c^2Var(X) $$
3. $Var(X) = E(X)^2 - E(X)$
4. $Var(X+Y) = Var(X) + Var(Y)$

![[variance_prop.png]]

