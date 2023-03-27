---
title: "Forecasting"
---

> See: 
> - [[AI/Time Series analysis]]
> - [[AI/Supervised Learning/Regression]]
> - [[AI/Deep learning/RNNs]]
> - "Sequence time series modelling" section in [[AI/Deep learning/CNNs]]
> - "For NLP" section in [[AI/Deep learning/Transformers]]

## Resources
- https://en.wikipedia.org/wiki/Forecasting
- [Microsoft - Time Series Forecasting Best Practices & Examples](https://github.com/microsoft/forecasting)
- Forecasting with a Time Series Model using Python: 
	- https://www.bounteous.com/insights/2020/09/15/forecasting-time-series-model-using-python-part-one/
	- https://www.bounteous.com/insights/2020/09/15/forecasting-time-series-model-using-python-part-two/
- https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775
- https://towardsdatascience.com/automl-for-time-series-advanced-approaches-with-fedot-framework-4f9d8ea3382c
- [Predicting energy demand with neural networks](https://towardsdatascience.com/forecasting-energy-consumption-using-neural-networks-xgboost-2032b6e6f7e2)
- Time series forecasting:
	- [Part 1 of 3: Understanding the fundamentals](https://medium.com/data-science-at-microsoft/time-series-forecasting-part-1-of-3-understanding-the-fundamentals-13b52eda3e5)
	- [Part 2 of 3: Selecting algorithms](https://medium.com/data-science-at-microsoft/time-series-forecasting-part-2-of-3-selecting-algorithms-11b6635f61bb)
	- [Part 3 of 3: Introducing AUTS (Adaptive Univariate Time Series forecasting algorithm)](https://medium.com/data-science-at-microsoft/time-series-forecasting-part-3-of-3-introducing-auts-adaptive-univariate-time-series-dfd7555ca8d4)
- [Python Time Series Forecasting: A Practical Approach (WANDB)](https://wandb.ai/madhana/Time_Series/reports/Python-Time-Series-Forecasting-A-Practical-Approach--VmlldzoyODk4NjUz)
- [The Reasonable Effectiveness of Deep Learning for Time Series Forecasting](https://towardsdatascience.com/the-reasonable-effectiveness-of-deep-learning-for-time-series-forecasting-60e2c8affb9)

## Code
- #CODE [Skforecast](https://github.com/JoaquinAmatRodrigo/skforecast)
	- https://joaquinamatrodrigo.github.io/skforecast/
	- Package towards building Explainable Forecasting and Nowcasting Models with State-of-the-art Deep Neural Networks and Dynamic Factor Model on Time Series data sets with single line of code
	- https://www.kdnuggets.com/2021/12/sota-explainable-forecasting-and-nowcasting.html
	- [Skforecast: time series forecasting with Python and Scikit-learn](https://www.cienciadedatos.net/documentos/py27-time-series-forecasting-python-scikitlearn.html)
- #CODE [Pytorch-forecasting](https://github.com/jdb78/pytorch-forecasting) - Time series forecasting with PyTorch
	- https://pytorch-forecasting.readthedocs.io/en/stable/index.html#
- #CODE [Deep_XF](https://github.com/ajayarunachalam/Deep_XF)
- #CODE [statsforecast](https://github.com/Nixtla/statsforecast)
	- StatsForecast offers a collection of widely used univariate time series forecasting models, including autoARIMA and ETS modeling optimized for high performance using numba
	- https://nixtla.github.io/statsforecast/
- #CODE [Darts](https://github.com/unit8co/darts)
	- https://unit8co.github.io/darts/
	- Python library for easy manipulation and forecasting of time series. It contains a variety of models, from classics such as ARIMA, Prophet,  deep neural networks (NBEATS, RNNs, Transformers)
	- https://towardsdatascience.com/darts-swiss-knife-for-time-series-forecasting-in-python-f37bb74c126
- #CODE [Neuralforecast](https://github.com/Nixtla/neuralforecast)
	- NeuralForecast is a Python library for time series forecasting with deep learning models. It includes benchmark datasets, data-loading utilities, evaluation functions, statistical tests, univariate model benchmarks and SOTA models implemented in PyTorch and PyTorchLightning
	- https://nixtla.github.io/neuralforecast
- #CODE [Prophet (Facebook)](https://github.com/facebook/prophet)
	- https://facebook.github.io/prophet/
	- Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data.
	- https://research.fb.com/prophet-forecasting-at-scale/
	- http://blog.fastforwardlabs.com/2017/03/22/prophet.html	
- #CODE [NeuralProphet](https://github.com/ourownstory/neural_prophet)
	- https://ourownstory.github.io/neural_prophet/
	- A simple forecasting model based on Neural Networks in PyTorch
- #CODE [Hcrystalball](https://github.com/heidelbergcement/hcrystalball)
	- Library that unifies the API for most commonly used libraries and modeling techniques for time-series forecasting in Python
- #CODE [AtsPy: Automated Time Series Forecasting in Python](https://github.com/firmai/atspy)
- #CODE [Greykite (Linkedin)](https://github.com/linkedin/greykite)
	- https://linkedin.github.io/greykite/
	- A flexible, intuitive and fast forecasting library
- #CODE [Scalecast](https://github.com/mikekeith52/scalecast)
	- https://towardsdatascience.com/introducing-scalecast-a-forecasting-library-pt-1-33b556d9b019
	
## Talks
- #TALK [Feature Engineering for Time Series Forecasting | PyData London 2022](https://www.youtube.com/watch?v=9QtL7m3YS9I)

## Books
- #BOOK [Forescasting: principles and practice (Hyndman, R)]
- [2nd ed.](https://otexts.com/fpp2/)
- [3rd ed.](https://otexts.com/fpp3/)

## References
- #PAPER [Time Series Forecasting With Deep Learning: A Survey (Lim 2020)](https://arxiv.org/abs/2004.13408)
- #PAPER [N-BEATS: Neural basis expansion analysis for interpretable time series forecasting (Oreshkin 2020)](https://arxiv.org/abs/1905.10437)
- #PAPER [A flexible forecasting model for production systems (Hosseini 2021)](https://arxiv.org/abs/2105.01098)
- #PAPER [An Experimental Review on Deep Learning Architectures for Time Series Forecasting (Lara-Benitez 2021)](https://arxiv.org/abs/2103.12057)
- #PAPER [Temporal Fusion Transformers for interpretable multi-horizon time series forecasting (Lim 2021)](https://www.sciencedirect.com/science/article/pii/S0169207021000637)
	- https://ai.googleblog.com/2021/12/interpretable-deep-learning-for-time.html
	- [[AI/Deep learning/Transformers]]
- #PAPER [Understanding forecast reconciliation (Hollyman 2021)](https://www.sciencedirect.com/science/article/abs/pii/S0377221721000199)
	- Forecast Reconciliation - a process by which independently generated forecasts of a collection of linearly related time series are reconciled via the introduction of accounting aggregations that naturally apply to the data
- #PAPER [A Review on Deep Sequential Models for Forecasting Time Series Data (Mahdi Ahmed 2022)](https://www.hindawi.com/journals/acisc/2022/6596397/)
- #PAPER [DeepTime: Deep Time-Index Meta-Learning for Non-Stationary Time-Series Forecasting (Woo 2022)](https://arxiv.org/pdf/2207.06046)
	- #CODE https://github.com/salesforce/DeepTime
	- DeepTime is a deep time-index based model trained via a meta-learning formulation, yielding a strong method for non-stationary time-series forecasting
	- https://pub.towardsai.net/meta-learning-for-time-series-forecasting-deeptime-in-pytorch-lightning-3d97351099c6
- #PAPER [Forecast evaluation for data scientists: common pitfalls and best practices (Hewamalage 2022)](https://link.springer.com/article/10.1007/s10618-022-00894-5)
- #PAPER #REVIEW [Review of ML and AutoML Solutions to Forecast Time-Series Data (Alsharef 2022)](https://link.springer.com/article/10.1007/s11831-022-09765-0)
