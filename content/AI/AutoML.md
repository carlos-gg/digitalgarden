---
title: "AutoML"
disableToc: false 
---

See [Model selection and tuning](Model%20selection%20and%20tuning.md)

## Resources
- https://en.wikipedia.org/wiki/Automated_machine_learning
- Automated machine learning (AutoML) is the process of automating the process of applying machine learning to real-world problems. AutoML covers the complete pipeline from the raw dataset to the deployable machine learning model. AutoML was proposed as an artificial intelligence-based solution to the ever-growing challenge of applying machine learning.
- Automated machine learning can target various stages of the machine learning process. Steps to automate are:
	- Data preparation and ingestion (from raw data and miscellaneous formats)
		- Column type detection; e.g., boolean, discrete numerical, continuous numerical, or text
		- Column intent detection; e.g., target/label, stratification field, numerical feature, categorical text feature, or free text feature
		- Task detection; e.g., binary classification, regression, clustering, or ranking
	- Feature engineering
		- Feature selection
		- Feature extraction
		- Meta learning and transfer learning
		- Detection and handling of skewed data and/or missing values
	- Model selection. See [Model selection and tuning](Model%20selection%20and%20tuning.md)
	- Hyperparameter optimization of the learning algorithm and featurization
	- Pipeline selection under time, memory, and complexity constraints
	- Selection of evaluation metrics and validation procedures
	- Problem checking
		- Leakage detection
		- Misconfiguration detection
	- Analysis of results obtained
	- User interfaces and visualizations for automated machine learning
- https://www.automl.org/
- http://www.kdnuggets.com/2017/01/current-state-automated-machine-learning.html
- https://medium.com/airbnb-engineering/automated-machine-learning-a-paradigm-shift-that-accelerates-data-scientist-productivity-airbnb-f1f8a10d61f8


## Books
-  #BOOK AutoML: Methods, systems, challenges: https://www.automl.org/book/


## Code
- #CODE FLAML - Fast and Lightweight AutoML: https://github.com/microsoft/FLAML
	- FLAML is powered by a new, cost-effective hyperparameter optimization and learner selection method invented by Microsoft Research
- #CODE EvalML - AutoML library written in python: https://github.com/alteryx/evalml
	- https://innovation.alteryx.com/introducing-evalml/
- #CODE Model Search: https://github.com/google/model_search
	- https://ai.googleblog.com/2021/02/introducing-model-search-open-source.html
- #CODE Auto-sklearn: https://github.com/automl/auto-sklearn
	- http://automl.github.io/auto-sklearn/stable/
	- Efficient and Robust Automated Machine Learning (Feurer 2015): https://ml.informatik.uni-freiburg.de/papers/15-NIPS-auto-sklearn-preprint.pdf
	- http://www.kdnuggets.com/2016/08/winning-automl-challenge-auto-sklearn.html
- #CODE TPOT: https://github.com/rhiever/tpot
	- http://rhiever.github.io/tpot/
	- Consider TPOT yourData Science Assistant. TPOT is a Python tool that automatically creates and optimizes ML pipelines using genetic programming
	- https://blog.alookanalytics.com/2017/05/25/automate-your-machine-learning/
- #CODE AutoKeras: https://github.com/keras-team/autokeras
- #CODE H2O autoML: https://blog.h2o.ai/2017/06/automatic-machine-learning/
- #CODE Adanet - Fast and flexible AutoML with learning guarantees: https://github.com/tensorflow/adanet 
	- https://adanet.readthedocs.io
	- AdaNet is a lightweight TensorFlow-based framework for automatically learning high-quality models with minimal expert intervention
- #CODE FEDOT: https://github.com/nccr-itmo/FEDOT
	- Automated modeling and machine learning framework
	- https://fedot.readthedocs.io/en/latest/


## Neural architecture search (NAS)
- NAS is closely related to hyperparameter optimization and is a subfield of automated machine learning (AutoML).
- https://en.wikipedia.org/wiki/Neural_architecture_search
	- Neural architecture search (NAS) is a technique for automating the design of artificial neural networks (ANN), a widely used model in the field of machine learning. NAS has been used to design networks that are on par or outperform hand-designed architectures. Methods for NAS can be categorized according to the search space, search strategy and performance estimation strategy used:
	- The search space defines the type(s) of ANN that can be designed and optimized.
	- The search strategy defines the approach used to explore the search space.
	- The performance estimation strategy evaluates the performance of a possible ANN from its design (without constructing and training it).

- Literature on NAS: https://www.automl.org/automl/literature-on-neural-architecture-search/
- #PAPER AdaNet: Adaptive Structural Learning of Artificial Neural Networks (Cortes 2017): http://proceedings.mlr.press/v70/cortes17a.html
	- https://ai.googleblog.com/2018/10/introducing-adanet-fast-and-flexible.html?m=1
- #PAPER Improving Neural Architecture Search Image Classifiers via Ensemble Learning, AdaNas (Macko 2019): https://arxiv.org/abs/1903.06236
- #PAPER Up to two billion times acceleration of scientific simulations with deep neural architecture search (Kasim 2020): https://arxiv.org/abs/2001.08055
- #PAPER Neural Architecture Search without Training (Mellor 2020): https://arxiv.org/abs/2006.04647
	- Paper explained: https://www.youtube.com/watch?v=a6v92P0EbJc
- #PAPER Automated Evolutionary Approach for the Design of Composite Machine Learning Pipelines (Nikitin 2021): https://arxiv.org/abs/2106.15397


