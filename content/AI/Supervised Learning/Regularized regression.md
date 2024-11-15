---
title: "Regularized regression"
---

> Regularization, in mathematics and statistics and particularly in the field of machine learning, refers to a process of introducing additional information in order to solve an ill-posed problem or to prevent overfitting

> See [[AI/Supervised Learning/Feature selection]]

## Resources
- https://en.wikipedia.org/wiki/Regularization_(mathematics)
- #TALK [Linear Regression, Logistic Regression, SVM](https://www.youtube.com/watch?v=_5lsmWpA5IU)
- [Regularización Lasso L1, Ridge L2 y ElasticNet](https://www.iartificial.net/regularizacion-lasso-l1-ridge-l2-y-elasticnet/)
- https://www.analyticsvidhya.com/blog/2016/01/complete-tutorial-ridge-lasso-regression-python/
- http://www.astroml.org/book_figures/chapter8/fig_lasso_ridge.html
- https://chaoticsenses.wordpress.com/2016/01/20/taming-the-beast-with-regularization-3/
- https://www.cienciadedatos.net/documentos/py14-ridge-lasso-elastic-net-python.html
- [LARS (Least angle regression)](https://en.wikipedia.org/wiki/Least-angle_regression)
- Penalized regression techniques don’t always create confidence intervals, t-statistics, or p-values for regression parameters. These types of measures are typically only available through iterative methods or bootstrapping that can require extra computing time.
- https://www.quora.com/What-is-regularization-in-machine-learning
- The loss function is penalized by adding an L1 or L2 norm of the weights vector W (the vector of the learned parameters in the linear regression):
	- L(X,Y) + lambda N(W), where N is either the L1, L2 or any other norm.
	- This helps avoiding overfitting and performs feature selection for the case of the L1 regularization. Lambda can be chosen by cross-validation. 

### Ridge regression
- [Ridge regression](https://en.wikipedia.org/wiki/Tikhonov_regularization)
- Tikhonov/L2/ridge penalties help preserve parameter estimate stability, even when many correlated variables exist in a wide data set or important predictor variables are correlated

### Elastic net
- https://en.wikipedia.org/wiki/Elastic_net_regularization
- In the fitting linear or logistic regression models, the elastic net is a regularized regression method that linearly combines the L1 and L2 penalties of the lasso and ridge methods.
- http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.ElasticNet.html

### LASSO
- [LASSO](https://en.wikipedia.org/wiki/Lasso_(statistics))
- Least absolute shrinkage and selection operator
- L1/LASSO penalties drive unnecessary regression parameters to zero, selecting a small, representative subset of regression parameters for the regression model while avoiding potential multiple comparison problems that arise in forward, backward, and stepwise variable selection.
- https://www.kirenz.com/post/2019-08-12-python-lasso-regression-auto/
- https://towardsdatascience.com/ridge-and-lasso-regression-a-complete-guide-with-python-scikit-learn-e20e34bcbf0b


## Code
- #CODE [Glmnet_py. Glmnet Vignette (for python)](https://github.com/bbalasub1/glmnet_python) ^glmnetpy