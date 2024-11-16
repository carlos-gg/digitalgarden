---
title: "Robust PCA"
---


## Resources
- https://en.wikipedia.org/wiki/Robust_principal_component_analysis
- IALM, GoDec 
	- [http://kastnerkyle.github.io/blog/2014/03/05/matrix-decomposition/](http://kastnerkyle.github.io/blog/2014/03/05/matrix-decomposition/)  
	- [http://blog.shriphani.com/2013/12/18/robust-principal-component-pursuit-background-matrix-recovery/](http://blog.shriphani.com/2013/12/18/robust-principal-component-pursuit-background-matrix-recovery/) 
- Robust PCA missing in scikit-learn 
	- [https://github.com/scikit-learn/scikit-learn/issues/5851](https://github.com/scikit-learn/scikit-learn/issues/5851) 
- [Robust Principal Component Analysis via ADMM in Python](https://jeremykarnowski.wordpress.com/2015/08/31/robust-principal-component-analysis-via-admm-in-python/)

### Godec
- https://sites.google.com/site/godecomposition/home
- https://github.com/niam/godec 
- The most interesting aspect of GoDec is that it builds an extremely simple model and develops an fast, randomized algorithm to produce an approximated low-rank + sparse decomposition when rank and cardinality are constrained, and the extra noise exists. This is always the case in real applications, where the model complexity needs to be pre-determined, and neither the low-rank nor sparse part is the noise. 
- It is worthy to note the difference between GoDec and Robust PCA with its extension stable principal component pursuit (SPCP). They have intersections on their application tasks. But their assumptions to data, their models and optimization algorithms are extirely different, thus they works for different situations. 
- https://tianyizhou.wordpress.com/2011/04/20/learn-low-rank-sparse-structures-via-randomized-alternating-projections/ 
- https://tianyizhou.wordpress.com/2011/11/14/semi-soft-godec-4-times-faster-auto-determined-k/ 
- https://tianyizhou.wordpress.com/2011/08/30/news-about-godec-code-and-icml-2011-paper/ 
- GREB: https://tianyizhou.wordpress.com/2013/02/11/greedy-bilateral-greb-paradigm-for-large-scale-matrix-completion-robust-pca-and-low-rank-approximation/ 


## Code
- https://github.com/jkarnows/rpcaADMM
- [https://github.com/nwbirnie/rpca](https://github.com/nwbirnie/rpca) 
- [https://github.com/dganguli/robust-pca](https://github.com/dganguli/robust-pca) 
	- A Python implementation of R-PCA using principle component pursuit by alternating directions. 
- [https://github.com/dfm/pcp](https://github.com/dfm/pcp) 
	- A Python implementation of the Principal Component Pursuit algorithm
- [https://github.com/apapanico/RPCA](https://github.com/apapanico/RPCA) 
	- Python Implementation of RPCA 
- [https://github.com/kuantkid/PyRPCA/blob/master/](https://github.com/kuantkid/PyRPCA/blob/master/robustpca.py) 
	- Various algorithms for RPCA 
- [https://jeankossaifi.github.io/tensorly/rpca.html](https://jeankossaifi.github.io/tensorly/rpca.html) 
	- Robust Tensor PCA with TensorLy


## References
- #PAPER [Robust Kernel Principal Component Analysis (Nguyen 2008)](https://proceedings.neurips.cc/paper/2008/file/8f53295a73878494e9bc8dd6c3c7104f-Paper.pdf)
- #PAPER [Robust principal component analysis? (Candes 2011)](https://dl.acm.org/doi/10.1145/1970392.1970395)
- #PAPER [Proximal algorithms. Foundations and Trends in optimization (Parikh & Boyd, S, 2013)](http://web.stanford.edu/~boyd/papers/prox_algs.html) 
