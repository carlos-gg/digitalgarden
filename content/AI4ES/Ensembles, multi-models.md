---
title: "Ensembles, multi-models"
---

>  See:
>  - [[Weather forecasting, nowcasting]] 
>  - [[S2S]]
>  - [[S2D]]

## Resources
- Improving predictions of Ensembles and averaging. Reducing uncertainty on future predictions
- No one model predicts best all the time, for all variables 
   - Best predictor: Average predictions over all models: http://www.cmap.polytechnique.fr/~zoltan.szabo/ml_external_seminar_EcoleP/2018_04_10_Claire_Monteleoni_slides.pdf 
	   - Average prediction weights all models equally 
	   - Weighted average prediction gives varying weights to each models based on past performances
	   - Adaptive weighted average prediction identifies current best predicting model vs one that quickly switching to other models 
	- Online Learning: Non stationary data. Learns the switching rate: level of non-stationarity 
   - Multi-model assessment of seasonal T and precipitation forecasts over Europe 
- Ensemble Verification Metrics: https://www.ecmwf.int/sites/default/files/elibrary/2017/17626-ensemble-verification-metrics.pdf
- IPCC Expert Meeting on Assessing and Combining Multi Model Climate Projections — IPCC : https://www.ipcc.ch/publication/ipcc-expert-meeting-on-assessing-and-combining-multi-model-climate-projections/

## Talks
- #TALK Statistical post-processing of ensemble weather forecasts: Current developments and future directions (Tilmann Gneiting): https://confluence.ecmwf.int/display/OPTR/Our+training+resources?preview=/35751136/45942083/Screen%20Shot%202015-02-15%20at%2019.38.24.png
- #TALK Multi-model ensemble predictions on seasonal timescale: https://confluence.ecmwf.int/display/OPTR/Our+training+resources?preview=/35751136/36012483/stockdale.png

## Courses
- #COURSE Ensemble forecasting: sources of forecast uncertainty (ECMWF): https://www.ecmwf.int/en/elibrary/18119-ensemble-forecasting-sources-forecast-uncertainty

## References
- #PAPER Decomposition of the Continuous Ranked Probability Score for Ensemble Prediction Systems (Hersbach 2000): https://journals.ametsoc.org/view/journals/wefo/15/5/1520-0434_2000_015_0559_dotcrp_2_0_co_2.xml
	- The CRPS can be seen as a ranked probability score with an infinite number of classes, each of zero width
	- Alternatively, it can be interpreted as the integral of the Brier score over all possible threshold values for the parameter under consideration 
	- For a deterministic forecast system the CRPS reduces to the mean absolute error
	- CRPS can be decomposed into three parts:
		- reliability, is closely related to the rank histogram. The reliability should be zero for an ensemble system with the correct statistical properties. 
		- uncertainty, is the best achievable value of the continuous ranked probability score, in case only climatological information is available.
		- resolution, expresses the superiority of a forecast system with respect to a forecast system based on climatology.
- #PAPER A multiple model assessment of seasonal climate forecast skill for applications (Lavers 2009): https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2009GL041365
- #PAPER Simple and Scalable Predictive Uncertainty Estimation using Deep Ensembles (Lakshminarayanan 2017): https://arxiv.org/abs/1612.01474
- #PAPER Predicting Weather Forecast Uncertainty with [[Machine Learning]] (Scher 2018): https://www.researchgate.net/publication/328264084_Predicting_Weather_Forecast_Uncertainty_with_Machine_Learning
- #PAPER Using multi‐model ensembles of CMIP5 global climate models to reproduce observed monthly rainfall and temperature with machine learning methods in Australia (Wang 2018): https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/joc.5705
	- https://agrivy.oss-cn-zhangjiakou.aliyuncs.com/papers_agrivy/webfiles/papers/2018-IJC-WANG-BIN.pdf
	- The purpose of this study is to compare the capacity of four different multi-model ensemble (MME) methods (random forest, support vector machine, Bayesian model averaging and the arithmetic ensemble mean) in reproducing observed monthly rainfall and temperature
