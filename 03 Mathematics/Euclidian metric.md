TAGS: #mathematics #data_analysis #metric #algebra 

This metric uses the Pythagorean theorem to find the nearest distance from one point to another point by constructing right triangles. 

$$
D(x, x_i) = \sqrt{\sum^D (x_d-x_{i,d})^2}
$$
We can rewrite this expression in vectorized form, in order to compute faster.
Our matrices look like this:
![[nns_1.jpg]]

Breaking this expression down (without the square root, since we are just comparing), we get the following:
$$
\sum (x-x_i)^2 = \sum x^2 - 2\sum x*x_i + \sum x_i^2
$$

We can use our matrices to calculate this using vector notation. The figure below illustrates the process.
![[nns_2.jpg]]

And so the final operation is:
$$
[XX^T]_{ii} + [XX^T] - 2[XX^T]_i
$$
