---
title: "Clustering"
---

> Cluster analysis or clustering is the task of grouping a set of objects in such a way that objects in the same group (called a cluster) are more similar (in some sense or another) to each other than to those in other groups (clusters)

## Resources
- http://scikit-learn.org/stable/modules/clustering.html
- Embeddings. [TF projector](http://projector.tensorflow.org)

### Hierarchical clustering
- Method of cluster analysis which seeks to build a hierarchy of clusters
- Strategies for hierarchical clustering generally fall into two types:
	- Agglomerative: This is a "bottom up" approach: each observation starts in its own cluster, and pairs of clusters are merged as one moves up the hierarchy.
	- Divisive: This is a "top down" approach: all observations start in one cluster, and splits are performed recursively as one moves down the hierarchy.
- The results of hierarchical clustering are usually presented in a dendrogram. The complexity of agglomerative clustering is O(n^2log(n)), slow for large data. Divisive clustering with an exhaustive search is O(2^n), which is even worse.
- https://blog.alookanalytics.com/2017/04/11/intuition-vs-unsupervised-learning-agglomerative-clustering-in-practice/
- Single linkage: Single-linkage clustering is one of several methods of hierarchical clustering. It is based on grouping clusters in bottom-up fashion (agglomerative clustering), at each step combining two clusters that contain the closest pair of elements not yet belonging to the same cluster as each other. A drawback of this method is that it tends to produce long thin clusters in which nearby elements of the same cluster have small distances, but elements at opposite ends of a cluster may be much farther from each other than to elements of other clusters. The naive version has a time complexity of O(n^3). There are improvements: SLINK and Kruskal's algo, with time complexity O(n^2).
- Mean linkage
	- [Unweighted Pair Group Method with Arithmetic Mean](https://en.wikipedia.org/wiki/UPGMA)
	- [Weighted Pair Group Method with Arithmetic Mean](https://en.wikipedia.org/wiki/WPGMA)
- Ward’s method: Ward's minimum variance criterion minimizes the total within-cluster variance.
  To implement this method, at each step find the pair of clusters that leads to minimum increase in total within-cluster variance after merging. This increase is a weighted squared distance between cluster centers. At the initial step, all clusters are singletons (clusters containing a single point).
- Complete linkage: The method is also known as farthest neighbour clustering. At the beginning of the process, each element is in a cluster of its own. The clusters are then sequentially combined into larger clusters until all elements end up being in the same cluster. At each step, the two clusters separated by the shortest distance are combined. 
  The definition of 'shortest distance' is what differentiates between the different agglomerative clustering methods. 
  In complete-linkage clustering, the link between two clusters contains all element pairs, and the distance between clusters equals the distance between those two elements (one in each cluster) that are farthest away from each other. Complexity O(n^3), CLINK version with O(n^2).

###  K-means
- https://en.wikipedia.org/wiki/K-means_clustering
- k-means clustering aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean, serving as a prototype of the cluster. The standard k-means algorithm is called Lloyd's algorithm:
	- Initialization: Forgy method (taking k random observations from the data set), random partitioning or k-means++ methods 
	- 2 steps: assignment and update (the "assignment" step is also referred to as expectation step, the "update step" as maximization step, making this algorithm a variant of the generalized expectation-maximization algorithm):
		- Assignment: Assign each observation to the cluster whose mean yields the least within-cluster sum of squares (WCSS). Also called “Expectation step” because it involves updating our expectation of which cluster each point belongs to
		- Update step: Calculate the new means to be the centroids of the observations in the new clusters. This also minimizes the within-cluster sum of squares (WCSS) objective. Also called “Maximization step” because it involves maximizing some fitness function that defines the location of the cluster centers — in this case, that maximization is accomplished by taking a simple mean of the data in each cluster
  - http://stanford.edu/~cpiech/cs221/handouts/kmeans.html  
  - Estimating the number of clusters:
	  - [Are You Still Using the Elbow Method?](https://towardsdatascience.com/are-you-still-using-the-elbow-method-5d271b3063bd)
	  - Elbow method: the best value for k is the point of maximum curvature of the inertia curve, where inertia is the sum of squared distances between each point and the center of the cluster it belongs to (inertia gets smaller as _k_ increases). The elbow is the point where a lower value of inertia is not worth the additional complexity (i.e. more clusters)
	  - Alternative scores, not based on the inertia concept: Calinski-Harabasz, Davies-Bouldin, Silhouette, BIC (Bayesian Information Criterion)
	  - A systematic comparison shows that Calinski-Harabasz and BIC are the best performing methods. The elbow method seems to be the worse choice overall

### DBSCAN 
- [Density-based spatial clustering of applications with noise](https://en.wikipedia.org/wiki/DBSCAN)
- [HDBSCAN](http://hdbscan.readthedocs.io/en/latest/soft_clustering_explanation.html)

### Spatial clustering
- [Introduction to hierarchical clustering (Spatial clustering)](https://towardsdatascience.com/introduction-to-hierarchical-clustering-part-3-spatial-clustering-1f8cbd451173)

## References
- #PAPER [k-means++: the advantages of careful seeding (Arthur 2007)](https://dl.acm.org/doi/10.5555/1283383.1283494)
- #PAPER [A Comparative Study of Efficient Initialization Methods for the K-Means Clustering Algorithm (Celebi 2012)](https://arxiv.org/abs/1209.1960)
- #PAPER [SCAN: Learning to Classify Images without Labels (Van Gansbeke 2020)](https://arxiv.org/abs/2005.12320)
	- #CODE https://github.com/wvangansbeke/Unsupervised-Classification
	- [Paper explained](https://www.youtube.com/watch?v=hQEnzdLkPj4)
	- grouping images into semantically meaningful clusters when ground-truth annotations. This is tackling the task of unsupervised image classification in [Computer vision](AI/Computer%20Vision/Computer%20vision.md)
	- advocate a two-step approach where feature learning and clustering are decoupled. First, a self-supervised task from representation learning is employed to obtain semantically meaningful features.Second, we use the obtained features as a prior in a learnable clustering  approach.  In  doing  so,  we  remove  the  ability  for  cluster  learning to depend on low-level features, which is present in current end-to-end learning approaches
- #PAPER [Deep Robust Clustering by Contrastive Learning (Zhong 2020)](https://arxiv.org/abs/2008.03030)
- #PAPER [DeepDPM: Deep Clustering With an Unknown Number of Clusters (Ronen 2022)](https://arxiv.org/pdf/2203.14309)
	- #CODE https://github.com/BGU-CS-VIL/DeepDPM
	- https://medium.com/syncedreview/meet-deepdpm-no-predefined-number-of-clusters-needed-for-deep-clustering-tasks-e7c635039013