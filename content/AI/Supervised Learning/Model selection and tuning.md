---
title: "Model selection and tuning"
---

> See: 
> - [[AI/AutoML]] 
> - [[AI/DS and DataEng/Data engineering and computer science]]


## Resources
- [Model selection and evaluation](https://scikit-learn.org/stable/model_selection.html)

## Code
See [[AI/DS and DataEng/ML Ops]]
- #CODE [Optuna - A hyperparameter optimization framework](https://github.com/optuna/optuna)
	- https://optuna.org/
- #CODE [Yellowbrick. Visual analysis and diagnostic tools to facilitate machine learning model selection](http://www.scikit-yb.org/en/latest/)
- #CODE [Tune-sklearn](https://github.com/ray-project/tune-sklearn)
	- Tune-sklearn is a drop-in replacement for Scikit-Learn’s model selection module (GridSearchCV, RandomizedSearchCV) with cutting edge hyperparameter tuning techniques
- #CODE [Talos. Hyperparameter Optimization for Keras Models](https://autonomio.github.io/docs_talos/#introduction)
- #CODE [Hyperopt. Distributed Asynchronous Hyperparameter Optimization in Python](http://hyperopt.github.io/hyperopt)
	- [Hyperparameter optimization for neural networks](https://github.com/hyperopt/hyperopt-nnet)
	- [Hyperopt-sklearn](http://hyperopt.github.io/hyperopt-sklearn/)
	- #CODE [Hyperas- Keras + Hyperopt: A very simple wrapper for convenient hyperparameter optimization](https://github.com/maxpumperla/hyperas)
		- http://maxpumperla.github.io/hyperas/
- #CODE [Hyperband - A Novel Bandit-Based Approach to Hyperparameter Optimization](https://github.com/zygmuntz/hyperband)
	- #PAPER https://arxiv.org/abs/1603.06560
	- http://fastml.com/tuning-hyperparams-fast-with-hyperband/

## Bias-variance trade-off
- Problem of minimizing two sources of errors that prevent a supervised learning algorithm from generalizing beyond the training set:
	- High bias  ->  underfitting
	- High variance  ->  overfitting
- [Validation curves: plotting scores to evaluate models](https://scikit-learn.org/stable/modules/learning_curve.html)
- https://www.quora.com/How-would-you-explain-the-bias-variance-tradeoff-to-a-five-year-old
- http://scott.fortmann-roe.com/docs/BiasVariance.html
- http://scott.fortmann-roe.com/docs/MeasuringError.html
- https://elitedatascience.com/bias-variance-tradeoff
- [Overfitting](https://en.wikipedia.org/wiki/Overfitting)
	- https://www.quora.com/What-is-an-intuitive-explanation-of-overfitting
	- https://www.quora.com/How-can-I-avoid-overfitting
	- https://www.quora.com/How-do-we-detect-overfitting-and-under-fitting-in-Machine-Learning

## Cross-validation
- [Train, test and validation](https://machinelearningmastery.com/difference-test-validation-datasets/)
- [Train, test, validation split and cross-validation (scikit-learn documentation)](http://scikit-learn.org/stable/modules/cross_validation.html)
- http://scikit-learn.org/stable/auto_examples/model_selection/plot_roc_crossval.html
- https://sebastianraschka.com/blog/2016/model-evaluation-selection-part3.html
- https://blog.dataiku.com/model-sucks-evaluating-models-validation-set-infographic
- [Making Predictive Models Robust: Holdout vs Cross-Validation](https://www.kdnuggets.com/2017/08/dataiku-predictive-model-holdout-cross-validation.html)
- [How to Train a Final ML Model](http://machinelearningmastery.com/train-final-machine-learning-model/)
- http://nbviewer.jupyter.org/github/cs109/content/blob/master/lec_10_cross_val.ipynb
- [Hyperparameter optimization](https://en.wikipedia.org/wiki/Hyperparameter_(machine_learning))
- [Tuning the hyper-parameters of an estimator (scikit-learn documentation)](https://scikit-learn.org/stable/modules/grid_search.html)
  
  
