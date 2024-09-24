---
tags:
  - motion
  - physics
  - math
  - velocity
---
Movement of objects along a **straight line** is the most elementary form of motion, and also the simplest to describe. We are very familiar with it in the real world, from cars driving on straight highways, bikes, walking, running, etc. Most of our motion involves straight lines. 

The **average velocity** is, as the name suggests, the average [[Velocity]] at which an object or *particle* traveled some distance, $\Delta x$. 
![[average&instant.png|500]]
The straight line connecting points 1 and 2 on the graph is the **slope between those two points**, or the ***average velocity***. $$v_{avg} = \frac{\Delta x}{\Delta t}$$
Now, the *blue line* in the drawing above is the **tangent to a specific point in time, $t$.** The slope at this particular point is ==the instantaneous velocity==. We use [[Calculus]] and [[Derivatives]] for such calculations, or:$$v_x = \lim_{\Delta t - 0} \frac{\Delta x}{\Delta t} = \frac{dx}{dt}$$
> 
> We can track the motion of a particle/object with a *motion diagram*, which is depicted above. 
>

What if **velocity changes though?** We defined velocity as the ==change in position over time==, or the *first derivative of position*, so the change in the change in position is the *second derivative of position* which we call ***acceleration***. Now, since velocity is a [[Vectors]], it has both a magnitude and a direction. So a change in *magnitude* or a change in *direction* both count as acceleration. 

We define average acceleration as:$$a_{av-x} = \frac{\Delta v_x}{\Delta t}$$, for one particular direction (after all, there are 3 axes in the [[Cartesian coordinate system]]). And as with velocity, the average acceleration is the slope between 2 velocity points, and the **instantaneous acceleration** is tangent to a point in time:$$a_x = \lim_{\Delta t - 0} \frac{\Delta v_x}{\Delta t} = \frac{dv_x}{dt} = \frac{d^2x}{dt^2}$$
While we can determine acceleration graphically from a v-t graph, and v from a x-t graph, acceleration from an x-t graph can only be really examined in "is it positive or negative way", since we would have to measure the *curvature of a graph* which isn't very practical. 

However, if we look at **the area underneath a v-t diagram**, we can calculate the ***total distance travelled.*** The same goes from an **a-t diagram**, where we can calculate the ***total velocity change!*** This corresponds to [[Integrals]] in calculus, as well, they are the area under a curve. 

## When the change is constant
---
The simplest (and best :)) kind of motion is one with ==constant acceleration==. We can easily describe **4 fundamental equations** to help us navigate these types of problems. 

#### 01
The first type is super easy, and is the most basic form of velocity and acceleration. From our basic formula on $a$:$$a = \frac{v_2 - v_1}{t_2 - t_1}$$, and assuming that $t_1 = 0$ which is a valid assumption, then:

>$$v_x = v_0 + at$$

#### 02
Now, we'll define an equation where *position is a function of time.* Here, we will be fancy and use a bit of calculus! As mentioned previously, the **area under the curve is an integration.** Hence to get the *total path over time* ($x(t)$), we need to integrate $x$ from the function of velocity. We know the function of velocity, we have already established it above, and hence:$$x(t) = \int_0^t v_x(t)\;dt = \int_0^t(at + v_0)\;dt$$
Remembering how to integrate, we know we can separate this integral into 2 components along with the **constant of integration at the end:**$$x(t) = \int_0^t at\;dt \;+ \int_0^t v_0\;dt$$
Doing the *antiderivative for the first and second integral, we gain:*$$x(t) = \frac{1}{2}at^2 + v_0t + C_2$$The integration constant is logically the **starting position, $x_0$**, and the final equation is:

>$$x(t) = \frac{1}{2}at^2 + v_0t + x_0$$

#### 03
What about a relationship between concepts *without time*? This requires some simple algebra, where we rewrite time as $t = (v_x - v_0)/a_x$ and fill into the formula above. By simplifying this equation we get:
>$$v_x^2 = v_0^2 + 2a(x-x_0)$$

#### 04
The final equation is if we don't have the value of acceleration. It stems from the relationship between ending and starting velocity, as well as average velocity. Since average is beginning plus ending divided by 2, we get:
>$$x-x_0 = \frac{1}{2}(v_x-v_0)t$$

## Times are a' changin'
---
What if the acceleration isn't constant? What do we do then? We use some more calculus! By applying the same principles as last time, we get:$$v_x = v_0 + \int_0^t a\;dt$$ and $$x = x_0 + \int_0^t v\;dt$$
Now, in a problem we will probably know the function for acceleration, and from there it is not difficult to figure out the rest. 


