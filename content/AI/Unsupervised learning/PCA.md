---
title: "Principal component analysis (PCA)"
---

> Principal component analysis (PCA) is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components. The number of principal components is less than or equal to the number of original variables. This transformation is defined in such a way that the first principal component has the largest possible variance (that is, accounts for as much of the variability in the data as possible), and each succeeding component in turn has the highest variance possible under the constraint that it is orthogonal to the preceding components. The resulting vectors are an uncorrelated orthogonal basis set

## Resources
- https://en.wikipedia.org/wiki/Principal_component_analysis

- http://setosa.io/ev/principal-component-analysis/
- https://www.neuraldesigner.com/blog/principal-components-analysis
- http://stats.stackexchange.com/questions/110508/questions-on-pca-when-are-pcs-independent-why-is-pca-sensitive-to-scaling-why 
- Explained variance ratio:
	- http://sebastianraschka.com/Articles/2015_pca_in_3_steps.html#explained-variance 
	- http://jotterbach.github.io/2016/03/24/Principal_Component_Analysis/ 

### PCA and SVD
- Link between [[AI/Math and Statistics/SVD]] and [[AI/Unsupervised learning/PCA]]: the eigenvectors of DDT are simply the left singular vectors of D. SVD gives us also the eigenvectors of DTD, useful for rows  instead of columns notation (python notation)
- http://stats.stackexchange.com/questions/2691/making-sense-of-principal-component-analysis-eigenvectors-eigenvalues 
- https://www.quora.com/What-is-an-intuitive-explanation-of-singular-value-decomposition-SVD
- https://stats.stackexchange.com/questions/10251/what-is-the-objective-function-of-pca

### Incremental PCA
- https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.IncrementalPCA.html
- This algorithm has constant memory complexity, on the order of `batch_size * n_features`, enabling use of np.memmap files without loading the entire file into memory. For sparse matrices, the input is converted to dense in batches (in order to be able to subtract the mean) which avoids storing the entire dense matrix at any one time.

### Robust PCA
See [[AI/Unsupervised learning/Robust PCA]]

### Multilinear PCA
- https://en.wikipedia.org/wiki/Multilinear_principal_component_analysis
- [http://alumni.media.mit.edu/~maov/tensorfaces/eccv02_corrected.pdf](http://alumni.media.mit.edu/~maov/tensorfaces/eccv02_corrected.pdf) 
- [http://www.comp.hkbu.edu.hk/~haiping/MSL.html](http://www.comp.hkbu.edu.hk/~haiping/MSL.html) 
- [http://www.mathworks.com/matlabcentral/fileexchange/26168-multilinear-principal-component-analysis--mpca](http://www.mathworks.com/matlabcentral/fileexchange/26168-multilinear-principal-component-analysis--mpca)- 
- [http://www.comm.toronto.edu/~kostas/Publications2008/pub/102.pdf](http://www.comm.toronto.edu/~kostas/Publications2008/pub/102.pdf)


## Code
- #CODE https://github.com/jakevdp/wpca

## References
- #PAPER [Principal Component Analysis with Noisy and/or Missing Data (Bailey 2012)](https://arxiv.org/pdf/1208.4122)            
- #PAPER [Weighted principal component analysis: a weighted covariance eigendecomposition approach (Delchambre 2014)](https://arxiv.org/pdf/1412.4533)            
- #PAPER [A Tutorial on Principal Component Analysis (Shlens 2014)](https://arxiv.org/pdf/1404.1100)            
- #PAPER [EigenGame: PCA as a Nash Equilibrium (Gemp 2021)](https://openreview.net/forum?id=NzTU59SYbNq)
	- https://pub.towardsai.net/deepmind-wants-to-reimagine-one-of-the-most-important-algorithms-in-machine-learning-381884d42de