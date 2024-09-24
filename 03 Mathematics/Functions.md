TAGS: #mathematics #functions #numbers 

Functions are a process which take in input, run through the process, and produce an output. For every input there exists a specific function (unless the output is undefined). We can graph functions in a [[Cartesian coordinate system]]. We use the notation $f(x)$ to represent a function, with $x$ as the input, and $f(x)$ as the output. $f(x)$ can be equal to any equation we want(without random factors). We can test if a graph represents a function using the **vertical line test**. 
![[vertical line test.png]]
Other than $f(x)$, we can use $y$ to represent the output *(x is the input, y is the output)*. 

## Parameters of functions
Parameters are constants in functions, but they alter how the functions behaves. Each function in its equation has many different parameters, the most famous being the [[Linear function equation]]. 

## Domain and Range
Not every input is valid for every function. A function can be undefined, or the output is not possible for every function. The **domain** is a set of inputs which have valid results for the function. The **range** is the set of all possible outcomes for a specific function.

## Translating  and stretching functions
We can translate functions across the plane (vertically or horizontaly), using the following expression:
$$ f(x-h) + k$$
Where increasing $h$ will move the graph to the right, and decreasing it will move it to the left. $k$ will move it up or down!

$$ a*f(b(x-h)) + k$$
For any point starting at (0,0), the new vertex is at (h, k). $a$ modifies the output of the function, $b$ modifies the input to the function by dividing the x-coordinates, $h$ shifts the values left or right and $k$ shifts the values up or down. 

>For example: $$f(4x+3) + 3$$gets turned into:
>$$ f(4(x + \frac{3}{4})) + 3$$
> So $a=1$, $b=4$, $h=\frac{3}{4}$ and $k=3$.

**X-coordinates**: divided by $b$ and then $h$ is added
**Y-coordinates**: multiplied by $a$, and then $k$ is added

## Reflections and symetry

1. $-f(x)$ flips with respect to the x-axis
2. $f(-x)$ flips with respect to the y-axis
3. $f(x) = f(-x)$: y-axis symetry

#### Even functions
Functions whose graphs are symetric about the y-axis.

#### Odd functions
Dunctions which are symetric about the origin and do not change (look the same upside down as right side up).

## Inverse functions
These types of functions swap the input and output values. If a function has (x,y) points, the inverse has the points (y,x). 

If we draw a horizontal line through a function's graph, and it only crosses it at most once, then an inverse exists which is definitely a function.

>Example: 
 >$$ f(x) = 2x+3$$
>Inverse is:
>$$g(x) = \frac{x-3}{2}$$

Inverses are the reflections over the line y=x, it is like a line between the inverse functions and symetry is present. 

## Composition
A composition of functions is when we chain more functions together so that the output of one is the input of the next one, kind of like a train! Each wagon is a function, transferring its output into the next function.

>Eg.
>We can have 2 functions: 
>$$g(x) = 2x,h(x) = x+5 $$
>We can chain these 2 functions together using the following notation, where first we need to solve $g$ and then $h$.:**the nested parentheses version**
>$$ h(g(x))$$
>Or in this common way of notation: We go from right to left
>$$(h∘g)(x)$$

We can work backwards from our composition to regain the original function if we know how both look like.

## Compositions as Transformations
Using compositions we can also make transformations to our functions! We can stretch and move them, depending on how we chunk the functions like lego blocks. 

~ from Brilliant

To summarize, given a function f,

- using $g(x)=ax$ and the composition $g(f(x))$ **multiplies** the vertical dimension by a scale factor of $a$
    
- using g$(x)=bx$ and the composition $f(g(x))$ **divides** the horizontal dimension by a scale factor of $b$
    
- using $g(x)=x+k$ and the composition $g(f(x))$ shifts the graph **vertically** by $k$ and
    
- using $g(x)=x−h$ and the composition $f(g(x))$ shifts the graph **horizontally** by $h$


- the ==end behaviour== of a function is how the end of the graph of the function behaves as x approaches infinity (be it positive or negative)

