---
title: "Data assimilation"
---

## Courses
- #COURSE ECMWF An introduction to data assimilation: https://www.ecmwf.int/assets/elearning/da/da1/story_html5.html
- #COURSE ECMWF Training course: Data assimilation: https://events.ecmwf.int/event/153/contributions/
- #TALK Ensemble Data Assimilation: https://confluence.ecmwf.int/display/OPTR/Our+training+resources?preview=/35751136/36012464/EDA.png

## References
- #PAPER A review of operational methods of variational and ensemble‐variational data assimilation (Bannister 2016): https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.2982
- #PAPER [Learning earth system models from observations: machine learning or data assimilation? (Geer 2020)](https://www.ecmwf.int/en/elibrary/19525-learning-earth-system-models-observations-machine-learning-or-data-assimilation)
- #PAPER [Towards an unbiased stratospheric analysis (Laloyaux 2020)](https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/qj.3798)
	- Weak-constraint 4D-Var: https://www.ecmwf.int/en/newsletter/163/meteorology/improving-handling-model-bias-data-assimilation
- #PAPER [Attention-based Convolutional Autoencoders for 3D-Variational Data Assimilation (Mack 2020)](https://www.sciencedirect.com/science/article/pii/S004578252030476X) ^81c123
	- Proposed a new ‘Bi-Reduced Space’ approach to solving 3D Variational Data Assimilation.
	- Used Convolutional Autoencoders to create the reduced space for solving 3D Var
	- Proved that our approach has the same solution as previous methods for reducing 3D Var space
	- Lower computational complexity of previous methods
	- Tested the new method with data from a real-world application: a pollution model in London
- #PAPER [Deep Data Assimilation: Integrating Deep Learning with Data Assimilation (Arcucci 2021)](https://www.mdpi.com/2076-3417/11/3/1114)
- #PAPER [Towards physics-inspired data-driven weather forecasting: integrating data assimilation with a deep spatial-transformer-based U-NET in a case study with ERA5 (Chattopadhyay 2022)](https://gmd.copernicus.org/articles/15/2221/2022/)


### ECMWF-ESA Workshop on ML for Earth System Observation and Prediction (2020)
- #POSTER [A Neural Network-Based Observation Operator for Coupled Ocean-Acoustic Variational Data Assimilation](https://ecmwfevents.com/i/2b97c2c6-d313-4e63-bcce-440cf1ea4746/posters/d8a72240-382e-4857-a66c-a3d430092e0c)
- #POSTER [DAN - An optimal Data Assimilation framework based on machine learning recurrent Networks](https://ecmwfevents.com/i/2b97c2c6-d313-4e63-bcce-440cf1ea4746/posters/d692728d-d047-4f0c-b05b-c5c87cfcf602)
- #POSTER [Toward an integrated NWP-DA-AI system for precipitation prediction](https://ecmwfevents.com/i/2b97c2c6-d313-4e63-bcce-440cf1ea4746/posters/fef6393a-a97f-42c9-ac2d-3649c8c0dfc6)
	- Phased-Array Weather Radar (PAWR) scans the whole sky in the 60-km range every 30 seconds at 110 elevation angles
	- 3D extension of the Convolutional Long Short-Term Memory (Conv-LSTM; Shi et al., 2015) is applied to PAWR nowcasting
	- In addition to the Conv-LSTM with past observations, we also develop a Conv-LSTM that accepts forecast data
- #POSTER  Using machine learning to correct model error and application to data assimilation with a quasi-geostrophic model: https://ecmwfevents.com/i/2b97c2c6-d313-4e63-bcce-440cf1ea4746/posters/39c445b7-cfc8-4bf7-aec2-0de39999f102
- #TALK [Data Assimilation and Machine Learning Science at ECMWF (Bonavita)](https://ecmwfevents.com/i/2b97c2c6-d313-4e63-bcce-440cf1ea4746/oral-presentations/c0d620fc-8923-480c-94f3-0be38c871553)
- #TALK [Artificial Neural Network at the service of Data Assimilation (and vice versa) (Arcucci)](https://ecmwfevents.com/i/2b97c2c6-d313-4e63-bcce-440cf1ea4746/oral-presentations/234cff11-da9b-485f-82e3-daf106739905)
	- [[Data assimilation#^81c123]]
	- #POSTER ICLR - Urban air pollution forecasts generated from latent space representation: https://openreview.net/forum?id=VY1hqB5Z7V#1d2023
	- Combination of simulation (process driven) data and observations (data-driven)
	- The Ensemble Kalman filter, at least 1000 members to better capture underlying PDF
	- DA methods assume linearity, ML could capture non-linearities (LSTMs)
	- Computational fluid dynamics software could be replaced by ML
- #PAPER [Combining data assimilation and machine learning to estimate parameters of a convective-scale model (Legler 2021)](https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.4235?af=R)
