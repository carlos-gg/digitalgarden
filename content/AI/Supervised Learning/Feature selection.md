---
title: "Feature selection"
disableToc: false 
---

See [[Regression#Regularized regression]]

- https://en.wikipedia.org/wiki/Feature_selection
- http://machinelearningmastery.com/an-introduction-to-feature-selection/
- http://scikit-learn.org/stable/modules/feature_selection.html

- Removing features with low variance: http://scikit-learn.org/stable/modules/feature_selection.html#removing-features-with-low-variance
- Univariate feature selection: http://scikit-learn.org/stable/modules/feature_selection.html#univariate-feature-selection
- Recursive feature elimination: http://scikit-learn.org/stable/modules/feature_selection.html#recursive-feature-elimination
- Regularization: 
	- http://scikit-learn.org/stable/modules/feature_selection.html#l1-based-feature-selection
	- https://en.wikipedia.org/wiki/Regularization_(mathematics)
	- Penalized regression has been applied widely across many research disciplines, but it is a great fit for business data with many columns, even data sets with more columns than rows, and for data sets with a lot of correlated variables. L1/LASSO penalties drive unnecessary regression parameters to zero, selecting a small, representative subset of regression parameters for the regression model while avoiding potential multiple comparison problems that arise in forward, backward, and stepwise variable selection. Tikhonov/L2/ridge penalties help preserve parameter estimate stability, even when many correlated variables exist in a wide data set or important predictor variables are correlated. It’s also important to know penalized regression techniques don’t always create confidence intervals, t-statistics, or p-values for regression parameters. These types of measures are typically only available through iterative methods or bootstrapping that can require extra computing time.
	- https://www.quora.com/What-is-regularization-in-machine-learning
	- The loss function is penalized by adding an L1 or L2 norm of the weights vector W (the vector of the learned parameters in the linear regression):
		- L(X,Y) + lambda N(W), where N is either the L1, L2 or any other norm.
		- This helps avoiding overfitting and performs fetuses selection for the case of the L1 regularization. Lambda can be chosen by cross-validation. 
- Tree-based methods
	- Random forest, extra trees. Feature importances with forests of trees: http://scikit-learn.org/stable/auto_examples/ensemble/plot_forest_importances.html
	- XGBoost, Feature importance and why it’s important: 
		- http://datawhatnow.com/feature-importance/
		- http://machinelearningmastery.com/feature-importance-and-feature-selection-with-xgboost-in-python/
		- Importance is calculated for a single decision tree by the amount that each attribute split point improves the performance measure, weighted by the number of observations the node is responsible for. The performance measure may be the purity (Gini index) used to select the split points or another more specific error function. The feature importances are then averaged across all of the the decision trees within the model.

## Books
- #BOOK Feature Engineering and Selection: A Practical Approach for Predictive Models (Kuhn 2018): http://www.feat.engineering/index.html

## Code 
- #CODE Scikit-feature:
	- scikit-feature is an open-source feature selection repository in Python developed by Data Mining and Machine Learning Lab at Arizona State University. It is built upon one widely used machine learning package scikit-learn and two scientific computing packages Numpy and Scipy. scikit-feature contains around 40 popular feature selection algorithms, including traditional feature selection algorithms and some structural and streaming feature selection algorithms.
	- http://featureselection.asu.edu/
- #CODE Feature-selector - Feature selector is a tool for dimensionality reduction of machine learning datasets.
	- Methods: Missing Values, Single Unique Values, Collinear Features, Zero Importance Features, Low Importance Features
    - https://github.com/WillKoehrsen/feature-selector/blob/master/Feature%20Selector%20Usage.ipynb
    - https://towardsdatascience.com/a-feature-selection-tool-for-machine-learning-in-python-b64dd23710f0