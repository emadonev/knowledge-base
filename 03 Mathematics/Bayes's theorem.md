TAGS: #probability  #statistics #mathematics 

This type of [[Statistics]] and [[Probability]] is when we use current observations to alter our predictions and probabilities. Our prior probabilities and beliefs should be updated based on new info!

The theorem is stated as such:
$$P(A|B) = \frac{P(B|A)P(A)}{P(B)} $$
The $P(A|B)$ sign means its part of [[Conditional probability]], or **The probability of A given B.**

Assumptions: A is a subset of a total sample space, Ω. B is not a perfect subset of A, meaning it is not fully enclosed in A. 

We can prove this using Conditional probability. 
1. We have the identity of conditional probability:
$$P(A|B) = \frac{P(A∩B)}{P(B)} $$
2. Similarly, we can apply this formula for $P(B|A)$
$$P(B|A) = \frac{P(A∩B)}{P(A)}$$
3. If we multiply both sides by $P(A)$, then
$$P(B|A)P(A) = P(A∩B)$$
4. Plugging this back into our first equation, 
$$P(A|B) = \frac{P(B|A)P(A)}{P(B)}$$

An important note is that while this formula is correct, it is difficult to calculate and know this stuff. So let's break it down.

We can rewrite this as:
$$P(A|B) = \frac{P(A)P(B|A)}{P(A)P(B|A + P(¬A)P(B|¬A))}$$
This means the following:
- Numerator: we multiply the original [[Probability]](proportion) by the "likelihood" of our evidence holding in the hypothesis group, or the probability of elements of A being part of B also.
- Denominator: we have to account for the probabilities of our hypothesis and for against our hypothesis! So first we multiply the original probability(proportion) of the hypothesis or set A by the probability of our evidence holding in the hypothesis group, or the probability of elements of A being part of B also. To that we add the probability(proportion) of elements which are not part of the hypothesis, or well A by the probability of our evidence not holding for our hypothesis. The image below might help with this description!!

![[bayes_theorem.png]]
![[bayes_theorem2.png]]
## When to use this theorem?
We use this theorem when we have a **hypothesis**, and we gain some **evidence**, and we want to see the probability of our hypothesis being true based on our evidence.

