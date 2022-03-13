---
title: "Supervised Learning"
disableToc: false 
---

## Resources
- https://en.wikipedia.org/wiki/Supervised_learning
- [Supervised Learning cheatsheet](https://stanford.edu/~shervine/teaching/cs-229/cheatsheet-supervised-learning)
- http://scikit-learn.org/stable/supervised_learning.html
- Metrics:
	- http://docs.aws.amazon.com/machine-learning/latest/dg/binary-model-insights.html
	- ROC curves, AUC
		- http://www.dataschool.io/roc-curves-and-auc-explained/
		- http://corysimon.github.io/articles/what-is-an-roc-curve/


### Classification
See [Classification](AI/Supervised%20Learning/Classification.md)

### Regression
See [Regression](AI/Supervised%20Learning/Regression.md)

### Structured learning
- https://en.wikipedia.org/wiki/Structured_prediction

### Ensemble learning
See [Ensemble learning](AI/Supervised%20Learning/Ensemble%20learning.md)

### Class imbalance
See [Class imbalance](AI/Supervised%20Learning/Class%20imbalance.md)

### Model selection and tuning
See [Model selection and tuning](AI/Supervised%20Learning/Model%20selection%20and%20tuning.md)

### Probability calibration
- https://en.wikipedia.org/wiki/Calibration_(statistics)
- https://scikit-learn.org/stable/modules/calibration.html
- When performing classification you often want not only to predict the class label, but also obtain a probability of the respective label. This probability gives you some kind of confidence on the prediction. Some models can give you poor estimates of the class probabilities and some even do not support probability prediction. 
- Well calibrated classifiers are probabilistic classifiers for which the output of the predict_proba method can be directly interpreted as a confidence level. For instance, a well calibrated (binary) classifier should classify the samples such that among the samples to which it gave a predict_proba value close to 0.8, approximately 80% actually belong to the positive class.
- https://scikit-learn.org/stable/auto_examples/calibration/plot_compare_calibration.html
- Isotonic regression: 
	- https://scikit-learn.org/stable/modules/isotonic.html
	- Isotonic regression is a probability calibration technique which can calibrate classifier scores to approximate probability values by fitting a stepwise non-decreasing function along the scores returned by the classifier.