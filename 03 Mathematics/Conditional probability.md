TAGS: #probability #mathematics 

Conditional probability has access to some information about our system which might change the outcome of our [[Probability]]. 

>"*For example, we might expect the probability that it will rain tomorrow (in general) to be smaller than the probability it will rain tomorrow _given that it is cloudy today_. This latter probability is a conditional probability, since it accounts for relevant information that we possess."* - from Seeing Theory, brown university

So, technically speaking, it asks us to **shrink our sample space(remember, total number of combinations)** due to some specific parameters.

Let's look at an example!
> You have 3 seats in a classroom, and 3 children who could occupy it. Let's say your job is to calculate the probability that there will be at least 1 girl sitting in the 3 spaces. In normal probability, you would include **all of the possibilities** of children sitting like so. But in **conditional probability**, you know some **condition which focuses on the elements of the sample space which satisfy our condition.** Let's say that your condition is that 1 boy would never sit with 2 girls. 

The formula is as such:
$$P(A|B) = \frac{P(A∩B)}{P(B)} $$
This makes intuitive sense. If we want to calculate how likely is it for A to occur given B, we divide the number of combinations in both A and B by the total number of combinations in B.

We can apply this formula for [[Bayes's theorem]]!