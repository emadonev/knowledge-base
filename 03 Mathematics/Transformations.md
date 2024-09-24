---
tags:
  - algebra
  - mathematics
  - geometry
  - coordinate_systems
---
Transformations are based in the [[Cartesian coordinate system]], and there are 3 elementary transformations which can produce any "movement" in [[Geometry]] based on their sequence of application (not a commutative operation), as we can treat a transformations as [[Functions]].

- !! It is very important to note that these transformations have to be **rigid**. This means that we don't *distort or change the distances between the points*, which would make all shapes mutable and geometry useless. Hence, the [[Distance formula]] must yield the **same distance between points no matter the transformation**, keeping the original shape of a triangle, let's say.

## Translation
---
**Translation** is simply the act of moving an object from one place to another, we change the x coordinate by a certain amount and the y coordinate by a certain amount.
$$T(x,y) = (x+a, y+b)$$
![[translation.png]]
## Rotation
---
**Rotation** is the act of rotating an object from an origin point by a certain angle, $\theta$. Its transformation is a tad more complicated, as it involves [[Fundamental trigonometry]]. 
$$R(x,y) = (x\;cos\theta - y\;sin\theta, x\;sin\theta+y\;cos\theta)$$
![[rotation.jpeg]]
## Reflection
---
**Reflection** is the act of, well, reflecting an object's coordinates based on some line, $l$. This line can also be an axis of the coordinate system, but it can also be any possible linear line. For reflections with the x and y axes, we refer to changing the sign of either the x or y coordinates. 
![[reflection.jpeg]]

We can define the transformations being done on a certain object as **composition of functions**, since we need to apply them in a specific order and they take ==coordinates as an input, manipulate them, and give 2 coordinates back as an output==. 
$$U(X) = T(R(X))$$
For example, we can first rotate and then translate an object, which is a composition of the functions for rotation and translation, respectively. 
