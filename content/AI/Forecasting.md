---
title: "Forecasting"
disableToc: false 
---

See: 
[[Time Series analysis]]
[[Regression]]
[[RNNs]]
[[CNNs#Sequence time series modelling]]
[[Transformers#For NLP]]

- https://en.wikipedia.org/wiki/Forecasting
- Microsoft - Time Series Forecasting Best Practices & Examples: https://github.com/microsoft/forecasting
- Forecasting with a Time Series Model using Python: 
	- https://www.bounteous.com/insights/2020/09/15/forecasting-time-series-model-using-python-part-one/
	- https://www.bounteous.com/insights/2020/09/15/forecasting-time-series-model-using-python-part-two/
- https://towardsdatascience.com/the-complete-guide-to-time-series-analysis-and-forecasting-70d476bfe775
- https://towardsdatascience.com/automl-for-time-series-advanced-approaches-with-fedot-framework-4f9d8ea3382c

## Code
- #CODE Darts: https://github.com/unit8co/darts
	- https://unit8co.github.io/darts/
	- Python library for easy manipulation and forecasting of time series. It contains a variety of models, from classics such as ARIMA, Prophet,  deep neural networks (NBEATS, RNNs, Transformers)
	- https://towardsdatascience.com/darts-swiss-knife-for-time-series-forecasting-in-python-f37bb74c126
- #CODE Prophet (Facebook): https://github.com/facebook/prophet
	- https://facebook.github.io/prophet/
	- Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data.
	- https://research.fb.com/prophet-forecasting-at-scale/
	- http://blog.fastforwardlabs.com/2017/03/22/prophet.html	
	- See [[Time Series analysis#^kats]]
- #CODE NeuralProphet: https://github.com/ourownstory/neural_prophet
	- https://ourownstory.github.io/neural_prophet/
	- A simple forecasting model based on Neural Networks in PyTorch
- #CODE Hcrystalball: https://github.com/heidelbergcement/hcrystalball
	- Library that unifies the API for most commonly used libraries and modeling techniques for time-series forecasting in Python
- #CODE AtsPy: Automated Time Series Forecasting in Python: https://github.com/firmai/atspy
- #CODE Greykite (Linkedin): https://github.com/linkedin/greykite
	- https://linkedin.github.io/greykite/
	- A flexible, intuitive and fast forecasting library
- #CODE Scalecast: https://github.com/mikekeith52/scalecast
	- https://towardsdatascience.com/introducing-scalecast-a-forecasting-library-pt-1-33b556d9b019

## Books
- #BOOK Forescasting: principles and practice (Hyndman 2018, R): https://otexts.com/fpp2/


## References
- #PAPER Time Series Forecasting With Deep Learning: A Survey (Lim 2020): https://arxiv.org/abs/2004.13408
- #PAPER A flexible forecasting model for production systems (Hosseini 2021): https://arxiv.org/abs/2105.01098
- #PAPER An Experimental Review on Deep Learning Architectures for Time Series Forecasting (Lara-Benitez 2021): https://arxiv.org/abs/2103.12057