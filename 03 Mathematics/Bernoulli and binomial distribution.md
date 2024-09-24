TAGS: #probability #combinatorics #mathematics 

Any random trial or experiment where the outcome can be either a success or a failure is called a Bernoulli trial. It is important to note that the probability of success is the same for every trial! It works like this:

If the probability of success is $p$, the probability of failure is the complement of this probability([[Set operations with Probability]]), or $1-p$. When $T$ consecutive trials are performed, the number of successes(N) is distributed as so:

$$
P(N=n) = \begin{pmatrix}T\\n\end{pmatrix}p^n(1-p)^{T-n}
$$
This is a **binomial distribution** because of the nature of the trials. We only have a Yes or No answer, so it is **binomial**. The coefficient represents the number of ways to choose n successes out of T trials. $p^n$ represents the probability of getting n successes in all the trials. Finally, $(1-p)^{T-n}$ represents the probability of getting a failure for all the trials. Since we have $n$ successes, then there **must be $T-n$ failures**. 

Another way to think about this formula is:
$$P(data|s) = cs^{sucess}(1-s)^{failure}$$


A **negative binomial random variable** counts the number of successes in the Bernoulli trials **before $r$ failures occur!** 
$$f(x;n,r,p) =  \begin{pmatrix}x+r-1\\x\end{pmatrix}p^x(1-p)^r$$


