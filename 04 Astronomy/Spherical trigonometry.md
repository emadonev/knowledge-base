---
tags:
  - trigonometry
  - triangle
  - celestial_sphere
  - astronomy
  - math
  - calculation
  - coordinate_systems
---
So, spherical geometry, or well ==trigonometry==([[Fundamental trigonometry]]), is the geometry of a sphere! To make astronomical coordinates easier to handle, we have defined the **celestial sphere**, a sphere of "infinite" distance away from the Earth (since the distance in this case is irrelevant). 

There are 2 types of circles inside a sphere: **great circles** and **small circles**. ==Great circles== are circles who include the centre of the sphere, in other words, their radius is the main radius of the sphere, which is constant and fixed. Small circles are basically any other circle which isn't $r$ distance from the centre. Every sphere has **poles**, which are 2 points perpendicular to the horizontal plane of the sphere. Here is an example of a sphere with circles:
![[spheretrig1.png]]
Something you may have noticed, is that we have things called **spherical angles**. While they might be hard to define at first, their definition is quite elementary:
- eg **Spherical angle**: the angle on a spherical surface created by 2 tangent lines along the arcs of the sphere.

Finally, our third object required to understand spheres are called **spherical triangles.** 
- eg **Spherical triangles** are triangles whose sides or *arcs* are defined by the intersection of *3 great circles*. 

So, from the image above, triangle $PBC$ is a spherical triangle, while $PFG$ isn't. However, there are a couple of other things to know about spherical triangles:
- !! 1. Any 2 sides are together greater than the 3rd side
- !! 2. The sum of the angles is **greater than 180º**, and we define the **excess** as:$$E = A + B + C - 180º$$
- !! 3. Each spherical angle is less than 180º

Here is a more detailed image of a spherical triangle:
![[sphereitrg2.png]]
From this we can see that each side (represented by the small letters *a, b and c*), can be expressed as follows:
$$a = R * \theta$$, with $\theta$ being the angle between COB, where O is the centre of the sphere. Since $R$ is constant, we can **define the arc lengths of the triangle as angles themselves, ==expressed in [[Radians]]==**. 

But, what if we wanted to calculate the length of the arc of the parallel small triangle right above the spherical triangle in the first image? We can see that the central angles, FKG and BOC are equal, and since we know that:
$$FG = r*FKG, BC = R*BOC$$
$$FG = BC * \frac{r}{R}$$
And now, if we look at the plane triangle KOF, it is right angled, which. means that trigonometric rules apply. So, $\frac{r}{R}$ is actually equal to: $$FG = BC* sin KOF$$

#### Area of spherical triangle
---
How would we calculate the area of a spherical triangle? Well, the formula is:
- f $$A = Er^2$$

But, why? Let's prove this!
If we extend the great circles of a sphere, we actually get 2 spherical triangles which are **congruent**. We then see that the area S(A) is actually $A/180º$ of the area of the sphere, which is $4\pi r^2$. Similarly, S(B) and S(C) are $B/180º$ and $C/180º$ part of the area. The slices all cover the area of the spherical triangle. The area of all of these slices is equl to the area of the sphere + 4 areas of the triangle, resulting in the formula above.
# Spherical triangles
---
An important note:
>SIDES: a, b, c
>ANGLES: A, B, C

### The cosine formula
![[sphertrig3.png]]
Consider the image above. We can see that DAE, DAO, DEO and AEO are plane triangles, but not in the same planes. Using the **cosine rule** from elementary trig, we can say that: $$DE^2 = AD^2 + AE^2 - 2AD.AE\;cos\;A$$
and for DEO:$$DE^2 = OD^2 + OE^2 - 2OD.OE\;cos\;a$$
If we equate these 2 equations, we get:
$$\begin{align}
DE^2 = DE^2 \\
AD^2 + AE^2 - 2AD.AE\;cos\;A = OD^2 + OE^2 - 2OD.OE\;cos\;a \\
2OD.OE\;cos\;a = (OD^2 - AD^2) + (OE^2 - AE^2) + 2AD.AE\;cos\;A \\
\end{align}
$$
Now, let's consider the 2 other planar triangles which are right-angled and share a side:
$$OD^2 - AD^2 = AO^2, OE^2 - AE^2 = AO^2$$, and we can then continue this equation:
$$\begin{align}
2OD.OE\;cos\;a = 2AO^2 + 2AD.AE\;cos\;A \\
OD.OE\;cos\;a = AO^2 + AD.AE\;cos\;A \\
\end{align}
$$
And now, we want to divide the entire equation by $OD.OE$. Now we get the following:
$$cos\;a = \frac{OA}{OD}\frac{OA}{OE} + \frac{AD}{OD}\frac{AE}{OE}\;cos\;A$$
Let's take a look at the planar triangles DAO and AEO:
![[sphertrig4.png]]
From the following we can conclude:
- $\frac{OA}{OD} = cos\;b$
- $\frac{OA}{OE} = cos\;c$
- $\frac{AD}{OD} = sin\;b$
- $\frac{AE}{OE} = sin\;c$

