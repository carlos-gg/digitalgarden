---
title: "Linear Algebra"
---

## Resources
- https://en.wikipedia.org/wiki/Linear_algebra
- [The Matrix Cookbook (Brandt 2012)](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf)
- [Stanford, Linear algebra refresher](https://stanford.edu/~shervine/teaching/cme-102/linear-algebra)
- Stanford CS229, algebra and calculus refresher: 
	- https://github.com/afshinea/stanford-cs-229-machine-learning/blob/master/en/refresher-algebra-calculus.pdf
	- http://cs229.stanford.edu/section/cs229-linalg.pdf
- http://people.duke.edu/~ccc14/sta-663/LinearAlgebraReview.html
- https://www.khanacademy.org/math/linear-algebra
- http://nbviewer.jupyter.org/github/relopezbriega/relopezbriega.github.io/blob/master/downloads/LinearAlgebraPython.ipynb

### Matrix decompositions
See [[AI/Unsupervised learning/Dimensionality reduction and low rank modeling]]
- https://en.wikipedia.org/wiki/Matrix_decomposition
- http://people.duke.edu/~ccc14/sta-663/LinearAlgebraMatrixDecompWithSolutions.html
- http://hameddaily.blogspot.be/2016/12/simple-matrix-factorization-with.html
- https://sites.google.com/site/igorcarron2/matrixfactorizations
- http://blog.ethanrosenthal.com/2017/06/20/matrix-factorization-in-pytorch/
- https://tryolabs.com/blog/introduction-to-recommender-systems/
- Alternating Least-squares
	- [Fast Python Collaborative Filtering for Implicit Datasets](https://github.com/benfred/implicit)
	- [Recommender system using matrix factorization (SVD, ALS)](http://www.benfrederickson.com/matrix-factorization/)
- Eigen decomposition: 
	- https://en.wikipedia.org/wiki/Eigendecomposition_of_a_matrix
	- http://setosa.io/ev/eigenvectors-and-eigenvalues/
- [LU decomposition](https://en.wikipedia.org/wiki/LU_decomposition)
- [QR decomposition](https://en.wikipedia.org/wiki/QR_decomposition)

#### SVD
See [[AI/Math and Statistics/SVD]] and [[AI/Unsupervised learning/PCA]]

## Code
- #CODE [Tensorly](https://github.com/tensorly/tensorly)
	- http://tensorly.org
	- TensorLy is a Python library that aims at making tensor learning simple and accessible. It allows to easily perform tensor decomposition, tensor learning and tensor algebra. Its backend system allows to seamlessly perform computation with NumPy, PyTorch, JAX, MXNet, TensorFlow or CuPy, and run methods at scale on CPU or GPU
	- https://github.com/JeanKossaifi/tensorly-notebooks/
	- http://tensorly.org/stable/modules/api.html#module-tensorly.decomposition
- #CODE [Eigen - Eigen is a C++ template library for linear algebra: matrices, vectors, numerical solvers, and related algorithms](http://eigen.tuxfamily.org/index.php?title=Main_Page)
- #CODE https://github.com/rballester/tntorch

## Books
- #BOOK [Templates for the Solution of Algebraic Eigenvalue Problems (Bai, Demmel 2000)](https://www.cs.ucdavis.edu/~bai/ET/contents.html)
- #BOOK [High Dimensional Data Analysis 2020 (HDA2020)](https://statomics.github.io/HDA2020/index.html)


## References
- #PAPER [tntorch: Tensor Network Learning with PyTorch (Usvyatsov 2022)](https://arxiv.org/pdf/2206.11128)
	- https://www.marktechpost.com/2022/06/30/eth-zurich-ai-researchers-introduce-tntorch-a-pytorch-powered-tensor-learning-python-library-that-supports-multiple-decompositions-under-a-unified-interface/