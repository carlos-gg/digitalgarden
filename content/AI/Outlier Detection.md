# Outlier Detection
Most of the approaches belong to [[Unsupervised learning]] although it might be framed as a [[Semi-supervised learning]] problem. In data mining, anomaly detection (also outlier detection) is the identification of rare items, events or observations which raise suspicions by differing significantly from the majority of the data. Typically the anomalous items will translate to some kind of problem such as bank fraud, a structural defect, medical problems or errors in a text. Anomalies are also referred to as outliers, novelties, noise, deviations and exceptions.

- https://towardsdatascience.com/density-based-algorithm-for-outlier-detection-8f278d2f7983 
- https://towardsdatascience.com/a-brief-overview-of-outlier-detection-techniques-1e0b2c19e561 
- Novelty and Outlier Detection: https://scikit-learn.org/stable/modules/outlier_detection.html
- Comparing anomaly detection algorithms for outlier detection on toy datasets: https://scikit-learn.org/stable/auto_examples/plot_anomaly_comparison.html
- Anomaly detection with TensorFlow (VAEs): https://www.youtube.com/watch?v=2K3ScZp1dXQ
- Isolation forest: 
	- #TALK Unsupervised Anomaly Detection with Isolation Forest - Pydata 2018: https://www.youtube.com/watch?v=5p8B2Ikcw-k
	- https://quantdare.com/isolation-forest-algorithm/
	- https://scikit-learn.org/stable/auto_examples/ensemble/plot_isolation_forest.html#sphx-glr-auto-examples-ensemble-plot-isolation-forest-py
	- https://towardsdatascience.com/outlier-detection-with-isolation-forest-3d190448d45e
	- Isolation forest’s basic principle is that outliers are few and far from the rest of the observations. To build a tree (training), the algorithm randomly picks a feature from the feature space and a random split value ranging between the maximums and minimums. This is made for all the observations in the training set. To build the forest a tree ensemble is made averaging all the trees in the forest.
    - Then for prediction, it compares an observation against that splitting value in a “node”, that node will have two node children on which another random comparisons will be made. The number of “splittings” made by the algorithm for an instance is named: “path length”. As expected, outliers will have shorter path lengths than the rest of the observations.
- Local outlier factor: https://scikit-learn.org/stable/auto_examples/neighbors/plot_lof_outlier_detection.html#sphx-glr-auto-examples-neighbors-plot-lof-outlier-detection-py
- One-class SVM
	- https://docs.microsoft.com/en-us/azure/machine-learning/studio-module-reference/one-class-support-vector-machine
	- https://scikit-learn.org/stable/auto_examples/svm/plot_oneclass.html#sphx-glr-auto-examples-svm-plot-oneclass-py
  - Z-score
	- The z-score or standard score of an observation is a metric that indicates how many standard deviations a data point is from the sample’s mean, assuming a gaussian distribution. This makes z-score a parametric method. 
	- Z-score is a simple, yet powerful method to get rid of outliers in data if you are dealing with parametric distributions in a low dimensional feature space. For nonparametric problems Dbscan and Isolation Forests can be good solutions.
- Dbscan
	- Density Based Spatial Clustering of Applications with Noise
	- Dbscan is a density based clustering algorithm, it is focused on finding neighbors by density (MinPts) on an ‘n-dimensional sphere’ with radius ɛ. A cluster can be defined as the maximal set of ‘density connected points’ in the feature space.
	- Dbscan then defines different classes of points: core, border and outlier points.

  
 ## Code
- #CODE Pyod: https://github.com/yzhao062/pyod
	- https://pyod.readthedocs.io/en/latest/
	- PyOD is a comprehensive and scalable Python toolkit for detecting outlying objects in multivariate data. This exciting yet challenging field is commonly referred as Outlier Detection or Anomaly Detection.
 - #CODE Anomaly detection (Twitter, for R): https://github.com/twitter/AnomalyDetection
  
  
 ## References
- #PAPER Modeling Extreme Events in Time Series Prediction (Ding 2019): http://staff.ustc.edu.cn/~hexn/papers/kdd19-timeseries.pdf
- #PAPER Bayesian Anomaly Detection and Classification (2019): https://arxiv.org/abs/1902.08627  
- [[Deep learning]] based approaches:
	- #PAPER Learning Deep Features for One-Class Classification: https://arxiv.org/abs/1801.05365
	- #PAPER Deep One-Class Classification: http://proceedings.mlr.press/v80/ruff18a.html

