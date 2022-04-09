---
title: "Classification"
---

## Resources
- https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/Multi-Class%20Classification.ipynb
- Comparison of classifiers
	- https://www.quora.com/What-are-the-advantages-of-different-classification-algorithms
	- http://scikit-learn.org/stable/auto_examples/classification/plot_classifier_comparison.html
- https://medium.com/@maheshkkumar/implementing-a-binary-classifier-in-python-b69d08d8da21#.goynlh7ah
- Metrics
	- https://www.neuraldesigner.com/blog/methods-binary-classification
	- http://machinelearningmastery.com/classification-accuracy-is-not-enough-more-performance-measures-you-can-use/
	- http://docs.aws.amazon.com/machine-learning/latest/dg/binary-model-insights.html

### Naive Bayes
- https://blancosilva.wordpress.com/2012/06/21/naive-bayes/
- https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/Supervised%20Learning%20-%20Naive%20Bayes.ipynb
- http://stackoverflow.com/questions/10059594/a-simple-explanation-of-naive-bayes-classification?rq=1
- https://monkeylearn.com/blog/practical-explanation-naive-bayes-classifier/
- #TALK [5 Minutes With Ingo - Naïve Bayes](https://www.youtube.com/watch?v=IlVINQDk4o8)

### Support Vector Machine (SVM)
- Given a set of training examples, each marked as belonging to one or the other of two categories, an SVM training algorithm builds a model that assigns new examples to one category or the other, making it a non-probabilistic binary linear classifier. An SVM model is a representation of the examples as points in space, mapped so that the examples of the separate categories are divided by a clear gap that is as wide as possible. SVM figures out how to separate the data based on the labels or outputs we’ve defined.
- SVMs can efficiently perform a non-linear classification using what is called the kernel trick, implicitly mapping their inputs into high-dimensional feature spaces. It's much more computationally intensive. Complexity: O(n^3m), n number of points, m number of dimensions
- https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/Support%20Vector%20Machines.ipynb
- https://monkeylearn.com/blog/introduction-to-support-vector-machines-svm/
- http://blog.yhat.com/posts/why-support-vector-machine.html
- The kernel trick takes the data you give it and transforms it. In expanding the dataset there are now more obvious boundaries between your classes and the SVM algorithm is able to compute a much more optimal hyperplane.
- #TALK [How Support Vector Machines work / How to open a black box (Brandon Rohrer)](https://www.youtube.com/watch?v=-Z4aojJ-pdg&t=331s)
- #TALK 5 Minutes With Ingo - Understanding Support Vector Machines: 
	- https://www.youtube.com/watch?v=YsiWisFFruY
	- https://www.youtube.com/watch?v=woEwY0Zi6X4
- #TALK [How SVM (Support Vector Machine) algorithm works](https://www.youtube.com/watch?v=1NxnPkZM9bc)

### K-nearest neighbors
See [[AI/Supervised Learning/Regression]]

### Logistic regression
- https://en.wikipedia.org/wiki/Logistic_regression
- In statistics, logistic regression, or logit regression, or logit model is a regression model where the dependent variable (DV) is categorical. This is the case of a binary dependent variable, which can take only two values, "0" and “1”.
- Cases where the dependent variable has more than two outcome categories may be analysed in multinomial logistic regression, or, if the multiple categories are ordered, in ordinal logistic regression.
- http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
- https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/Supervised%20Learning%20-%20Logistic%20Regression.ipynb
- http://www.kdnuggets.com/2017/02/gentlest-introduction-tensorflow-part-4.html
- https://stats.stackexchange.com/questions/228763/regularization-methods-for-logistic-regression
- Regularization can be used in all linear methods, including both regression and classification. There is not too much difference between regression and classification: the only difference is the loss function. Specifically, there are three major components of a linear method: Loss Function, Regularization,  Algorithms. Where loss function plus regularization is the objective function in the problem in optimization form and the algorithm is the way to solve it. 
- Logistic loss can be used for classification: L(y, y’) = log(1 + exp(−y’y))
- Logistic regression with L2 regularization: minimizew ∑_x,y log(1 + exp(−w^T x⋅y)) + λw^Tw


### Gaussian Processes
See [[AI/Supervised Learning/Regression]] 

### Tree-based approaches
See [[AI/Supervised Learning/Ensemble learning]], [[AI/Supervised Learning/Random forest]] and [[AI/Supervised Learning/Gradient boosting]]

- https://github.com/jmportilla/Udemy---Machine-Learning/blob/master/Decision%20Trees%20and%20Random%20Forests.ipynb
- https://www.analyticsvidhya.com/blog/2016/04/complete-tutorial-tree-based-modeling-scratch-in-python/
- Decision trees (DT): DT-learning uses a decision tree as a predictive model which maps observations about an item (represented in the branches) to conclusions about the item's target value (represented in the leaves). Tree models where the target variable can take a finite set of values are called classification trees; in these tree structures, leaves represent class labels and branches represent conjunctions of features that lead to those class labels. Decision trees where the target variable can take continuous values (typically real numbers) are called regression trees.


