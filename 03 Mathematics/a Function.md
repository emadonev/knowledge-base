---
tags:
  - mathematics
  - functions
  - graphs
  - coordinate_systems
  - calculus
---
# Covering the basics
---
>
> A **function** $f$ is a rule which assigns to each element $x$, part of a set $D$ exactly *one element*, $f(x)$ in a set $E$. $D$ is called the **domain of the function** (all possible inputs), while $E$ is the **range.** (all possible outcomes)
> 

![[function def.png]]

- elements of the domain are **independent** - we chose which one we would like to *transform* into another value, $f(x)$.
- elements of the range are **dependent** on the *element chosen from the domain*!

A function is described by its **equation**, or the way we transform a certain input into an output. We can present a **graph** of a function, as the set of all values such that: ${(x, f(x)) | x \;\epsilon \;D}$
![[graph of functions.png]]

We can define a function 4 different ways:
1. verbally (description with words)
2. numerically (a table of values)
3. visually (a graph)
4. algebraically (an explicit formula, such as $f(x) = ax+b$)

- !! A super important test which determines if a graph is a function or not is the **vertical line test** - if the line passes through more than 1 point, then it can't be a function!

- eg A function with *different definitions based on a subset of the domain* is called a **piecewise defined function.**

>An **even function** is one where $$f(-x) = f(x)$$, for example a parabola! In other words, these *functions are symmetrical via the y axis.*

> An **odd function** is one where:$$f(-x) = -f(x)$$, and these functions are *symmetric around the origin*

Finally, functions aren't static and over their domains they constantly **increase or decrease**. Hence, we define a function $f$ as increasing over some interval $I$ if:$$f(x_1) < f(x_2), \;\;x_1<x_2\;\epsilon\;I$$
And the function $f$ is decreasing if:$$f(x_1) > f(x_2), \;\;x_1<x_2\;\epsilon\;I$$

## Combining functions
---
There are many different types of functions, from *linear to polynomial, exponential, rational, logarithmic,...* and by conducting [[Transformations]] of functions as well as combine them, we can create ==interesting and unique new ones==. 

#### Translation
The first transformation we can do is *translation*. It is the act of moving or translating a graph across a [[Cartesian coordinate system]]. 
> $y = f(x) + c \ce{->}$  shifts the graph upwards
> $y = f(x) - c \ce{->}$ shifts the graph down
> $y = f(x+c) \ce{->}$ shifts the graph to the right
> $y = f(x-c) \ce{->}$ shifts the graph to the left

Now, these are simple enough. Whatever operation we do to $x$, we can easily shift it by addition or subtraction. 

#### Stretching / reflecting
Now, let's conduct some more serious transformations, where we really try to alter the shape. We can multiply the function by a constant, $c$ to stretch it out **vertically**. If we want to shrink it, the logical step is to **divide by $c$**! By multiplying/dividing *inside the parentheses* we can expand/shrink via the horizontal axis.

Finally, reflection is taking the same graph just reflecting about either the x or y axis. Multiplying by $-1$ either outside (x-axis) or inside the parentheses (y-axis) gives us the desired reflection. 

![[stretching reflection.png]]

#### Operations on functions
Other than pure transformations, we could also perform regular operations on functions, such as adding them together, multiplying, subtracting and dividing them together to create new functions. 

One more operation we can do is **composition of functions**, taking the function of a function:$$f(g(x))$$
We can also obviously **decompose a function**, which is super useful if we want to separate a huge function that is complicated into smaller functions.

# Exponential functions
---
These functions are defined as such:$$f(x) = b^x$$
For example, here is $2^x$. 
![[2x.png]]

There are 3 possible graphs depending on the constant, $b$. The function can either be decreasing, be constant if $b=1$ or increase (the most common)
![[expo functions.png]]

We can apply the same transformations to exponential functions as we did to linear and [[Polynomials]], and we determine the domain and range in the same way as well.

> NOTE: exponential functions grow **much more quickly than power functions**!

Here, in exponential functions, is where our good friend [[The number e]] comes in. It is described as a shorthand for an exponential function where it can be described as $e^x$. The ***slope of the exponential graph of $e$ is always 1***! The graph of $e$ is also called the *natural exponential function.* 

# Inverse functions
---
