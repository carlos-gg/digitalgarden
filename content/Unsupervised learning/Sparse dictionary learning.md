---
title: "Sparse dictionary learning"
---

> Sparse coding is a representation learning method which aims at finding a sparse representation of the input data (also known as sparse coding) in the form of a linear combination of basic elements as well as those basic elements themselves. These elements are called atoms and they compose a dictionary. Atoms in the dictionary are not required to be orthogonal, and they may be an over-complete spanning set

## Resources
- https://en.wikipedia.org/wiki/Sparse_dictionary_learning
- https://en.wikipedia.org/wiki/Compressed_sensing
- As the era of big data dawns upon us, we are now faced with problems where not only the number of records is massive, but also the number of features per record can be massive too. The problems that arise relating to data that is “too wide” is referred to as the curse of dimensionality. It can therefore be vital to take some measures to reduce the dimensionality of the data set while still preserving the (majority of the) information it holds. 
- Sparse coding is a technique for discovering a small number of “representatives” that can be used to reconstruct the original high-dimensional signal. In the linear generative model of sparse coding, given a set of k-dimensional vectors in a (possibly high-dimensional) real space, the goal of sparse coding is to find some number of basis vectors in addition to a sparse weight vector such that the linear combination of the basis vectors and the weight vector closely approximate the input vectors. (Note: there are other techniques for performing sparse coding) 
- A distinguishing feature of sparse coding from other dimensionality reduction procedures (e.g. principal components analysis, singular value decomposition, etc.) is that the number of bases can exceed the input dimension. It is argued in the literature that this may make sparse coding more biologically realistic, as there is some evidence that the primary visual cortex acts in this manner (see e.g. Honglak Lee et al’s 2006 Advances in neural information processing systems paper titled “Efﬁcient sparse coding algorithms”)
- https://paperswithcode.com/task/dictionary-learning/codeless
- Optimizing Orthogonal Matching Pursuit code in Numpy
	- http://vene.ro/blog/optimizing-orthogonal-matching-pursuit-code-in-numpy-part-1.html
	- http://vene.ro/blog/optimizing-orthogonal-matching-pursuit-code-in-numpy-part-2.html
	- https://gist.github.com/vene/996771
- https://earlbellinger.wordpress.com/2013/12/15/sparse-coding/
- https://www.quora.com/Sparse-Coding-what-is-the-step-by-step-implementation-for-sparse-coding-What-does-the-l0-norm-l1-norm-regularization-represent

## Code
- #CODE [Mini-batch dictionary learning (sklearn)](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.MiniBatchDictionaryLearning.html)
- #CODE [modl](https://github.com/arthurmensch/modl)
	- MODL: Massive Online Dictionary Learning
	- This python package allows to perform sparse / dense matrix factorization on fully-observed/missing data very efficiently, by leveraging random subsampling with online learning. It is able to factorize matrices of terabyte scale with hundreds of components in the latent space in a few hours
- #CODE [sparselandtools](https://github.com/fubel/sparselandtools)
	- A Python package for sparse representations and dictionary learning, including matching pursuit, K-SVD and applications
- #CODE [dictlearn](https://github.com/permfl/dictlearn)
	- Dictionary Learning for image processing
- #CODE [mdla](https://github.com/sylvchev/mdla)
	- Multivariate Dictionary Learning Algorithm, for time series
- #CODE [pytorch-lasso](https://github.com/rfeinman/pytorch-lasso)
- #CODE [PyMP](http://mmoussallam.github.io/PyMP/doc.html)


## References
- #PAPER [Online Dictionary Learning for Sparse Coding (Mairal 2009)](https://www.di.ens.fr/~fbach/mairal_icml09.pdf)
- #PAPER [Online Learning for Matrix Factorization and Sparse Coding (Mairal 2010)](https://arxiv.org/abs/0908.0050)
- #PAPER [Sparse Modeling for Image and Vision Processing (Mairal 2014)](https://arxiv.org/pdf/1411.3230)            