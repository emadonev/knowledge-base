TAGS: #research_paper #astronomy #variable_star #light 

Link: file:///Users/emadonev/Downloads/journal.pone.0259735.pdf

- **Visibility graph:** plots a timeseries into a graph
	- every node is a datapoint in time, and 2 nodes are connected if they can be joined by a *visibility line.*
	- this algorithm is used to find the shortest path from one place to anther without bumping into obstacles or other data points.
	- **Normal VG:** the visibility line joins data points, allows different slopes and relative heights.
	- **Horizontal VG (HVG):** data points are replaced by vertical bars, ad the visibility line is drawn parallel to the x-axis. 
- **Graph theory stuffs**
	- *Average degree (k):* the degree of a node is how many edges are connected to it. So the average sums up all of the degrees and divides by the number of nodes.
	- *Clustering coefficient (C):* this says how densely connected the nodes of the graph are. This is the average individual clustering of all nodes.
		- *Individual clustering coefficient ($c_i$):* the ration of the number of actual connections between the neighbours to the maximum number of connections. 
	- *Transitivity coefficient:* this is another measure of density. It is the ratio of the total amount of triangles in the graph to the total number of connected triples of nodes. 