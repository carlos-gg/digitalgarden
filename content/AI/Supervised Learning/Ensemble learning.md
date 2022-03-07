---
title: "Ensemble learning"
disableToc: false 
---

- https://en.wikipedia.org/wiki/Ensemble_learning
- In statistics and machine learning, ensemble methods use multiple learning algorithms to obtain better predictive performance than could be obtained from any of the constituent learning algorithms alone. By analogy, ensemble techniques have been used also in [[unsupervised learning]] scenarios, for example in consensus clustering or in anomaly or [[AI/Anomaly and Outlier Detection]]
- In general, ensembling is a technique of combining two or more algorithms of similar or dissimilar types called base learners. This is done to make a more robust system (improving generalizability / robustness over a single estimator) which incorporates the predictions from all the base learners.

- http://scikit-learn.org/stable/modules/ensemble.html
- http://mlwave.com/kaggle-ensembling-guide/
- https://www.analyticsvidhya.com/blog/2016/04/complete-tutorial-tree-based-modeling-scratch-in-python/
- http://www.datasciencecentral.com/profiles/blogs/improving-predictions-with-ensemble-model
- http://www.kdnuggets.com/2016/11/data-science-basics-intro-ensemble-learners.html
- https://medium.com/diogo-menezes-borges/ensemble-learning-when-everybody-takes-a-guess-i-guess-ec35f6cb4600
- https://blog.statsbot.co/ensemble-learning-d1dcd548e936
- How to Reduce Variance in the Final DL Model With a Horizontal Voting Ensemble: https://machinelearningmastery.com/horizontal-voting-ensemble/


## Bagging
- With bootstrap aggregating (Bagging) we build models of smaller datasets by sampling with replacement. The results of these bootstrap samples are then aggregated, using majority voting (equal weighting of models)

### [[Random Forest]]

## Boosting
See [[Gradient boosting]]
- Same as bagging but operates via weighted voting. Algorithm proceeds iteratively (one tries to reduce the bias of the combined estimator); new models are influenced by previous ones. E.g. AdaBoost (Adaptive Boosting) and LogitBoost
- https://en.wikipedia.org/wiki/AdaBoost

## Stacking
- uses a meta learner (as opposed to bagging/boosting which use voting schemes)
- It consists in training multiple learners/algorithms (as opposed to bagging/boosting which train a single learner).  Each learner uses a subset of data. 
- A "combiner" is trained on a validation set. This combiner can be any ensemble technique, but logistic regression is often found to be an adequate and simple algorithm to perform this combining.
- http://blog.kaggle.com/2016/12/27/a-kagglers-guide-to-model-stacking-in-practice/
- https://machinelearningmastery.com/ensemble-methods-for-deep-learning-neural-networks/