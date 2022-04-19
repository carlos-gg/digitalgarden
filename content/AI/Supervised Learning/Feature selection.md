---
title: "Feature selection"
---

> See:
> - [[AI/Supervised Learning/Regularized regression]]
> - [[AI/Feature learning]]

## Resources
- https://en.wikipedia.org/wiki/Feature_selection
- http://machinelearningmastery.com/an-introduction-to-feature-selection/
- http://scikit-learn.org/stable/modules/feature_selection.html
- [Removing features with low variance](http://scikit-learn.org/stable/modules/feature_selection.html#removing-features-with-low-variance)
- [Univariate feature selection](http://scikit-learn.org/stable/modules/feature_selection.html#univariate-feature-selection)
- [Recursive feature elimination](http://scikit-learn.org/stable/modules/feature_selection.html#recursive-feature-elimination)
 
### Regularization
See [[AI/Supervised Learning/Regularized regression]]
- http://scikit-learn.org/stable/modules/feature_selection.html#l1-based-feature-selection

### Tree-based methods
- https://scikit-learn.org/stable/modules/feature_selection.html#tree-based-feature-selection
- [Random forest, extra trees. Feature importances with forests of trees](http://scikit-learn.org/stable/auto_examples/ensemble/plot_forest_importances.html)
- XGBoost, Feature importance and why it’s important: 
	- http://datawhatnow.com/feature-importance/
	- http://machinelearningmastery.com/feature-importance-and-feature-selection-with-xgboost-in-python/
	- Importance is calculated for a single decision tree by the amount that each attribute split point improves the performance measure, weighted by the number of observations the node is responsible for. The performance measure may be the purity (Gini index) used to select the split points or another more specific error function. The feature importances are then averaged across all of the the decision trees within the model.

## Books
- #BOOK [Feature Engineering and Selection: A Practical Approach for Predictive Models (Kuhn 2018)](http://www.feat.engineering/index.html)

## Code 
- #CODE [Scikit-feature](https://github.com/jundongl/scikit-feature)
	- http://featureselection.asu.edu/
- #CODE Feature-selector - Feature selector is a tool for dimensionality reduction of machine learning datasets.
	- Methods: Missing Values, Single Unique Values, Collinear Features, Zero Importance Features, Low Importance Features
    - https://github.com/WillKoehrsen/feature-selector/blob/master/Feature%20Selector%20Usage.ipynb
    - https://towardsdatascience.com/a-feature-selection-tool-for-machine-learning-in-python-b64dd23710f0
- #CODE [ITMO_FS](https://github.com/ctlab/ITMO_FS)
	- Feature selection library in python
	- https://itmo-fs.readthedocs.io/en/latest/