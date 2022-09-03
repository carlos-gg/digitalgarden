---
title: "Singular Value Decomposition (SVD)"
---

> The singular value decomposition (SVD) is a factorization of a real or complex matrix. It generalizes the eigendecomposition of a square normal matrix with an orthonormal eigenbasis to any `m x n` matrix

> See [[AI/Unsupervised learning/PCA#PCA and SVD]]

## Resources
- https://en.wikipedia.org/wiki/Singular_value_decomposition
- https://mathworld.wolfram.com/SingularValueDecomposition.html
- [Geometric explanation of SVD and applications](http://www.ams.org/publicoutreach/feature-column/fcarc-svd)
- [Cool Linear Algebra: Singular Value Decomposition](https://andrew.gibiansky.com/blog/mathematics/cool-linear-algebra-singular-value-decomposition/)
- [Singular Value Decomposition as Simply as Possible](https://gregorygundersen.com/blog/2018/12/10/svd/)
- https://jeremykun.com/2016/04/18/singular-value-decomposition-part-1-perspectives-on-linear-algebra/
- Implementations:
	- https://fa.bianp.net/blog/2012/singular-value-decomposition-in-scipy/
	- http://scicomp.stackexchange.com/questions/1861/understanding-how-numpy-does-svd
	- http://scicomp.stackexchange.com/questions/6979/how-is-the-svd-of-a-matrix-computed-in-practice
	- https://software.intel.com/sites/products/documentation/doclib/mkl_sa/11/mkl_lapack_examples/sgesdd.htm 
	- http://www.alglib.net/matrixops/general/svd.php 
	- LAPACK implements a divide and conquer algorithm SGESDD or DGESDD (not the “highly accurate” Golub-Kahan-Reinsch algorithm, SGESVD or DGESVD) 
	- [Truncated SVD by implicitly restarted Lanczos bidiagonalization for Python Numpy](https://github.com/bwlewis/irlbpy)
	- https://stackoverflow.com/questions/15414027/multiprocessing-pool-makes-numpy-matrix-multiplication-slower

### Randomized SVD
- https://gregorygundersen.com/blog/2019/01/17/randomized-svd/
- [Fast Randomized SVD (Meta/Facebook research)](https://research.facebook.com/blog/2014/09/fast-randomized-svd/)

## Talks
- #TALK [SVD (MIT, Gilbert Strang)](https://www.youtube.com/watch?v=mBcLRGuAFUk)
- #TALK [Singular Value Decomposition (SVD): Mathematical Overview](https://www.youtube.com/watch?v=nbBvuuNVfco)
- #TALK [Randomized Singular Value Decomposition (SVD)](https://www.youtube.com/watch?v=fJ2EyvR85ro)

## References
- #PAPER [Singular value decomposition and least squares solutions (Golub & Reinsch 1970)](https://link.springer.com/article/10.1007/BF02163027)
	- http://people.duke.edu/~hpgavin/SystemID/References/Golub+Reinsch-NM-1970.pdf
- #PAPER [Finding structure with randomness: Probabilistic algorithms for constructing approximate matrix decompositions (Halko 2010)](https://arxiv.org/pdf/0909.4061)            
