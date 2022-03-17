---
title: "Anomaly and Outlier Detection"
disableToc: false 
---

See "Active learning for anomaly discovery" section in [Active learning](AI/Active%20learning.md)

## Resources
- Most of the outlier detection approaches belong to [Unsupervised learning](AI/Unsupervised%20learning/Unsupervised%20learning.md) although it might be framed as a [Semi-supervised learning](AI/Semi-supervised%20learning.md) problem. In data mining, anomaly detection (also outlier detection) is the identification of rare items, events or observations which raise suspicions by differing significantly from the majority of the data. Typically the anomalous items will translate to some kind of problem such as bank fraud, a structural defect, medical problems or errors in a text. Anomalies are also referred to as outliers, novelties, noise, deviations and exceptions.
- https://towardsdatascience.com/density-based-algorithm-for-outlier-detection-8f278d2f7983 
- https://towardsdatascience.com/a-brief-overview-of-outlier-detection-techniques-1e0b2c19e561 
- [Novelty and Outlier Detection](https://scikit-learn.org/stable/modules/outlier_detection.html)
- [Comparing anomaly detection algorithms for outlier detection on toy datasets](https://scikit-learn.org/stable/auto_examples/plot_anomaly_comparison.html)
- #TALK [Anomaly detection with TensorFlow (VAEs)](https://www.youtube.com/watch?v=2K3ScZp1dXQ)
- [Local outlier factor](https://scikit-learn.org/stable/auto_examples/neighbors/plot_lof_outlier_detection.html#sphx-glr-auto-examples-neighbors-plot-lof-outlier-detection-py)
- One-class SVM
	- https://docs.microsoft.com/en-us/azure/machine-learning/studio-module-reference/one-class-support-vector-machine
	- https://scikit-learn.org/stable/auto_examples/svm/plot_oneclass.html#sphx-glr-auto-examples-svm-plot-oneclass-py
  - Z-score
	- The z-score or standard score of an observation is a metric that indicates how many standard deviations a data point is from the sample’s mean, assuming a gaussian distribution. This makes z-score a parametric method. 
	- Z-score is a simple, yet powerful method to get rid of outliers in data if you are dealing with parametric distributions in a low dimensional feature space. For nonparametric problems Dbscan and Isolation Forests can be good solutions.
- Dbscan
	- Density Based Spatial Clustering of Applications with Noise
	- Dbscan is a density based clustering algorithm, it is focused on finding neighbors by density (MinPts) on an ‘n-dimensional sphere’ with radius ɛ. A cluster can be defined as the maximal set of 'density connected points' in the feature space.
	- Dbscan then defines different classes of points: core, border and outlier points.

  
## Code
- #CODE [Pyod](https://github.com/yzhao062/pyod)
	- https://pyod.readthedocs.io/en/latest/
	- PyOD is a comprehensive and scalable Python toolkit for detecting outlying objects in multivariate data. This exciting yet challenging field is commonly referred as Outlier Detection or Anomaly Detection.
 - #CODE [Anomaly detection (Twitter, for R)](https://github.com/twitter/AnomalyDetection)
  
  
## References
- #PAPER [Isolation forest (Liu 2008)](https://ieeexplore.ieee.org/document/4781136 )
	- #TALK [Unsupervised Anomaly Detection with Isolation Forest - Pydata 2018](https://www.youtube.com/watch?v=5p8B2Ikcw-k)
	- https://quantdare.com/isolation-forest-algorithm/
	- https://scikit-learn.org/stable/auto_examples/ensemble/plot_isolation_forest.html#sphx-glr-auto-examples-ensemble-plot-isolation-forest-py
	- https://towardsdatascience.com/outlier-detection-with-isolation-forest-3d190448d45e
	- Isolation forest’s basic principle is that outliers are few and far from the rest of the observations. To build a tree (training), the algorithm randomly picks a feature from the feature space and a random split value ranging between the maximums and minimums. This is made for all the observations in the training set. To build the forest a tree ensemble is made averaging all the trees in the forest.
    - Then for prediction, it compares an observation against that splitting value in a “node”, that node will have two node children on which another random comparisons will be made. The number of “splittings” made by the algorithm for an instance is named: “path length”. As expected, outliers will have shorter path lengths than the rest of the observations.
- #PAPER [Modeling Extreme Events in Time Series Prediction (Ding 2019)](http://staff.ustc.edu.cn/~hexn/papers/kdd19-timeseries.pdf)
- #PAPER [Bayesian Anomaly Detection and Classification (2019)](https://arxiv.org/abs/1902.08627  )


### DL-based
See "GANs for anomaly detection" section in [GANs](AI/Deep%20learning/GANs.md)

- #PAPER [Learning Deep Features for One-Class Classification (Perera 2018)](https://arxiv.org/abs/1801.05365)
- #PAPER [Deep One-Class Classification (Ruff 2018)](http://proceedings.mlr.press/v80/ruff18a.html)
- #PAPER [Learning and Evaluating Representations for Deep One-Class Classification (Sohn 2021)](https://openreview.net/forum?id=HCSgyPUfeDj)
	- #CODE https://github.com/google-research/deep_representation_one_class
	- https://ai.googleblog.com/2021/09/discovering-anomalous-data-with-self.html
- #PAPER [VOS: Learning What You Don't Know by Virtual Outlier Synthesis (Du 2022)](https://arxiv.org/pdf/2202.01197)
	- #CODE https://github.com/deeplearning-wisc/vos
	- [Paper explained](https://www.youtube.com/watch?v=i-J4T3uLC9M&list=WL&index=59&t=4s)

#### Code
- #CODE [Anomalib](https://github.com/openvinotoolkit/anomalib)
	- An anomaly detection library comprising state-of-the-art algorithms and features such as experiment management, hyper-parameter optimization, and edge inference
	- https://openvinotoolkit.github.io/anomalib/
	- Anomalib is a deep learning library that aims to collect state-of-the-art anomaly detection algorithms for benchmarking on both public and private datasets
- #CODE [Orion - A machine learning library for detecting anomalies in signals](https://github.com/signals-dev/Orion) ^oriontfanomalies
	- https://sintel.dev/Orion/
	- Orion is a machine learning library built for unsupervised time series anomaly detection