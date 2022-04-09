---
title: "Class imbalance"
---

## Resources
- https://en.wikipedia.org/wiki/Oversampling_and_undersampling_in_data_analysis
- http://www.marcoaltini.com/blog/dealing-with-imbalanced-data-undersampling-oversampling-and-proper-cross-validation
- http://www.alfredo.motta.name/cross-validation-done-wrong/
- http://www.win-vector.com/blog/2015/02/does-balancing-classes-improve-classifier-performance/
- http://www.chioka.in/class-imbalance-problem/
- http://www.kdnuggets.com/2017/06/7-techniques-handle-imbalanced-data.html
- https://svds.com/learning-imbalanced-classes/
	- Conventional algorithms are often biased towards the majority class because their loss functions attempt to optimize quantities such as error rate, not taking the data distribution into consideration. Result: a trivial classifier that classifies every example as the majority class.

## Code
- #CODE [Imbalanced-learn](https://github.com/scikit-learn-contrib/imbalanced-learn )
	- https://imbalanced-learn.readthedocs.io/en/stable/
	- https://imbalanced-learn.readthedocs.io/en/stable/api.html
- #CODE [Smote_variants](https://github.com/analyticalmindsltd/smote_variants)
	- http://smote-variants.readthedocs.io/
	-  The package implements 85 variants of the Synthetic Minority Oversampling Technique (SMOTE). Besides the implementations, an easy to use model selection framework is supplied to enable the rapid evaluation of oversampling techniques on unseen datasets. 

## Approaches
### Resampling
- Balance the training dataset
- #PAPER [Survey of resampling techniques for improving classification performance in unbalanced datasets (More 2016)](https://arxiv.org/abs/1608.06048)

#### Oversampling
- #PAPER [SMOTE: Synthetic Minority Over-sampling Technique (Chaula 2002)](https://jair.org/index.php/jair/article/view/10302)
	- There are a number of methods available to oversample a dataset used in a typical classification problem (using a classification algorithm to classify a set of images, given a labelled training set of images). The most common technique is known as SMOTE. 
	- https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/
- #PAPER [ADASYN: Adaptive synthetic sampling approach for imbalanced learning (He 2008)](https://ieeexplore.ieee.org/document/4633969)
	- https://sci2s.ugr.es/keel/pdf/algorithm/congreso/2008-He-ieee.pdf
	- ADASYN builds on the methodology of SMOTE, by shifting the importance of the classification boundary to those minority classes which are difficult. ADASYN uses a weighted distribution for different minority class examples according to their level of difficulty in learning, where more synthetic data is generated for minority class examples that are harder to learn.

#### Undersampling
- Down-sampling involves randomly removing observations from the majority class to prevent its signal from dominating the learning algorithm. The most common heuristic for doing so is resampling without replacement.
- https://machinelearningmastery.com/undersampling-algorithms-for-imbalanced-classification/
- Cluster. Cluster centroids is a method that replaces cluster of samples by the cluster centroid of a K-means algorithm, where the number of clusters is set by the level of undersampling.
- Tomek links. Tomek links remove unwanted overlap between classes where majority class links are removed until all minimally distanced nearest neighbor pairs are of the same class. Tomek links are pairs of instances of opposite classes who are their own nearest neighbors. Tomek’s algorithm looks for such pairs and removes the majority instance of the pair.
	- [Classification of Imbalance Data using Tomek Link (T-Link) Combined with Random Under-sampling (RUS) as a Data Reduction Method](https://pdfs.semanticscholar.org/6ec4/18f9071f3a96d5548e87e34be3665703119e.pdf)
- Throw away minority examples and switch to an anomaly detection framework

### Adjust the class importance or the metric
- At the algorithm level, or after: Adjust the class weight (misclassification costs), adjust the decision threshold. Many machine learning toolkits have ways to adjust the “importance” of classes (classifiers that take an optional class_weight). 
- Change the metric. 
	- Evaluating the classifier: Accuracy is not a good metric for imbalanced classes!!
	- Use a ROC curve
	- Don’t get hard classifications (labels) from your classifier (via score or predict). Instead, get probability estimates via proba or predict_proba
	- No matter what you do for training, always test on the natural (stratified) distribution your classifier is going to operate upon. Seesklearn.cross_validation.StratifiedKFold
	- For a singe metric (value): AUC, F1 (harmonic mean of precision and recall), Cohen’s Kappa (evaluation statistic that takes into account how much agreement would be expected by chance)
	- https://medium.com/towards-data-science/what-metrics-should-we-use-on-imbalanced-data-set-precision-recall-roc-e2e79252aeba
	- http://machinelearningmastery.com/classification-accuracy-is-not-enough-more-performance-measures-you-can-use/
	- The following performance measures that can give more insight into the accuracy of the model than traditional classification accuracy:
		- Confusion Matrix: A breakdown of predictions into a table showing correct predictions (the diagonal) and the types of incorrect predictions made (what classes incorrect predictions were assigned).
		- Precision: A measure of a classifiers exactness.
		- Recall: A measure of a classifiers completeness
		- F1 Score (or F-score): A weighted average of precision and recall.
		- Kappa (or Cohen’s kappa): Classification accuracy normalized by the imbalance of the classes in the data.
		- ROC Curves: Like precision and recall, accuracy is divided into sensitivity and specificity and models can be chosen based on the balance thresholds of these values.

### Cost-sensitive training
- Cost-Sensitive Training. For this tactic we use penalized learning algorithms that increase the cost of classification mistakes on the minority class. A popular algorithm for this technique is Penalized-SVM. During training, we can use the argument class_weight='balanced'  to penalize mistakes on the minority class by an amount proportional to how under-represented it is.

### Select or create a suitable algorithm
- Create new algorithm for the imbalanced classes situation, or use one which handles the data imbalance
- #PAPER [Boosting/bagging. Comparing Boosting and Bagging Techniques With Noisy and Imbalanced Data (Khoshgoftaar 2010)](https://ieeexplore.ieee.org/document/5645694?arnumber=5645694)
	- The experiments show that the bagging techniques generally outperform boosting, and hence in noisy data environments, bagging is the preferred method for handling class imbalance.
