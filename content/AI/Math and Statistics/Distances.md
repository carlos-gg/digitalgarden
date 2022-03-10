---
title: "Distances"
disableToc: false 
---


## Resources
- Anscombe dataset: http://datascienceplus.com/the-importance-of-data-visualization/
- Distance = 1 - Similarity 
- Having a set of points (space), a distance d is a function d(x,y) that takes 2 point in the space and produces a real number. It must satisfy 4 axioms:
	1. d(x,y)>=0, no negative distances
	2. d(x,y)=0 if and only if x=y, positive distances except the from a point to itself
	3. d(x,y) = d(y,x), distance is symmetric 
	4. d(x,y) <= d(x,z)+d(z,y), the triangle inequality says that to travel from x to y, we cannot obtain any benefit if we are forced to travel via some particular third point z. 
- http://www.benfrederickson.com/distance-metrics/ (notebook kind of post using pandas, d3)
- https://github.com/andrecosta90/distance-similarity-measures

### Minkowski
- The Minkowski distance is the generalized Lp -norm of the difference. 
- Lp-norm is the distance d defined as: d = (sum|x_i - y_i|^p)^1/p 

### Euclidean
- Same as L2-norm (Lp-norm when p=2)
- Most familiar distance measure, defined as the square root of the sum of the square distances: d = sqrt(sum((x_i - y_i)^2)
- An equivalent to the L2-norm is the Squared Euclidean distance or sum of squared difference (SSD). This is the fundamental metric in least squares problems and linear algebra. It’s very sensitive to outliers (because of the square). The Mean Squared Error (MSE) is the normalized version of the SSD. 

### Manhattan
- https://en.wikipedia.org/wiki/Taxicab_geometry
- Same as L1-norm (Lp-norm when p=1)
- Also known as Taxicab norm and SAD
- Distance defined as the sum of the absolute differences of the coordinates: d = sum(|x_i - y_i|)
- In solving an underdetermined system of linear equations, the regularisation term for the parameter vector is expressed in terms of the-norm (taxicab geometry) of the vector. This approach appears in the signal recovery framework called compressed sensing.
- The Mean-Absolute Error (MAE) is a normalized version of the SAD: d_MAE(x,y) = d_SAD(x,y)/n = 1/n sum(|x_i - y_i|)

### Cosine
- The cosine distance contains the dot product scaled by the product of the Euclidean distances from the origin. It represents the angular distance of two vectors while ignoring their scale. 

### Jaccard
- The Jaccard distance, is a measure of how _dissimilar_ two sets are. It is the complement of the Jaccard index and can be found by subtracting the Jaccard Index from 100%
- https://en.wikipedia.org/wiki/Jaccard_index

### Hamming
- The hamming distance represents the number of entries in the two sample vectors which are different. It is a fundamental distance measure in information theory but less relevant in non-integer numerical problems. 

### Pearson
- The Pearson distance is a correlation distance based on Pearson's product-momentum correlation coefficient of the two sample vectors. Since the correlation coefficient falls between [-1, 1], the Pearson distance lies in [0, 2] and measures the linear relationship between the two vectors. 
d_pearson(x,y) = 1 - Correlation(x,y)