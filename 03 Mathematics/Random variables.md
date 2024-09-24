TAGS: #random #probability #mathematics 

A **random variable** is a variable to which a numerical value was assigned which is the outcome of a chance event (it was picked at chance). Another way of defining this is to say that a function which maps outcomes in the sample space to real numbers is called a **random variable.** 

Let's say we are flipping a coin 5 times. I can quantify that there are 2 possible outcomes for each coin toss: heads or tails. I can create a **sample space** of all the possible combinations that could occur. The **randomness** of this example is the **number of observed heads or tails in the 5 flips.** 

We have to distinguish **random events from random variables**. Random events are those which occur once, like winning a lottery, sharing a birthday with a person in your class, or selecting an ice cream flavor with your eyes closed. However, when random events have numbers related to them, they are by definition a random variable.

Let's look at an example.
*(From brilliant)*

Let ${H,T}$ be the sample space for a single fair coin flip. H and T are not random variables, but if we assign the number **1 to H** and the number **0 to T**, then we've just created one:
$$
X(H) = 1, X(T) = 0
$$
We can compute the probability of heads or tails occurring (50%), but we **do not know which will happen**. All of these are **discrete random variables**.

**Continuous random variables** are those which we continuously measure. This might be the velocity of an air molecules in a closed space. These variables are any values which can be from a range of values. 

#### Example:
> Let's say we pick a value $x$ the following way:
> $$ P(a ≤ x ≤ b) = b-a$$
> And we now have a **random variable Y**:
> $$Y = 2x + 5 $$
> What is the probability of:
> $$ P(6 ≤ Y ≤ 7) = ?$$
> So the 1st step is to see the minimum and maximum values of $x$ by substituting 6 and 7 instead of $Y$ in the equation for $Y$.
> From this we get that:
> $$ P(1/2 ≤ x ≤ 1) = 1 - 1/2$$
> And from here we get that the probability is $1/2$. 


In essence, we have all of these random chance events happening in our lives. While we **can never know exactly what will happen in these events**, we can calculate the **[[Probability]]** of some random event occurring. All a **random variable** does is quantify the possible outcomes of our chance event. So we have option A or B, $A=1$ and $B=0$ are random variables, because we have assigned some value to them.
