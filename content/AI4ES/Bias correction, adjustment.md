---
title: "Bias correction, adjustment"
---

> See: 
> - [[AI4ES/Statistical downscaling]]
> - [[AI4ES/S2S]], [[AI4ES/S2D]]
> - [[AI4ES/Ensembles, multi-models]]

## Resources
- [Seasonal forecast calibration](https://www.metoffice.gov.uk/research/climate/seasonal-to-decadal/gpc-outlooks/user-guide/calibration)


## Courses
- #COURSE [Statistical post-processing of ensemble weather forecasts: Current developments and future directions (Tilmann Gneiting)](https://confluence.ecmwf.int/download/attachments/45754015/TK_StatisticalPostrocessing_2015.mp4?version=1&modificationDate=1424535945271&api=v2)


## References
- #PAPER [#BSC Use of bias correction techniques to improve seasonal forecasts for reservoirs - A case-study in northwestern Mediterranean (Marcos 2018)](https://pubmed.ncbi.nlm.nih.gov/28803203/)
- #PAPER [Neural networks for post-processing ensemble weather forecasts (Rasp 2018)](https://journals.ametsoc.org/view/journals/mwre/146/11/mwr-d-18-0187.1.xml)
	- Extend to gridded data with CNNs?
- #PAPER [Bias adjustment and ensemble recalibration methods for seasonal forecasting: a comprehensive intercomparison using the C3S dataset (Manzanas 2019)](https://link.springer.com/article/10.1007%2Fs00382-019-04640-4 )
	- https://core.ac.uk/download/pdf/326021617.pdf
- #PAPER [Machine learning for observation bias correction with application to dust storm data assimilation (Jin 2019)](https://acp.copernicus.org/articles/19/10009/2019/)
- #PAPER [Calibration of ECMWF seasonal SEAS5 models monthly temperature re-forecasts over the southeast Asia region (Yun 2020)](https://www.researchgate.net/publication/338335009)
- #PAPER [Comparative Assessment of Various Machine Learning‐Based Bias Correction Methods for Numerical Weather Prediction Model Forecasts of Extreme Air Temperatures in Urban Areas (Cho 2020)](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2019EA000740)
- #TALK [Downscaling and bias correction of seasonal forecasts to support climate services for the Alpine regions (Crespi 2020)](https://meetingorganizer.copernicus.org/EGU2020/EGU2020-10109.html)
- #PAPER [Deep learning for Post-Processing Ensemble Weather Forecasts (Gronquist, 2020)](https://arxiv.org/abs/2005.08748 ) ^gronquist20
   - https://royalsocietypublishing.org/doi/abs/10.1098/rsta.2020.0092?af=R
   - #CODE https://github.com/spcl/deep-weather
   - #TALK https://www.youtube.com/watch?v=5REg7_UtJcs
   - Bias correction with [[AI/Deep learning/DL]] 
   - Simulations are started from GT (from data assimilation)
   - Then get statistics of the ensemble. This is very costly. Can we learn mu and sigma from smaller ensembles?
   - ENS10 and ERA5, selected variables
   - Bias correction input (ERA5) model
   - Uncertainty quantification (ENS10)
   - ResNet, 3D UNET with added locally-connected network (LCN) as the last layer
   - SSIM as training loss
   - CRPS loss function
   - Extreme events too
- #PAPER [A new bias-correction method for precipitation over complex terrain suitable for different climate states: a case study using WRF (Velasquez 2020)](https://gmd.copernicus.org/articles/13/5007/2020/)
- #PAPER [Deep learning for bias correction of MJO prediction (Kim 2021)](https://www.nature.com/articles/s41467-021-23406-3)
	- #CODE https://github.com/HyemiKim77/DLcorrection_MJO


### MOS
- [Model Output Statistics](https://en.wikipedia.org/wiki/Model_output_statistics)
	- MOS is a multiple linear regression technique in which predictands, often near-surface quantities, such as 2-meter (AGL) air temperature, horizontal visibility, and wind direction, speed and gusts, are related statistically to one or more predictors

- #PAPER [Deep Learning for Climate Model Output Statistics (Steininger 2020)](https://www.climatechange.ai/papers/neurips2020/7)
	- https://meetingorganizer.copernicus.org/EGU21/EGU21-2175.html
- #PAPER [[Ensembles, multi-models#^gronquist20]]
- #PAPER [A Model Output Deep Learning Method for Grid Temperature Forecasts in Tianjin Area (Chen 2020)](https://www.mdpi.com/2076-3417/10/17/5808/htm)
	- This paper proposes a model output deep learning (MODL) method for post-processing
	- Samples are multi-variable and spatio-temporal (53 time steps as leadtime)
	- The core of the MODL is 3D Fully Convolutional Neural Networks (3D FCNN)
	- The 3D FCNN or MODL-PLAIN is composed of three convolutional layers. Compared with a UNET-style CNN architecture
	- Each CNN block has CON3d -> activation -> BatchNorm
	- Two DL models, one with 3 CNN layers, one with a UNET-like structure
	- MSE loss function
	- MODL method is better than the univariate linear MOS method, the MOML method based random forest, and linear regression with a running period, and it has the ability to improve grid temperature forecast results in Tianjin area
	- Weather (few days) forecasting
- #PAPER [Adjusting spatial dependence of climate model outputs with Cycle-Consistent Adversarial Networks (Francois 2021)](https://www.researchsquare.com/article/rs-299929/v1)
	- #CODE https://github.com/bastien-francois/MBC_CycleGAN
	- multivariate bias correction (MBC) method
	- adapted  a computer vision technique used for Image-to-Image translation tasks (CycleGAN) for the adjustment of spatial dependence structures of climate model projections
	- the method is applied to adjust maps of temperature and precipitation from climate simulations through two cross-validation approaches
	- The first one is designed to assess two different post-processing schemes (Perfect Prognosis and Model Output Statistics)
	- The second one assesses the influence of nonstationary properties of climate simulations on the performance of MBC-CycleGAN to adjust spatial dependences
	- For the performance assessment of the CycleGAN model during training, the energy distance is used
	- This metric, already used in the bias correction literature permits to measure the statistical discrepancy between two multivariate distributions that are potentially in high dimension
- #PAPER [On the use of convolutional Gaussian processes to improve the seasonal forecasting of precipitation and temperature (Wang 2021)](https://www.sciencedirect.com/science/article/abs/pii/S0022169420313238?dgcid=rss_sd_all)
- #PAPER [Correcting Coarse-Grid Weather and Climate Models by Machine Learning From Global Storm-Resolving Simulations (Bretherton 2022)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021MS002794)