- eg And the final formula is: $$cos\;a = cos\;b\;cos\;c + sin\;b\;sin\;c\;cos\;A$$

### The sine formula
Let's take the previous formula and write it as so:$$ sin\;b\;sin\;c\;cos\;A= cos\;a  -cos\;b\;cos\;c$$
Now let's square this equation:$$ sin^2\;b\;sin^2\;c\;cos^2\;A= cos^2\;a  - 2cos\;a\;cos\;b\;cos\;c + cos^2\;b\;cos^2\;c$$
Taking a closer look, we see we can rewrite the left-hand side as such:$$\begin{align}
sin^2\;b\;sin^2\;c(1-sin^2A) = 
sin^2\;b\;sin^2\;c - sin^2\;b\;sin^2\;c\;sin^2A = \\ 
(1-cos^2\;b)(1-cos^2\;c) - sin^2\;b\;sin^2\;c\;sin^2A \\
back \; to \; original \; equation \\
cos^2\;a  - 2cos\;a\;cos\;b\;cos\;c + cos^2\;b\;cos^2\;c = 1-cos^2b - cos^2c + cos^2bcos^2c - sin^2\;b\;sin^2\;c\;sin^2A \\
sin^2\;b\;sin^2\;c\;sin^2A = 1-cos^2a-cos^2b-cos^2c + 2cos\;a\;cos\;b\;cos\;c \\
\end{align}$$
What we can realise from this final equation, is that this is a **symmetrical function of a, b and c**, since with whichever equation for the cosine formula we started with, ==we would get the same result==. Hence, we can say the following:
$$sin^2a\;sin^2b\;sin^2C = sin^2b\;sin^2c\;sin^2A = sin^2c\;sin^2a\;sin^2B$$, and by dividing, we get the following:
- eg The final formula:$$\frac{sin\;A}{sin\;a} = \frac{sin\;B}{sin\;b} = \frac{sin\;C}{sin\;c}$$

### The analogue to the cosine formula
We start the same as before: $$sin \;b \;sin \;c \;cos \;A = cos \;a − cos \;b \;cos \;c$$
And, instead of $cos\;c$,. we substitute with the cosine formula, obtaining:$$sin \;b \;sin \;c \;cos \;A = cos \;a − cos \;b(cos \;a \;cos\; b + sin \;a \;sin \;b \;cos \;C)$$$$sin \;b \;sin\; c \;cos\; A = cos \;a\; sin^2 b − sin \;a \;sin\; b \;cos\; b\; cos\; C$$
Now, we divide everything by $sin\;b$, and we get:
- eg The final formula:$$sin \;c \;cos\; A = cos\; a \;sin \;b − sin \;a \;cos\; b \;cos C$$

### The four parts formula
This is the final formula that is necessary for spherical trigonometry. Its proof is also quite simple:
Let's start from the cosine formulas for both $c$ and $b$:
$$cos \;b = cos \;c \;cos\; a + sin \;c \;sin \;a \;cos \;B$$$$cos \;c = cos\; a\; cos \;b + sin \;a \;sin\; b\; cos\; C$$
And now, we replace $cos\;c$ in the first equation with the entire equation below. 
$$cos \;b(1 − cos^2 a) = cos \;a\; sin \;a \;sin\; b \;cos \;C + sin\; c\; sin\; a \;cos \;B$$
And dividing everything by $sin\;a\;sin\;b$, we get:$$cot \;b \;sin \;a = cos \;a \;cos\; C + \frac{sin\;c}{sin\;b}cos \;B$$
And via the **sine formula**, we get that this ratio is the same ratio as it would be for the angles, so $\frac{sin\;C}{sin\;B}$, and so:
- eg The final formula:$$cos\;a\;cos\;C =sin\;a\;cot\;b−sin\;C\;cot\;B$$

---
