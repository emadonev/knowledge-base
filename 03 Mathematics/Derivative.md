---
tags:
  - calculus
  - math
  - calculation
  - mathematics
  - numbers
---
*A* derivative is an element of ==differentiation== which is all about how 2 variables are related by a [[Functions]]. When 2 elements are related by some function in an *implicit way*, we can rewrite it so we can see the relationship specifically for $x$ and $y$ or a different set of variables. This is called *explicit* notation.

What if we wanted to see the ratio between a small part of $x$ that we change and see what happens to $y$? This change is called ==differentiation or taking a derivative==! 

------
Let's say that we want to look into a super simple example. $$y = x^2$$ We can see that since y is equal to x, if x increases, so does y. But by how much? This is where we introduce the ratio: $$\frac{dy}{dx}$$ $\ce{->}$ how much does $y$ change with respect to $x$.

So, then what if we enlarge $x$ by some tiny value $dx$? Well then, $y$ would increase by a proportional $dy$ as well. Let's square it out.
$$y + dy = (x + dx)^2$$ $$y + dy = x^2 + 2x *dx + (dx)^2$$ Now, we know that from [[Calculus]], that $dx$ is an extremely small quantity. So, we can forget it. We also know that $y=x^2$, so we can cancel that out. We are left with:
$$dy = 2x * dx $$, or $$\frac{dy}{dx} = 2x$$ And that's it! If we repeat this same process for $y=x^3$, we would get: $$\frac{dy}{dx} = 3x^2$$. We are starting to notice a pattern here. We can make the following statement:
- eg *Let $y=x^n$. Then, we should expect the derivative to be: $$\frac{dy}{dx} = nx^{(n-1)}$$*

But what if we have constants? Well, it turns out that if we add constants to our equation or subtract a constant from our equation, nothing happens. The derivative ==isn't dependent on the added/subtracted constant==. 

However, if we multiply a constant:
$$y = 4x^3$$, then:
$$\frac{dy}{dx} = 12x^2$$

- eg Let $y = ax^n$. Then, we should expect the derivative to be: $$\frac{dy}{dx} = a * nx^{n-1}$$
## Taking the derivative with products, sums and quotients
----
For sums, the rule is very simple.
$$\frac{dy}{dx} = \frac{du}{dx} + \frac{dv}{dx}$$, where the original equation is $y = u + v$. 

However, for products and quotients it gets a bit tricky. $$y + dy = (v+dv)×(u+du)$$
$$y +dy= v×u + v×du + u×dv + dv×du$$
$dv×du$ is too small of a quantity, so we ignore it.
$$dy = v×du + u×dv$$, and when we divide everything by $dx$, we get:
$$\frac{dy}{dx} = v\frac{du}{dx} + u\frac{dv}{dx}$$And there! Even though it seemed difficult at the start, the main point is to ==generalize every situation and then calculate a general rule which can be applied to any example==.

And finally, for quotients:
- eg *For $y + dy = \frac{u + du}{v + dv}$, the general formula is:* $$\frac{dy}{dx} = \frac{v\frac{du}{dx} + u\frac{dv}{dx}}{v^2}$$

# Successive derivation
---
If we want to take successive derivation, eventually we won't have anything to differentiate! We go by the same rules as previously stated:
- eg For every differentiation degree $m$, where $y = f'(x) =x^n$:$$mth \; = f(x) = n(n-1)(n-2)...(n-m-1)x^n-m$$
> Successive derivation is basically taking the derivative of a derivative. An intuitive example is [[Position]], [[Velocity]] and [[Acceleration]]. We express tiny changes in position with velocity and time, and we express tiny changes in velocity with acceleration and time. Each component builds upon each other, with position being a [[Quadratic formula]] of velocity, and velocity being a [[Linear function equation]] of acceleration - the linear function is the derivative of the quadratic formula by the ==power rule==. 


