TAGS: #probability #mathematics 

Our world is random. And, we do not know what will happen sometimes, but we can use **probability** to infer the likelihood some event will occur. It is always between 0 and 1, 0 being impossible and 1 being certain. We denote probability with $p(A)$, where $A$ is some event which might occur. 

## Chance events
The most common example of probability is **tossing coins**. We have 2 possible outcomes, or our sample space: Heads or Tails(H or T). 

Probability in essence is dividing the number of events or outcomes we are looking into by the total sample space:
$$ p(A) = \frac{N(A)}{N}$$
In the case of a fair coin toss, we have a 50% chance of landing H or 50% chance landing T, mathematically. If we observed this coin tossing, it won't always be 50:50, but eventually, after many, many tossings, it approaches 50% each. We **theoretically** calculate the probability of this occurring is 50%, but **empirically** we observe that it might not be 50%!

In a weighted coin toss, we need to take into account the weight of each factor, maybe there is a 30% chance for T and 70% chance for H. If we were to keep track of these coin tosses by saying that T=0 and H=1, then we created [[Random variables]]. We can describe the behavior of our random variables by [[Expectation]] and [[Variance]]. 

## Terminology 
Each **trial** is called a **probabilistic experiment** which contains a few components. Each trial has it's **sample space**, or the number of all of the possible outcomes of our trial/experiment. We denote sample space with $Ω$, and our sample space has [[Set theory]] notation. For example, all of the odd numbers you can roll on a die are represented with the following sample space:
$$Ω={1,3,5} $$
**Events** are collections of elements in the sample space which we would like to observe or count in our probabilities. A basic set of rules called **axioms** guide probability. These are the [[Kolmogorov axioms]]! But there are other axioms other than the ones Kolmogorov mentioned. There is the axiom that *the sum of the probabilities of all the outcomes must be 1*. 
$$\sum_{ω∈Ω}P(ω) = 1 $$
## Strategies
There are 2 ways of going about solving for the probability of something occurring. We can tackle this with counting all of the outcomes where it does happen, using [[Kolmogorov axioms]] OR we can find the occurrences where our event does not happen and then substract this from 1!

## Properties
### Independence
2 events ae **independent** if eg. event A gives no information about event B and vice versa. 
$$P(A ∩ B) = P(A)P(B) $$
-> the intersection ([[Set operations with Probability]]) denotes that both events are happening and we need to calculate the probability for both of them

