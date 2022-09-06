---
title: "Regression"
---

> In statistical modeling, regression analysis is a set of statistical processes for estimating the relationships between a dependent variable (often called the 'outcome' or 'response' variable) and one or more independent variables (often called 'predictors', 'covariates', 'explanatory variables' or 'features')

> See: 
> - [[AI/Supervised Learning/Regularized regression]]
> - [[AI/Time Series analysis]]
> - [[AI/Forecasting]]
> - [[AI/Deep learning/RNNs]]
> - "Sequence time series modelling" section in [[AI/Deep learning/CNNs]]


## Resources
- https://en.wikipedia.org/wiki/Regression_analysis
- https://www.analytics. idhya.com/blog/2015/08/comprehensive-guide-regression/
- https://towardsdatascience.com/a-beginners-guide-to-regression-analysis-in-machine-learning-8a828b491bbf
- http://www.datasciencecentral.com/profiles/blogs/10-types-of-regressions-which-one-to-use
- http://www.datasciencecentral.com/profiles/blogs/23-types-of-regression
- [Curve fitting vs regression](https://blog.datazar.com/curve-fitting-vs-regression-752ce295b0b1)
- Goodness of fit:
	- [Coefficient of determination (The R-squared measure of goodness of fit)](http://blog.minitab.com/blog/adventures-in-statistics-2/regression-analysis-how-do-i-interpret-r-squared-and-assess-the-goodness-of-fit)
	- Reduced chi-squared
- [Linear models](http://scikit-learn.org/stable/modules/linear_model.html)
- Multicollinearity:
	- [Dealing With Multicollinearity: A Brief Overview and Introduction to Tolerant Methods](https://waterprogramming.wordpress.com/2017/02/22/dealing-with-multicollinearity-a-brief-overview-and-introduction-to-tolerant-methods/)
	- https://stackoverflow.com/questions/42904211/lasso-or-ridge-for-correlated-variables
	- [Permutation Importance with Multicollinear or Correlated Features (scikit-learn)](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance_multicollinear.html)
1
### Linear Regression
- https://en.wikipedia.org/wiki/Linear_regression
- In statistics, linear regression is an approach for modeling the relationship between a scalar dependent variable y and one or more explanatory variables (or independent variables) denoted X. The case of one explanatory variable is called simple linear regression. For more than one explanatory variable, the process is called multiple linear regression.
- http://www.datasciencecentral.com/profiles/blogs/linear-regression-geometry
- https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/Supervised%20Learning%20-%20%20Linear%20Regression.ipynb

### Least squares
- https://en.wikipedia.org/wiki/Least_squares
- The method of least squares is a standard approach in regression analysis to the approximate solution of overdetermined systems, i.e., sets of equations in which there are more equations than unknowns. "Least squares" means that the overall solution minimizes the sum of the squares of the errors made in the results of every single equation. The most important application is in data fitting. The best fit in the least-squares sense minimizes the sum of squared residuals (a residual being: the difference between an observed value, and the fitted value provided by a model).
- [Cook's D](https://en.wikipedia.org/wiki/Cook%27s_distance)
	- In statistics, Cook's distance or Cook's D is a commonly used estimate of the influence of a data point when performing a least-squares regression analysis. In a practical ordinary least squares analysis, Cook's distance can be used in several ways: to indicate influential data points that are particularly worth checking for validity; or to indicate regions of the design space where it would be good to be able to obtain more data points.
	- https://www.mathworks.com/examples/statistics/mw/stats-ex80505511-determine-outliers-using-cook-s-distance
- Ordinary least squares (OLS): 
	- https://en.wikipedia.org/wiki/Ordinary_least_squares
	- http://setosa.io/ev/ordinary-least-squares-regression/
- Non-linear least squares: 
	- https://en.wikipedia.org/wiki/Non-linear_least_squares
	- Non-linear least squares is the form of least squares analysis used to fit a set of m observations with a model that is non-linear in n unknown parameters (m> n).

### Principal component regression
- https://en.wikipedia.org/wiki/Principal_component_regression

### Generalized linear models (GLM)
- https://en.wikipedia.org/wiki/Generalized_linear_model
	- GLM is a flexible generalization of ordinary linear regression that allows for the response variable to have an error distribution other than the normal distribution
- [Generalized Linear Models](https://scikit-learn.org/0.15/modules/linear_model.html)
- [Understand Generalized Linear Models, and How It Relates to Linear, Logistic and Poisson Regression](https://towardsdatascience.com/understand-generalized-linear-models-and-how-it-relates-to-linear-logistic-and-poisson-regression-53f3aea8a9d)
- https://towardsdatascience.com/beyond-linear-regression-an-introduction-to-glms-7ae64a8fad9c
	- Under the GLM assumptions, the output variable Y can now follow any probability distribution within the “exponential family”, which includes not only the exponential distribution, but also the normal, gamma, chi-squared, Poisson, binomial (for a fixed number of trails), negative binomial (for a fixed number of failures), beta and lognormal distributions, among others
 
### Logistic regression 
See [[AI/Supervised Learning/Classification]]

### Regularized regression
See [[AI/Supervised Learning/Regularized regression]]

### SVM
See [[AI/Supervised Learning/Classification]]

### Gaussian Process
See [[AI/Supervised Learning/Gaussian Process]]

### Tree-based approaches
See [[AI/Supervised Learning/Ensemble learning]] and [[AI/Supervised Learning/Classification]]

### K-nearest neighbors
- https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm
- k-NN is a non-parametric method used for classification and regression. In both cases, the input consists of the k closest training examples in the feature space. The output depends on whether k-NN is used for classification or regression:
	- for classification - An object is classified by a majority vote of its k nearest neighbors.
	- for regression - The value is the average of the values of its k nearest neighbors.
- k-NN is a type of instance-based learning, or lazy learning, where the function is only approximated locally and all computation is deferred until classification. The k-NN algorithm is among the simplest of all machine learning algorithms.

### Approximate nearest neighbors
- https://en.wikipedia.org/wiki/Nearest_neighbor_search
- ANN benchmarks:
	- http://ann-benchmarks.com/
	- https://github.com/erikbern/ann-benchmarks
	- https://erikbern.com/2018/02/15/new-benchmarks-for-approximate-nearest-neighbors.html
	- https://erikbern.com/2018/06/17/new-approximate-nearest-neighbor-benchmarks.html


## Code
- #CODE [Annoy](https://github.com/spotify/annoy) (Spotify)
	- Approximate Nearest Neighbors in C++/Python optimized for memory usage and loading/saving to disk
- #CODE [FALCONN](https://github.com/FALCONN-LIB/FALCONN) - FAst Lookups of Cosine and Other Nearest Neighbors
	- Locality-Sensitive Hashing (LSH), nearest neighbor search in high-dimensional spaces
- #CODE [NMSLIB](https://github.com/nmslib/nmslib)
	- Non-Metric Space Library. Efficient cross-platform similarity search library and a toolkit for evaluation of similarity search methods. The core-library does not have any third-party dependencies
- #CODE [FAISS (Facebook)](https://github.com/facebookresearch/faiss)
	- Faiss is a library for efficient similarity search and clustering of dense vectors. It contains algorithms that search in sets of vectors of any size, up to ones that possibly do not fit in RAM. It also contains supporting code for evaluation and parameter tuning. Faiss is written in C++ with complete wrappers for Python/numpy. Some of the most useful algorithms are implemented on the GPU. It is developed by Facebook AI Research.


