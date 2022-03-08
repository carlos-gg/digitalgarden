---
title: "Gradient boosting"
disableToc: false 
---

See [Ensemble learning](Ensemble%20learning.md)

## Resources
- Outperforms Random Forests and AdaBoost. RF is easier to tune and less prone to overfitting
- http://arogozhnikov.github.io/2016/06/24/gradient_boosting_explained.html
- http://arogozhnikov.github.io/2016/07/05/gradient_boosting_playground.html
- https://www.analyticsvidhya.com/blog/2017/06/which-algorithm-takes-the-crown-light-gbm-vs-xgboost/
- https://www.analyticsvidhya.com/blog/2016/03/complete-guide-parameter-tuning-xgboost-with-codes-python/

## Code
- #CODE Xgboost: https://github.com/dmlc/xgboost
	- Scalable, Portable and Distributed Gradient Boosting (GBDT, GBRT or GBM) Library, for Python, R, Java, Scala, C++ and more. Runs on single machine, Hadoop, Spark, Flink and DataFlow
	- https://xgboost.readthedocs.org/
	- https://www.analyticsvidhya.com/blog/2016/03/complete-guide-parameter-tuning-xgboost-with-codes-python/
- #CODE Light GBM: https://github.com/microsoft/LightGBM
	- a very high-performance gradient boosting tree framework (supporting GBDT, GBRT, GBM, and MART), and its distributed implementation. Part of DMTK (Microsoft)
	- https://www.analyticsvidhya.com/blog/2017/06/which-algorithm-takes-the-crown-light-gbm-vs-xgboost/
	- https://www.techleer.com/articles/489-lightgbm-a-light-gradient-boosting-machine/
- #CODE CatBoost: https://github.com/catboost/catboost/
	- https://catboost.ai/
	- https://catboost.ai/docs/
	- A fast, scalable, high performance Gradient Boosting on Decision Trees library, used for ranking, classification, regression and other machine learning tasks for Python, R, Java, C++. Supports computation on CPU and GPU
	- CatBoost vs. Light GBM vs. XGBoost: https://towardsdatascience.com/catboost-vs-light-gbm-vs-xgboost-5f93620723db
- #CODE https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html


## References
- #PAPER Probabilistic Gradient Boosting Machines for Large-Scale Probabilistic Regression (Sprangers 2021): https://arxiv.org/abs/2106.01682v2
	- #CODE https://paperswithcode.com/paper/probabilistic-gradient-boosting-machines-for?from=n11