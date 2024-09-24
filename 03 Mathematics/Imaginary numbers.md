---
tags:
  - math
  - complex_numbers
  - numbers
  - calculation
  - mathematics
  - algebra
---
So, let's say I want to take the root of a negative number. Impossible, right?, Well, maybe not!

# A bit of history
-----
In the 16th century, there was a very talented mathematician who wanted to derive a formula for the cubic equations, same as we have the formula for the quadratic equation. He managed to get a solution, and swore to secrecy all the way to his deathbed where he told his student. Then the student challenged a very talented mathematician Tartaglia to a math duel, and while Tartaglia was originally bluffing, he figured out the solution and beat the student. Later, a very good mathematician Cardan challenged Tartaglia to tell him the formula, and he did. Cardan also stumbled upon the original work of the first mathematician and published his solution in his book. The formula was improved, but there was a slight hitch. For certain values, there appears to be no solution!

In some cases the solution tries to include the **roots of negative numbers**, which is naturally impossible. How do we proceed from here?
- n NOTE: In cubic equations, by their definition or well how they are structured on a graph, every cubic equation has at least 1 solution, which means that there must be a solution to the root of a negative number, but we just don't see it!

## The $\sqrt{-1}$ 
-----
The solution to Cardan's problem was provided by Bombelli, who said that we should include the square root of negative 1 in our number system, which would allow us to rewrite the expression and get a "real" result without the $\sqrt{-1}$. By extending our definition of numbers, he was able to solve the problem and eliminate the square roots of negative numbers to get a real solution. However, he then proclaimed this to be ludicrous and a way to deceive. But is it really?

## The complex plane
------
So, how do we visualise the complex number? What is a complex number?
- eg A complex number is a number which contains the real and the imaginary components of a number. In reality, every number is a complex number, written in the following form: $$z = a + bi$$, where $a$ is the real component and $b$ is the imaginary component. If we want to represent real numbers, whole numbers, natural numbers, whatever, all we need to say is that $b=0$. 

Okay, but how can we visualise this? By using the complex plane! This plane introduces the vertical axis of the number line, bringing the imaginary number line and the real number line together. Now, let's say we multiply i around the complex plane. We see that multiplying by i rotates the number by 90º. This is cool! This means that there must be some connection between the real and imaginary parts of the plane. 
![[complex rotation.png|400]]

Now, let's look at the connections between numbers.
### Connecting the axes
------
So, we can accomplish this by multiplying 2 complex numbers. After we plot them on the complex plane, let's take a look at their angles.
![[complex angles.png|400]]
Using [[Fundamental trigonometry]] we can calculate the angles of every component of the multiplication and the result. ![[angles plane.png|400]]
Now, what can we notice?
That if we add the angles corresponding to the components of the multiplication we get the angle of the sum!
![[adding rule complex.png|400]]
This is awesome! What about the length?
![[distance complex.png|400]]
We can use the pythagorean theorem! After we calculate c of each number, what do we notice?
![[distance rule complex.png|400]]
We notice that if we multiply the distances of the factors we get the distance of the result! This is a superb connection between the complex numbers and the complex plane! We don't need to use standard algebra to calculate everything for complex numbers, since we can use the complex plane to draw everything geometrically. We have created a whole coordinate system exactly for this purpose: [[Polar coordinate system]]! We denote complex numbers as:$$z = 1<156º$$, where $1$ is the distance and $156º$ is the angle.

### Using the complex plane for problem solving
------
We can use the complex plane for easier solving of problems by using the [[Unit circle]] and [[Fundamental trigonometry]] and a bit of knowledge about [[Functions]] and [[Polynomials]]. If we wanted to know all the solutions to a polynomial, all we need is the unit circle and the division of the complex plane to search for answers. 

-----

Now that we know all about imaginary numbers and complex numbers, what about [[Complex functions]]?