- #PAPER Predicting Weather Uncertainty with Deep [[CNNs]] (Gronquist 2019): https://arxiv.org/abs/1911.00630
	- Ensembles uncertainty estimation with DL
	- WF uncertainty quantification using ensembles prediction system (nonparametrics stats on multiple perturbed simulations)
	- Intensive simulations (dozens and up to 50)
	- Each ensemble member is perturbed, the STDDEV of the embers can be used to identify the uncertainty of a HRes forecast
	- Data: ERA5 (similar to production NWP data) Reanalysis by ECMWF with weather data reanalysis from 1979. 
	- Ensemble of 9 perturbed trajectories and a single unperturbed (control) one. Mapped to 0.5 degree resolution, 37 pressure levels. Temperature prediction. 
	- Subset of IPs that have an influence on Temp: zonal and meridional wind, geopotential, temperature, relative humidity and the factions of cloud cover  
	- Cropping for EU and Atlantic, 40 lat by 136 lon  
	- 7 pressure levels including 500 hPa, 850 hPa  
	- Temporally: 2000 – 2011, between 0600 and 1800 UTC with forecasts made for 3h and 6h into the future  
	- Standardize the data for each pressure level and parameter  
	- Second dataset:  ENS10, re-forecast with 10 perturbed members, 24 h intervals. 2 times per week the last 20 years. Similar to the operational 51-member ensemble, but coarser resolution of 0.5 degrees
	- Model: Weight sharing on each pressure level separately ("full"), more representational power but more parameters 
	- Point-wise affine transforms per pressure level after each convolution ("affine") 2D convs followed by 1D vertical convs ("separable") 
	- Temporal trends (can the temporal progression of the spread be learned?): data of the spread of all 10 trajectories at times 0h, 3h and 6h Tried CLSTMs At the end, treating time sequences as additional channels in U-Net and ResNet Not enough timesteps to learn temporal dynamics 
	- Data parallelism, eventually could use pipeline parallelism for network depth and model parallelism for HiRes data 
	- Evaluation: RMSE as the optimization target, visualization 
	- Comparison with linear regression on the full ensemble spread at time t 0h 
	- Model using only one unperturbed trajectory provides a better spread estimation than using four perturbed trajectories, then 5 ensembles (half of what is available) IPs concatenated to input data 
	- No improvement using temporal models ENS10, model approximates larger ensembles using only a few input trajectories
- #PAPER Ensemble size: How suboptimal is less than infinity? (Leutbecher 2019): https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/qj.3387
- #PAPER Multi-model skill assessment of seasonal temperature and precipitation forecasts over Europe (Mishra 2019): https://link.springer.com/article/10.1007%2Fs00382-018-4404-z
	- https://www.researchgate.net/publication/327349294_Multi-model_skill_assessment_of_seasonal_temperature_and_precipitation_forecasts_over_Europe
	- #BSC, Chloe Prodhomme
	- IMPREX, legacy open data: https://imprex.eu/system/files/generated/files/resource/imprex-opendata-overview.pdf
- See [[Bias correction#^gronquist20]]
- #TALK A new approach to subseasonal multi-model forecasting: Online prediction with expert advice (Brayshaw and Gonzalez 2020): https://meetingorganizer.copernicus.org/EGU2020/EGU2020-17663.html
	- Tested algorithms to perform ‘online prediction with expert advice’ (Cesa-Bianchi et al. 2006). These methods consider a set of weighted ‘experts’ (usually uniformly weighted at the start of the process) to produce subsequent predictions in which the combination or mixture is updated to optimize a loss or skill function
	- S2S4E (https://s2s4e.eu/)
	- The online learning algorithms
		- BOA: Bernstein online aggregation
		- MLpol: Polynomial potential aggregation
	- Compared to the 'exponentiated gradient' method as a reference, which is a sequential learning algorithm previously used in weather and climate -> EGA_NWP
	- The BOA and MLpol methods show skill improvements for leads beyond week 3, a horizon rarely beaten by ECMWF at the country level
- #PAPER Multi-model ensemble predictions of precipitation and temperature using machine learning algorithms (Ahmed 2020): https://www.sciencedirect.com/science/article/pii/S0169809519309858
	- Optimum performance of multi-model ensemble is achieved with 50% of top-ranked GCMs
	- K-Nearest Neighbour and Relevance Vector Machine are good for multi-model ensembles
	- Artificial Neural Network multi-model ensembles showed large performance fluctuations in space
	- Machine learning-based multi-model ensembles outperformed simple ensemble mean
- #PAPER A data-driven multi-model ensemble for deterministic and probabilistic precipitation forecasting at seasonal scale (Xu 2020): https://link.springer.com/article/10.1007/s00382-020-05173-x
	- Current numerical models have large uncertainty in model structure, parameterization and initial conditions
	- A data-driven multi-model ensemble is constructed using a series of statistical and machine learning methods with varying inputs
	- Deterministic precipitation forecasts are produced by the weighting of ensemble members using Bayesian model averaging (BMA) and probabilistic forecasts are generated by sampling from BMA predictive probability density function (PDF)
	- The results demonstrate that the accuracy in the statistical ensemble is significantly higher than the North American multi-model ensemble (NMME) for both deterministic and probabilistic precipitation forecasts, especially at 1-month lead
- #PAPER How to create an operational multi-model of seasonal forecasts? (Hemri 2020): https://link.springer.com/article/10.1007/s00382-020-05314-2
	- #BSC Paco Doblas-Reyes