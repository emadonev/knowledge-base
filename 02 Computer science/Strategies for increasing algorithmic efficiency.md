TAGS: #computer_science #data #data_analysis #programming #algorithm 

> How can we accelerate our programs?

1. **[[Trees(programming)]]**
	1. chop up space into nodes
	2. prove that some parts can be ignored or approximated
	3. use the remainder to chop it up again
	4. finally infer from the data your answer
2. **Subproblem reuse**
	1. using techniques to reuse parts of code or things the program learned so it's more efficient
	2. [[Dynamic programming]] and [[Memoization]]
3. **Locality**
	1. making sure that the computation is not limited by the computer itself. 
4. **Streaming**
	1. downloading and using an entire massive dataset is unfeasible, so we use *streaming*, or constantly taking a new data point at a time
	2. [[Stochastic programming]] and [[Online learning]]
5. **Function transformations**
	1. transforming our starting function into a new one which is easier to compute and requires less power. 
	2. [[Taylor series]] and [[Fourier transforms]]
6. **Sampling**
	1. reducing the amount of data points analyzed at a time.
	2. [[Active learning]]
7. **Parallelism**
	1. speeding up a computation by simultaneously working on multiple parts of the code of a computation
8. **Transforming the problem**
	1. if nothing works, rework the problem in a different form which might be solvable