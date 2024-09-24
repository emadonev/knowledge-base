TAGS: #functions #mathematics #algebra
RELATED: [[Functions]]

### $n$ is positive
In a graph graphing a power function: $y = a*x^n$, $a$ determines if the values are positive or negative and how wide the bottom is, and $n$ determines the shape of the graph. 

If $n$ is **even**, both sides of the graph relative to the y-axis are symetrical.
If $n$ is **odd**, the two sides show different behaviour.

## Zero and negative exponents
If $n$ is 0 in the form $y = ax^n$, then anything to the power of 0 is 1, so $y=a$, or in other words a horizontal line.

If $n$ is less than 0 in the form $y=ax^n$, then we can rewrite this as $y = \frac{a}{x^n}$. The domain is all real numbers except 0 because we cannot divide by zero.

## Fractional exponents
Taking the "root" of something is the same as having a fractional exponent. If we have a function $f(x) = x^n$, the inverse of that is $g(x) = x^{\frac{1}{x^n}}$, and it is also called **taking the n-th root.**
It helps to remember the following rule:
$$y = x^{\frac{m}{n}} = (x^m)^{\frac{1}{n}} = (x^{\frac{1}{n}})^m$$
## Radical Conjugates
An idea where you multiply a square root by another square root in order to turn it into a perfect square, or when using signs you eliminate an irrational number is called a **radical conjugate**. This is especially useful in fractions because we can **rationalize** the denominator which makes calculations easier and simplification possible.

The difference between the square roots of the **smaller** consecutive numbers will be greater than the difference between the square roots of the **larger** consecutive numbers.

> Which of these is larger: $\sqrt{10} - \sqrt{9}$  or $\sqrt{11} - \sqrt{10}$?
> We can use **radical conjugates** or logic to solve this problem. Using algebra, we know that the conjugate of $(a + \sqrt{b})$ is $(a - \sqrt{b})$. 
> $$\sqrt{10} - \sqrt{9} = (\sqrt{10} - \sqrt{9}) * \frac{(\sqrt{10} + \sqrt{9})}{(\sqrt{10} + \sqrt{9})} = \frac{(\sqrt{10})^2 + (\sqrt{9})^2}{(\sqrt{10} + \sqrt{9})} = \frac{10 - 9}{(\sqrt{10} + \sqrt{9})} = \frac{1}{(\sqrt{10} + \sqrt{9})}$$
> We repeat the same process for the other expression. 
> Given that we know (and which is logical) that $\sqrt{11} + \sqrt{10}$ is greater than $\sqrt{10} + \sqrt{9}$, then:
> $$\frac{1}{(\sqrt{10} + \sqrt{9})} > \frac{1}{(\sqrt{11} + \sqrt{10})}$$

## Infinite nests
What is a nested radical expression? It is an expression which contains another radical within it. An **infinitely nested radical** is an expression with an infinite amount of nested radicals. 

If we start from:
$$x = \sqrt{x- \sqrt{x- \sqrt{x- \sqrt{x...}}}} $$
We can see that if we go down a level in the square root we get another expression equal to x because the x roots go down infinitely, so x is 0. 

If we have 
$$x = \sqrt{a\sqrt{a\sqrt{a\sqrt{a\sqrt{a...}}}}}$$
, we can see that 1 layer down, the following is equal to x since both go off into infinity
$$x = \sqrt{a\sqrt{a\sqrt{a\sqrt{a\sqrt{a...}}}}}$$
$$x = \sqrt{ax}$$
$$x^2 = ax$$
$$x(x-a) = 0$$
Since $a$ is nonzero, $x=a$.




