TAGS: #probability #statistics #mathematics 

Suppose X is a nonnegative [[Random variables]] and $a$ is a positive constant. Then:
$$P(X≥a) ≤ \frac{EX}{a} $$
This inequality tries to give an upper bound on the probability that a nonnegative random value takes on large values.

*Proof:*
- so the [[Expectation]] of the non-negative random variable X is really the sum of all the possible numbers it could be, multiplied by the probability of each value.
$$E[X] = \sum xP(X=x) $$
- bc X has to be positive, every time it is not, it contributes to the event where X is a very large value (a). 
$$E[X] = \sum xP(X=x, X≥a) + \sum xP(X=x, X < a) $$
- if $X≥a$, then $x$ must at least be $a$, so:
$$\sum xP(X=x, X≥a) ≥ \sum aP(X=x, X≥a) =$$
$$=a\sum P(X = x, X≥a) = aP(X≥a) $$
- therefore we have:
$$E[X] ≥ aP(X≥a)$$
- which we rewrite as:
$$P(X≥a) ≤ \frac{EX}{a} $$
