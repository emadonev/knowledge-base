---
tags:
  - coordinate_systems
  - mathematics
  - astronomy
  - calculation
  - trigonometry
---
Our standard coordinates are represented in the [[Cartesian coordinate system]], with $x,y,z$ coordinates for the 3 dimensions. However, since everything in astronomy and [[The celestial sphere]] is spherical, we use the [[Polar coordinate system]]. A 3D polar coordinate system also has  variables:
1. $r$ - the distance from the origin to the point of interest (P)
2. $\psi$ - the angle between the x axis and the projection of r on the xy plane - basically the "bottom" coordinate 
3. $\theta$ - the angle between r and the z axis - basically the "vertical" coordinate

We can easily convert each of the standard $x,y,z$ coords into the new and improved $r, \psi, \theta$ coordinates.

![[cart to polar.jpeg|400]]

Now, in order to convert from one coordinate system to another system, we need to rotate a cartesian system by some axis, which is usually the *y axis*, since for different systems we use different bases (horizon, equator, ecliptic,...). 
![[rot of cart 1.jpeg|400]]

![[rot of cart 2.jpeg|600]]

And just like that, we have derived a series of equations to convert all our cartesian coordinates into rotated polar coordinates! Without the use of [[Spherical trigonometry]]! Of course, this whole process could have been done with spherical triangles, but this is (for me at least) a much more intuitive and easier way to grasp coordinate conversion. Now, let's apply this general form to specific transformations from one coordinate system to another.

# Horizontal to HA-dec
---
![[horizon-HA.jpeg|400]]
Or, if we are using spherical trigonometry:

![[spherical triangle hor to equ.png]]

If we look at it, we can say that the conversion from the horizontal system to the HA-dec system ([[The celestial sphere]]), is the same as first defining a cartesian horizontal system, then converting it to a polar system, and rotating it by an angle, in order to get the spherical HA-dec system. 

Using the angle notions from the previous part, $\psi$ is the notion of the "bottom" angle or the angle along the bottom plane, which are *A* in the original system, and *H* in the rotated one. Also, since they are defined anticlockwise, and here they are measured clockwise then:$$\psi = -A, \psi' = -H$$
Next, the angle $\theta$ is the vertical change from the line r to the z axis, hence for our case this means:$$\theta = 90º-h, \; \theta' = 90º - \delta$$
And finally, by how much did we rotate? Well, the angle SOH is (O is the middle point of the sphere), is coangular with NOP, so:$$\chi = 90º-\phi$$
Using the equations we defined earlier, we get:
$$\begin{align} cos(-H)sin(90º-\delta) = cos(-A)sin(90º-h)cos(90º-\phi) + cos(90º-h)sin(90º-\phi) \\
sin(-H)sin(90º-\delta) = sin(-A)sin(90º-h) \\
cos(90º-\delta) = cos(90º-h)cos(90º-\phi) - cos(-A)sin(90º-h)sin(90º-\phi)
\end{align}$$

Using some simplification and reduction of [[Fundamental trigonometry]]:
- !! $$sin(-a) = -sin(a), sin(180º-a) = sin(a)$$ $$cos(-a) = cos(a), cos(180º-a) = -cos(a)$$ $$sin(90º +- a) = cos(a), \;cos(90º+-a) = +- sin(a)$$

we get:
$$\begin{align} cos(H)cos(\delta) = cos(A)(-cos(h))(-sin(\phi)) + (-sin(h))(-cos(\phi)) \\
-sin(H)cos(\delta) = -sin(A)cos(h) \\
sin(\delta) = (-cos(h))(-cos(\phi)) - cos(A)cos(h)cos(\phi)
\end{align}$$
With the final result being:
- eg $$\begin{align} cos\;H\;cos\;\delta = cos\;A\;cos\;h\;sin\;\phi + sin\;h\;cos\;\phi \\ sin\;H\;cos\;\delta = sin\;A\;cos\;h \\ sin\;\delta = cos\;h\;cos\;\phi - cos\;A\;cos\;h\;cos\;\phi \end{align}$$

We apply this process in the opposite direction as well if we want to convert from HA to horizontal.

- !! Important note!!!! We need to make sure that we are aware that $H$ and $A$ are **not confined to the first quadrant** in trigonometry, so we need to know both their **sine and cosine to determine the angle.**

# Ecliptic system to RA-dec
---
![[ecliptic to RA.jpeg|400]]
We apply the same mechanism as before, where the ecliptic system is now the base and the RA-dec system is the rotated version. Looking at the horizontal angles, we can see that:$$\psi = \alpha - 90º, \;\psi'=\lambda - 90º$$, as for the vertical angles:$$\theta = 90º-\delta,\;\theta' = 90º-\beta$$, and finally the angle of inclination is:$$\chi = \epsilon$$, or the obliquity of the orbit. Performing the same algebraic and trigonometric functions/tricks we obtain the following equations

- eg $$\begin{align} cos\;\lambda\;cos\;\beta = sin\;\delta\;sin\;\epsilon + cos\;\delta\;cos\;\epsilon\;sin\;\alpha \\ sin\;\lambda\;cos\;\beta = cos\;\delta\;cos\;\alpha \\ sin\;\beta = sin\;\delta\;cos\;\epsilon - cos\;\delta\;sin\;\epsilon\;sin\;\alpha \end{align}$$

When wanting to convert from RA-dec to ecliptic we get the following:
$$\begin{align} sin\;\alpha\;cos\;\delta = -sin\;\beta\;sin\;\epsilon + cos\;\beta\;cos\;\epsilon\;sin\;\lambda \\ cos\;\alpha\;cos\;\delta = cos\;\lambda\;cos\;\beta \\ sin\;\delta = sin\;\beta\;cos\;\epsilon - cos\;\beta\;sin\;\epsilon\;sin\;\lambda \end{align}$$

# Galactic to equatorial coords
---
Finally, we can convert galactic coordinates into equatorial ones by following the exact same steps beforehand:
- f $$\sin(l_N - l)\cos b = \cos \delta \sin (\alpha - \alpha_p)$$$$\cos(l_N - l)\cos b = -\cos \delta \sin \delta_p \cos(\alpha - \alpha_p) + \sin \delta \sin \delta_p$$$$\sin b = \cos \delta \cos \delta_p \cos(\alpha - \alpha_p) + \sin \delta \sin \delta_p$$

Where $\alpha_p = 12h 51.4min$, $\delta_p = 27º08'$ and $l_N = 123.0º$

