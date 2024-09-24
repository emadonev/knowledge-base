TAGS: #mathematics #series #algebra #polynomials 

A **Taylor series** is a series which tries to approximate a complex function using ever higher degrees of [[Polynomials]]. 

The fundamental function looks like this:
$$ f(x) = a + b(x-c) + d(x-c)^2 + e(x-c)^3 + ...$$
Where the constants (a, b, c, d, e, ...) are most commonly **factorials**. 

The Taylor series is useful for
- optimizing algorithms
- approximating functions
- understanding error and stability (we use the series to calculate errors)
- and for machine learning algorithms.

## Step-by-step process of forming a Taylor series

1. Choose a function: $f(x) = e^x$, and we will expand it around the point x=0
2. The function for building a Taylor series around a point looks something like this before we start building it:
$$ f(x) = f(a) + f'(a)(x-a) + \frac{f''(a)(x-a)^2}{2!} + \frac{f'''(a)(x-a)^3}{3!} + ...$$
3. **0th approximation**
	1. We choose x=0 as our point
	2. $f(0) = e^0 = 1$
	3. $f_0(x) = 1$
4. **1st order approximation**
	1. The first derivative of $e^x$ is $e^x$
	2. $f'(0) = e^0 = 1$
	3. $f_1(x) = 1 + 1*(x-0) = 1+x$ - the first element is a horizontal line, then we add a linear equation where we only have x as an element, etc.
5. **2nd order approximation**
	1. The second derivative of $e^x$ is also $e^x$. 
	2. $f''(0) = e^0 = 1$
	3. And we keep building: $f_2(x) = 1 + x + \frac{1*(x-0)^2}{2!} = x + \frac{x^2}{2}$
6. We continue do build higher orders, and the sequence continues like so:
$$ e^x = 1 + x + \frac{x^2}{2} + \frac{x^3}{6} + \frac{x^4}{24} + ...$$

*"When you take the derivative of a function like x^n, you get n * x^(n-1), and when you take the derivative again, you get n * (n - 1) * x^(n-2), and so on. After taking the derivative n times, you end up with a factor of n!, the product of all integers from 1 to n."* - ChatGPT