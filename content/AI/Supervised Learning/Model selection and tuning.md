---
title: "Model selection and tuning"
---

> See: 
> - [[AI/AutoML]] 
> - [[AI/DS and DataEng/Data engineering and computer science]]
> - [[AI/DS and DataEng/ML Ops]]


## Resources
- [Model selection and evaluation](https://scikit-learn.org/stable/model_selection.html)

### Bias-variance trade-off
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

### Cross-validation
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

## Code
- See [[AI/DS and DataEng/ML Ops]]
- #CODE [Vizier](https://github.com/google/vizier) - Python-based research interface for blackbox and hyperparameter optimization, based on the internal Google Vizier Service
	- https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html
	- #PAPER [Open Source Vizier: Distributed Infrastructure and API for Reliable and Flexible Blackbox Optimization (Song 2023)](https://arxiv.org/pdf/2207.13676)
	- https://www.marktechpost.com/2023/02/04/google-ai-open-sources-vizier-a-standalone-python-package-designed-for-managing-and-optimizing-machine-learning-experiments-at-scale/
- #CODE [Optuna](https://github.com/optuna/optuna) - A hyperparameter optimization framework
	- https://optuna.org/
- #CODE [Yellowbrick](http://www.scikit-yb.org/en/latest/) - Visual analysis and diagnostic tools to facilitate machine learning model selection
- #CODE [Tune-sklearn](https://github.com/ray-project/tune-sklearn) - Drop-in replacement for Scikit-Learn’s model selection module (GridSearchCV, RandomizedSearchCV) with cutting edge hyperparameter tuning techniques
- #CODE [Talos](https://autonomio.github.io/docs_talos/#introduction) - Hyperparameter Optimization for TensorFlow, Keras and PyTorch
- #CODE [Hyperopt](http://hyperopt.github.io/hyperopt) - Distributed Asynchronous Hyperparameter Optimization in Python
	- [Hyperparameter optimization for neural networks](https://github.com/hyperopt/hyperopt-nnet)
	- [Hyperopt-sklearn](http://hyperopt.github.io/hyperopt-sklearn/)
	- #CODE [Hyperas- Keras + Hyperopt: A very simple wrapper for convenient hyperparameter optimization](https://github.com/maxpumperla/hyperas)
		- http://maxpumperla.github.io/hyperas/
- #CODE [Hyperband](https://github.com/zygmuntz/hyperband) - A Novel Bandit-Based Approach to Hyperparameter Optimization
	- #PAPER https://arxiv.org/abs/1603.06560
	- http://fastml.com/tuning-hyperparams-fast-with-hyperband/


  
  
