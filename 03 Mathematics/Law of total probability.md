TAGS: #probability #mathematics 

This law allows us to break down the probability of an event by breaking it down into smaller scenarios which are mutually exclusive. 

Let's say we have a large set called S. Inside of S, we have events $B_1, B_2, B_3, ...$ Each of these events is mutually exclusive, meaning that only **one of these can occur**! So, for some event A, this law says that the probability of A is dependent on the different ways that the mutually exclusive events happen. 
$$
p(A) = \sum^N_{i=1} p(A∩B_i) = \sum^N_{i=1} p(B_i)*p(A|B_i)$$
So for every scenario of combinations that an event A can occur, we multiply the probability of that way by the [[Conditional probability]] of A such that $B_i$ has occurred. 