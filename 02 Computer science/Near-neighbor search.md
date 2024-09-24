TAGS: #programming #computer_science #data #mathematics 

This is a type of search which uses the [[Euclidian metric]], and it tries to find the nearest "neighbor" to our desired datapoint. It can be **monochromatic**, from the same dataset, or **bichromatic**, meaning you compare 2 datasets to each other. 

When having a **monochromatic near neighbor search**, we use the original matrix of data and its [[Transpose]] as the second factor in our vectorized operations. 

The first thought is to loop through the matrix, calculate each distance and then find the smallest one. This is extremely time consuming, and the [[Algorithmic efficiency]] is very low. So we need another approach. 

We can use [[Vectorized operations]] to quickly calculate the nearest neighbor. This works much better, however, it is still not fast enough as the number of data points grows substantially. This is where [[Trees(programming)]] come in. 

Using trees we can divide our matrix into areas where our data is and then focus on the areas closest to our desired area. The algorithm efficiency increases a lot, however the **curse of dimensionality** hinders us from using quad-trees or kd trees. Another solution was to adapt the cutting of our matrix to be more representative. However the curse still follows! Another solution is to use **ball trees**, where different radii are constantly drawn to mimic trees. This converges more quickly than the normal trees, but still with a lot of data, dimensionality is a curse. The final 