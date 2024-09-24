TAGS: #probability #mathematics 

This number tries to calculate the center of the random variable's [[Distribution]]. It is sort-of an average (on the long run), considering it takes many, many eg. rolls of a dice to reach this expectation. If we wanted to take a weighted average, we multiply each outcome ([[Random variables]]) by its probability.


If we would try to calculate the average of all the outcomes we get by rolling dice, we would get the same result as a weighted average of probabilities! This is called the **expectation**.

![[expectation_dice.png]] *The expectation converges around 3.5*

It is defined as the probability-weighted sum of all the possible values of a random variable:
$$E[X] = \sum xP(x) $$
### Properties of expectation
1. If X and Y are 2 random variables, the expectation of both of the variables is the same as if we added the expectation of each.
$$E(X+Y) = E(X) + E(Y) $$
2. If X is a random variable and c is a constant then:
$$E(cX) = cE(X) $$
-> *proof*: follows directly from the formula for expectation
3. If X and Y are independent random variables, then
$$ E[XY] = E[X]E[Y] $$
