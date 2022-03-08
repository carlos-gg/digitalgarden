---
title: "Dimensionality reduction and low-rank modeling"
disableToc: false 
---

## Resources
- The Beginner's Guide to Dimensionality Reduction: https://idyll.pub/post/visxai-dimensionality-reduction-1dbad0a67a092b007c526a45/
- Distances, Neighborhoods, or Dimensions? Projection Literacy for the Analysis of Multivariate Data: https://visxprojections.dbvis.de/client/index.html
- Decomposing signals in components (matrix factorization problems): https://scikit-learn.org/stable/modules/decomposition.html
- Projection techniques transform high-dimensional data to a lower-dimensional space while preserving its main structure. Often, the data is transformed to two-dimensional space and visualized as a scatter plot as a means to analyze and understand the data
- Two categories: linear and non-linear projection techniques. 

### Linear methods
- Linear projection techniques produce a linear transformation of data dimensions in lower-dimensional space. Proximity between data points indicates similarity. The more similar data points are, the closer they are located to each other and vice versa. This is why linear projection techniques are also known as global techniques.

#### Principal component analysis (PCA)
- Principal component analysis(PCA) is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components. The number of principal components is less than or equal to the number of original variables. This transformation is defined in such a way that the first principal component has the largest possible variance(that is, accounts for as much of the variability in the data as possible), and each succeeding component in turn has the highest variance possible under the constraint that it is orthogonal to the preceding components. The resulting vectors are an uncorrelated orthogonal basis set.
- http://setosa.io/ev/principal-component-analysis/
- https://www.neuraldesigner.com/blog/principal-components-analysis

#### Non-negative matrix factorization (NMF)
- Non-negative matrix factorization (NNMF, or NMF) is a method for factorizing a matrix into two lower rank matrices with strictly non-negative elements.
- https://en.wikipedia.org/wiki/Non-negative_matrix_factorization
- https://yliapis.github.io/Non-Negative-Matrix-Factorization/
- https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.NMF.html
- https://scikit-learn.org/stable/auto_examples/decomposition/plot_faces_decomposition.html#sphx-glr-auto-examples-decomposition-plot-faces-decomposition-py

#### Generalized Low Rank Models
Extension of the idea of PCA to handle arbitrary data sets consisting of numerical, Boolean, categorical, ordinal, and other data types. This framework encompasses many well known techniques in data analysis, such as nonnegative matrix factorization, matrix completion, sparse and robust PCA,-means,-SVD, and maximum margin matrix factorization. The method handles heterogeneous data sets, and leads to coherent schemes for compressing, denoising, and imputing missing entries across all data types simultaneously. It also admits a number of interesting interpretations of the low rank factors, which allow clustering of examples or of features.
	- https://github.com/cehorn/GLRM
	- #TALK Generalized Low Rank Models - Madeleine Udell: https://www.youtube.com/watch?v=zwvzGuS82MA
	- #TALK Introduction to generalized low-rank models and missing values (OREILLY): 
	  - https://conferences.oreilly.com/strata/strata-eu-2016/public/schedule/detail/49771
	  - http://docs.h2o.ai/h2o/latest-stable/h2o-docs/data-science/glrm.html

#### Dynamic mode decomposition
- https://en.wikipedia.org/wiki/Dynamic_mode_decomposition
- linear dimensionality reduction technique for high-dimensional time-series originating from fluid dynamics. DMD combines the best of two worlds: PCA and Fourier transform. Mathematically, it is related to a fundamental operator in dynamical system theory known as the Koopman operator
- A case against PCA for time-series analysis: https://towardsdatascience.com/a-case-against-pca-for-time-series-analysis-ac66b47629e0
	- Recent studies have shown that DMD behaves as a source separation algorithm (e.g. ICA), although this framework can be more flexible
	- For a similar computational cost, it moreover provides a far more interpretable model than PCA

### Non-linear methods
- Non-linear projection techniques, also known as local projection techniques, aim at preserving the local neighborhoods across the features in the data. Hereby, proximity highlights differences and coherences between observations and is not to put on the same level as similarity

#### Multidimensional scaling (MDS)
- Multidimensional scaling (MDS) is a means of visualizing the level of similarity of individual cases of a dataset. It refers to a set of related ordination techniques used in information visualization, in particular to display the information contained in a distance matrix. It is a form of non-linear dimensionality reduction.

#### Self organizing maps (SOM)
- https://en.wikipedia.org/wiki/Self-organizing_map
- unsupervised machine learning technique used to produce a low-dimensional (typically two-dimensional) representation of a higher dimensional data set while preserving the topological structure of the data
- https://stackabuse.com/self-organizing-maps-theory-and-implementation-in-python-with-numpy/

#### T-distributed Stochastic Neighbor Embedding (t-SNE)
- http://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html
- t-SNE is a tool to visualize high-dimensional data. It converts similarities between data points to joint probabilities and tries to minimize the Kullback-Leibler divergence between the joint probabilities of the low-dimensional embedding and the high-dimensional data. t-SNE has a cost function that is not convex, i.e. with different initializations we can get different results.
- t-SNE is a technique for nonlinear dimensionality reduction that is particularly well suited for the visualization of high-dimensional datasets. The technique can be implemented via Barnes-Hut approximations, allowing it to be applied on large real-world datasets. It is particularly well-suited for embedding high-dimensional data into a space of two or three dimensions, which can then be visualized in a scatter plot. Specifically, it models each high-dimensional object by a two- or three-dimensional point in such a way that similar objects are modeled by nearby points and dissimilar objects are modeled by distant points.
- https://mark-borg.github.io/blog/2016/tsne/
- https://blog.alookanalytics.com/2017/02/28/analytical-market-segmentation-with-t-sne-and-clustering-pipeline/
- How to Use t-SNE Effectively (Interactive): http://distill.pub/2016/misread-tsne/

#### Uniform Manifold Approximation and Projection (UMAP)
- #PAPER UMAP - Uniform Manifold Approximation and Projection for Dimension Reduction (McInnes 2020): https://arxiv.org/abs/1802.03426

