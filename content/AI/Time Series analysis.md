---
title: "Time series analysis"
---

> See: 
> - [[AI/Supervised Learning/Regression]]
> - [[AI/Forecasting]]
> - [[AI/Deep learning/RNNs]]
> - [[AI/Deep learning/CNNs#Sequence (time series) modelling]]
> - [[AI/Deep learning/DL#DL for tabular data]]
> - [[AI/Deep learning/Transformers]]
> - [[AI/Causality/Causality]]

## Resources
- https://en.wikipedia.org/wiki/Time_series
- https://github.com/MaxBenChrist/awesome_time_series_in_python
- https://github.com/frutik/awesome-timeseries
- https://github.com/cuge1995/awesome-time-series
- http://machinelearningmastery.com/convert-time-series-supervised-learning-problem-python/
- [Python to work with time series data](https://github.com/MaxBenChrist/awesome_time_series_in_python)

## Code
- See "Code" in [[AI/Forecasting]]
- #PAPER [A systematic review of Python packages for time series analysis (Siebert 2021)](https://arxiv.org/pdf/2104.07406)            
- #CODE [tsai](https://github.com/timeseriesAI/tsai) - State-of-the-art Deep Learning library for Time Series and Sequences
	- https://timeseriesai.github.io/tsai/
- #CODE [Sktime](https://github.com/alan-turing-institute/sktime)
	- https://towardsdatascience.com/sktime-a-unified-python-library-for-time-series-machine-learning-3c103c139a55
- #CODE [Stumpy](https://github.com/TDAmeritrade/stumpy) - STUMPY is a powerful and scalable Python library for modern time series analysis
- #CODE [Orbit](https://github.com/uber/orbit) - A Python package for Bayesian forecasting with object-oriented design and probabilistic models under the hood
	- https://eng.uber.com/the-new-version-of-orbit-v1-1-is-released/
- #CODE [TSflex](https://github.com/predict-idlab/tsflex)
	- https://predict-idlab.github.io/tsflex/
- #CODE [Merlion](https://github.com/salesforce/merlion) - Merlion is a Python library for time series intelligence
	- #PAPER [Merlion: A Machine Learning Library for Time Series (Bhatnagar 2021)](https://arxiv.org/abs/2109.09265)
- #CODE [Kats](https://github.com/facebookresearch/Kats) 
	- Kats, a kit to analyze time series data, a lightweight, easy-to-use, generalizable, and extendable framework to perform time series analysis, from understanding the key statistics and characteristics, detecting change points and anomalies, to forecasting future trends
	- https://facebookresearch.github.io/Kats/
	- https://engineering.fb.com/2021/06/21/open-source/kats/
	- https://towardsdatascience.com/kats-a-generalizable-framework-to-analyze-time-series-data-in-python-3c8d21efe057
- #CODE [Tsfresh](https://github.com/blue-yonder/tsfresh) - Time Series Feature extraction based on scalable hypothesis tests
	- [Automatic extraction of relevant features from time series](http://tsfresh.readthedocs.io)
- #CODE [TSFEL](https://github.com/fraunhoferportugal/tsfel)
	- #PAPER [TSFEL: Time Series Feature Extraction Library (Barandas 2020)](https://www.sciencedirect.com/science/article/pii/S2352711020300017)
- #CODE [Tslearn](https://github.com/rtavenar/tslearn) - A machine learning toolkit dedicated to time-series data
- #CODE [Pmdarima](https://github.com/alkaline-ml/pmdarima)
	- Pyramid bridges one more gap between R and Python by bringing R's auto.arima to Python. Pyramid wraps statsmodels' well-tested ARIMA and SARIMAX estimators.
- #CODE [Tick](https://github.com/X-DataInitiative/tick)
- #CODE [Feature engine](https://feature-engine.readthedocs.io/en/1.3.x/user_guide/timeseries/index.html)
- #CODE [Featuretools](https://github.com/alteryx/featuretools) - An open source python library for automated feature engineering
	- https://www.featuretools.com/

## Subtopics
### Time Series Forecasting
See [[AI/Forecasting]]

### Anomaly and Outlier Detection
See [[AI/Anomaly and Outlier Detection#For Time series]]

### TS models
- [Autoregressive](https://en.wikipedia.org/wiki/Autoregressive)
- [Moving average](https://en.wikipedia.org/wiki/Moving_average_model)
- [Autoregressive moving average (ARMA)](https://en.wikipedia.org/wiki/Autoregressive_moving_average)
- [Autoregressive integrated moving average (ARIMA)](https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average)
- [Generalized additive model (GAM)](https://en.wikipedia.org/wiki/Generalized_additive_model)
	- http://www.kdnuggets.com/2017/04/time-series-analysis-generalized-additive-models.html
- #PAPER [HyperTime: Implicit Neural Representation for Time Series (Fons 2022)](https://arxiv.org/pdf/2208.05836)

### TS classification
- [UEA & UCR Time Series Classification Repository](http://www.timeseriesclassification.com/)
	- [Datasets](http://www.timeseriesclassification.com/dataset.php)
- [Dynamic time warping](https://en.wikipedia.org/wiki/Dynamic_time_warping) - DTW is one of the algorithms for measuring similarity between two temporal sequences, which may vary in speed
- https://medium.com/@hassanismailfawaz/deep-learning-for-time-series-classification-a-brief-overview-73b58767ed0f
- #PAPER [ROCKET: Exceptionally fast and accurate time series classification using random convolutional kernels (Dempster 2019)](https://arxiv.org/abs/1910.13051)
- #PAPER [InceptionTime: Finding AlexNet for Time Series Classification (Ismail Fawaz 2019)](https://arxiv.org/abs/1909.04939)
- #PAPER [Deep learning for time series classification: a review (Ismail Fawaz 2019)](https://arxiv.org/abs/1809.04356)
	- #CODE https://github.com/hfawaz/dl-4-tsc
	- https://medium.com/@hassanismailfawaz/deep-learning-for-time-series-classification-a-brief-overview-73b58767ed0f
- #PAPER [TS-CHIEF: A Scalable and Accurate Forest Algorithm for Time Series Classification (Shifaz 2020)](https://arxiv.org/abs/1906.10329)

### Time-frequency analysis
- [Continuous wavelet transform](https://en.wikipedia.org/wiki/Continuous_wavelet_transform)

#### Fourier Analysis
- [Fourier analysis](https://en.wikipedia.org/wiki/Fourier_analysis)
	- [Fast Fourier transform](https://en.wikipedia.org/wiki/Fast_Fourier_transform)
		- A fast Fourier transform (FFT) is an algorithm that computes the discrete Fourier transform (DFT) of a sequence, or its inverse (IDFT).
	- [Fourier Transform for Time Series](https://towardsdatascience.com/fourier-transform-for-time-series-292eb887b101)
	- [Understanding FFTs and Windowing](https://download.ni.com/evaluation/pxi/Understanding%20FFTs%20and%20Windowing.pdf)

### Causality
See [[AI/Causality/Causality]]

### Explainability
See [[AI/XAI]]
  
