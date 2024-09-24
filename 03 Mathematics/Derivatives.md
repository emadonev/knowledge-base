---
tags:
  - calculus
  - mathematics
  - physics
---
**Derivatives** are a crucial part of [[Calculus]], aiming to look for the *change in a moment*, an infitesimaly small fraction of time, actually no time at all. 
- !! They look at a *particular moment* and look for the **change in a particular property**, for example the change in position over time or the change in happiness over time, etc. 

A *positive derivative* means that our desired quantity is increasing, while a *negative derivative* that it is decreasing. When the derivative is 0, we have reached a local *maximum or minimum*. Naturally*, we can take the **derivative of a derivative**, to monitor the change of a change.
- eg For example, looking at the change in position over time gives us [[Velocity]], while the **change in velocity or the second derivative of position** is actually [[Acceleration]]. Now, taking many derivatives of derivatives can get carried away. ![[derivatives out of control.jpeg]]

However, when looking at an *instantaneous* change, or looking at a particular moment, w<mark style="background: #faedcd;">e realize that the change in our quantities is 0</mark>, since we are only looking at a moment. A very clever guy by the name Leibniz figured out a sleight of hand to help mathematicians with this conundrum. He developed the *dx* notation, where they don't really represent numbers or specific values, they cannot really be divided, however, they represent a **infinitesimal increment of a quantity**, which is visually self-explanatory and cannot *really* be described. 

But, how can we describe the rate of change? How would we begin describing it? Let's say we look at some curves. Like a parabola, defined with the [[Quadratic equation]]. The more we zoom into its graph, the more **linear** it becomes, and it is almost like its curviness disappears! If we look at a snapshot, a moment, it is straight for all intents and purposes!
![[curves2.png]]
![[curves1.png]]

So, if curves approach straight lines, we can say that the **slope of a point is a ==tangent line==**, which comes extremely handy in calculus.
![[tangents and calculus.png]]
Now, another thing we need to take care of are [[Limits]]. They define how far we can really look into the infinite, so we don't step over the boundary of a limit, off into infinity... 

### What if we can't take a derivative?
---
But, what happens if we don't have smooth [[Functions]]? Can we still take a derivative? Well, not really. With a smooth function, there is a **transition from one direction to another**, a point where ==the derivative is 0.== However, for nondifferential functions, there is a **sharp turn** (like in absolute functions), where we cannot take the derivative since *nothing can be defined in that moment*.
![[no derivatives.png]]
But, this is just a function with only one undefined point. A very "poetic" mathematician
- n *""It is true, that a mathematician who is not somewhat of a poet, will never be a perfect mathematician.*

created a monster of a function, one whose every single point doesn't have a derivative. It approximately looks like this:
![[weierstrass.png]]
This is the point in history where<mark style="background: #e9edc9;"> geometric intuition became less reliable in calculus, but rather analytic rigor took over. </mark>

## How do we even derive?
---
Let's start with a square with sides x.
- eg If we change the length x by *just a little bit*, how would $x^2$ change?

![[power rule.png]]
We can say that: $$(x + dx)^2 = x^2 + 2xdx + dx^2$$ But, how large is dx really?
![[dx size.png]]
So, we can actually ignore $dx^2$. Now, looking at the rate of change, we can really see that $x^2$ changed by only ==2x==. 

What about $x^3$? We can look at a very similar example:
![[x3.png]]
And looking at the sides of this cube, we can ignore the sides with $dx^2$ and the tiny square of $dx^3$. So, we are left with:
![[derivative of x3.png]]
So the derivative of $x^3$ is $3x^2$. Is there a slight pattern here? ([[Power rule]]) 

Derivatives of lower powers are super easy to visualize, and this is where [[Geometry]] comes in handy for understanding. However, for more complicated analysis, we turn to **algebra!** 

## A slightly more formal definition
---
The general definition of a derivative is:$$f'(a) = lim_{b\ce{->}a} \frac{f(b)-f(a)}{b-a}$$
Which is really like saying that we are calculating the slope of a tangent line along the curve of the graph of the function $f$. 

These are the rules when handling derivatives, and they are:
- [[Constant rule]]
- [[Sum rule]]
- [[Product rule]]
- [[Power rule]]
- [[Chain rule]]
- [[Quotient rule]]




### A slightly more geometrical look of graphs
---
By plotting [[Functions]] onto the [[Cartesian coordinate system]], we gain a sort of image of a graph. We can then picture the derivative of a constant shifting tangent line along a curve.
- !! When the derivative is equal to 0, we have reached a *minimum* or *maximum* point in the function - **critical point for a smooth function f** 

We differentiate 2 kinds of minima and maxima:
1. LOCAL - they are confined to a local area of a graph, largest or smallest value compared to neighbouring points
2. GLOBAL or ABSOLUTE - as the name suggests, the largest extreme value in the graph.

> How do we differentiate from minima or maxima?

By using the *second derivative!* We can track how the derivative changes, and if it<mark style="background: #f2cd60;"> is decreasing </mark>after the critical point it <mark style="background: #f2cd60;">must be a maximum</mark>, and if it is <mark style="background: #f2cd60;">increasing it has to be a minimum</mark>.

- !! However, if the derivative of the derivative is 0, *we cannot tell if it is a maxima or minima*, and this is often called the **saddle point**. 

- n We cannot (unfortunately) tell using derivatives if one extreme is local or global, as for that we would have to look at  the entire domain of a function, and these domains are usually infinite. 
