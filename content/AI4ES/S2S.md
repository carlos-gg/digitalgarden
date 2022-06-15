---
title: "S2S"
---

> See:
> - [[S2D]]
> - [[Ensembles, multi-models]]
> - [[AI4ES/AI4ES data#AI4ES data#Seasonal systems]]
> - [[AI4ES/S2S ML-based prediction]]
> - [[AI4S2S project review]]
> - [[AI4ES/AI4ES data#Seasonal forecasts]]

## Resources
- S2Sprediction project: http://s2sprediction.net/
- Challenge to improve Sub-seasonal to Seasonal Predictions using Artificial Intelligence: https://s2s-ai-challenge.github.io/
- The Subseasonal Experiment (SubX): https://cpo.noaa.gov/Meet-the-Divisions/Earth-System-Science-and-Modeling/MAPP/Research-to-Operations-and-Applications/Subseasonal-Experiment
	- Customized Subseasonal Weekly Forecasts: http://wxmaps.org/subx_custom.php
- The Subseasonal Rodeo: https://www.drought.gov/drought/forecast-rodeo-ii-leaderboard 
	- Dataset: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/IHBANG
	- https://www.microsoft.com/en-us/research/blog/predicting-the-holy-grail-of-climate-forecasting-a-new-model-and-a-new-public-dataset/
	- #TALK Machine learning seminar series - Enhancing Western United States Sub-Seasonal Forecasts: Forecast Rodeo Prize Competition Series: https://events.ecmwf.int/event/218/ ^c044aa
- EGU 2020 Session. Subseasonal-to-Seasonal Prediction: meteorology and impacts. https://meetingorganizer.copernicus.org/EGU2020/displays/36782
- Improved three-week weather forecasts could save lives from disaster: https://www.sciencenews.org/article/climate-weather-forecast-three-week-disaster-storms
	- Between short-term and seasonal prediction lies the realm of subseasonal prediction. Making such forecasts is hard because the initial information that drives short-term forecasts is no longer useful, but the longer-term trends that drive seasonal forecasts have not yet become apparent.
	- Short-term weather predictions and longer-term seasonal forecasts are relatively good. People need something in between, so researchers are trying to improve subseasonal forecasts, which look ahead a few weeks, using information from many sources, including predictable weather systems.
	- Part of the challenge stems from the fact that many patterns influence weather on the subseasonal scale — and some of them aren’t predictable. 
	- E.g. MJO: A belt of thunderstorms that typically starts in the Indian Ocean and travels eastward, that happens several times a year. The MJO travels eastward along the equator as winds push warm, wet air high into the atmosphere, where the air dries out, cools and descends back toward the surface.
	- “If you can predict the MJO better, then you can predict the weather better” 
	-  Another weather pattern that might help improve subseasonal forecasts is a quick rise in temperature in the stratosphere, a layer of the upper atmosphere, above the Arctic or Antarctic. These “sudden stratospheric warming” events happen once every couple of years in the Northern Hemisphere and much less often in the Southern Hemisphere. But when one shows up, it affects weather worldwide. 

MJO:
- Check updates in: http://s2sprediction.net/xwiki/bin/view/Phase2/MJOTel
- #PAPER Madden–Julian Oscillation impacts on South American summer monsoon season: precipitation anomalies, extreme events, teleconnections, and role in the MJO cycle (Grimm 2019): https://link.springer.com/article/10.1007/s00382-019-04622-6


## Code
- #CODE xskillscore - Metrics for verifying forecasts: https://github.com/xarray-contrib/xskillscore
	- https://xskillscore.readthedocs.io/en/stable/quick-start.html
- #CODE Climpred - Verification of weather and climate forecasts: https://github.com/pangeo-data/climpred
	- https://climpred.readthedocs.io/en/stable/


## Books
- #BOOK Sub-Seasonal to Seasonal Prediction - The Gap Between Weather and Climate Forecasting: https://www.sciencedirect.com/book/9780128117149/sub-seasonal-to-seasonal-prediction
- #BOOK Statistical Postprocessing of Ensemble Forecasts (2018, ELSEVIER): https://www.elsevier.com/books/statistical-postprocessing-of-ensemble-forecasts/vannitsem/978-0-12-812372-0


## Courses
- #COURSE Seasonal forecasting (ECMWF): https://www.ecmwf.int/en/elibrary/19273-seasonal-forecasting
- #COURSE Using stochastic physics to repesent model uncertainty (ECMWF): https://www.ecmwf.int/en/elibrary/19275-using-stochastic-physics-repesent-model-uncertainty
- #COURSE Ensemble forecasting: sources of forecast uncertainty (Richardson, ECMWF): https://www.ecmwf.int/en/elibrary/18119-ensemble-forecasting-sources-forecast-uncertainty
- #COURSE ECMWF extended range forecasts: https://learning.ecmwf.int/group/guest/lesson-viewer?p_p_id=com_arcusys_valamis_web_portlet_LessonViewerView&p_p_lifecycle=0&p_p_state=maximized&p_p_mode=view&p_p_auth=Jze9AVQe&_com_arcusys_valamis_web_portlet_LessonViewerView_lesson_id=1847
- #COURSE Advanced School and Workshop on Subseasonal to Seasonal (S2S) Prediction and Application to Drought Prediction: 
	- https://www.youtube.com/playlist?list=PLos1JqOLJm3uvpiao2C71Pa-9SpmkrKih
	- Forecast verification: https://www.youtube.com/watch?v=SUu4oIERgRw
	- Sub-Seasonal forecasting,Forecasting system design: https://www.youtube.com/watch?v=L3vKJ1vwpr4&list=PLos1JqOLJm3uvpiao2C71Pa-9SpmkrKih&index=6
	- An introduction to numerical weather prediction and climate model uncertainly: https://www.youtube.com/watch?v=DYPqo16oOts&list=PLos1JqOLJm3uvpiao2C71Pa-9SpmkrKih&index=3


## References
- #PAPER Kullback–Leibler Divergence as a Forecast Skill Score with Classic Reliability–Resolution–Uncertainty Decomposition (Weijs 2010): https://journals.ametsoc.org/view/journals/mwre/138/9/2010mwr3229.1.xml
- #PAPER Winter Precipitation Forecast in the European and Mediterranean Regions Using Cluster Analysis (Totz 2017): https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2017GL075674
- #PAPER Seasonal Drought Prediction: Advances, Challenges, and Future Prospects (Hao 2018): https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2016RG000549 ^seasdroughthao18
- #PAPER S2S reboot: An argument for greater inclusion of machine learning in subseasonal to seasonal forecasts (Cohen, 2019): https://onlinelibrary.wiley.com/doi/full/10.1002/wcc.567
	- The discipline of seasonal climate prediction began as an exercise in simple statistical techniques. Beginning in the 1990s, forecasts from dynamical models of increasing complexity were introduced into the operational production of S2S forecasts while inclusion of statistical techniques was phased out
	- today the large government forecast centers almost exclusively rely on complex fully coupled dynamical forecast systems for their subseasonal to seasonal (S2S) predictions while statistical techniques are mostly neglected and those techniques still in use have not been updated in decades
	- new statistical techniques mostly developed outside the field of climate science, collectively referred to as machine learning, can be adopted by climate forecasters to increase the accuracy of S2S predictions
	- traditional forecast methodologies based on CCA http://rcc.imdpune.gov.in/Training/SASCOF12/CPT_Dayone/PCR_CCA_Nachiketa.pdf
	- novel ones (unsupervised)
		- (hierarchical) clustering : https://onlinelibrary.wiley.com/action/downloadSupplement?doi=10.1002%2Fwcc.567&file=wcc567-sup-0001-AppendixS1.pdf
		- other potential (supervised) ML approaches are outlined in that supplement
		- multilinear regression
	- the lack of attention, resources and implementation of statistical techniques is a mistake and deprives the public of immediate and relatively inexpensive improvements to S2S prediction
	- Statistical predictions in general and machine learning techniques in particular are likely to improve subseasonal climate forecasts where there are repeatable patterns in the atmosphere and where there are fairly consistent sequences of events
- #PAPER Improving Subseasonal Forecasting in the Western U.S. with Machine Learning (Hwang 2019): https://arxiv.org/abs/1809.07394
	- #CODE https://github.com/paulo-o/forecast_rodeo
	- https://www.microsoft.com/en-us/research/project/subseasonal-climate-forecasting/
	- NOAA launched the Subseasonal Climate Forecast Rodeo, a year-long real-time forecasting challenge in which participants aimed to skillfully predict temperature and precipitation in the western U.S. two to four weeks and four to six weeks in advance
	- Subseasonal Climate Forecast Rodeo (2016-2018): https://www.challenge.gov/challenge/sub-seasonal-climate-forecast-rodeo/
	- ML approach (ensemble of two nonlinear regression models) to the Rodeo and release our SubseasonalRodeo dataset, collected to train and evaluate our forecasting system 
- #PAPER El Niño-Southern Oscillation forecasting using complex networks analysis of LSTM neural networks (Broni-Bedaiko 2019): https://www.semanticscholar.org/paper/El-Ni%C3%B1o-Southern-Oscillation-forecasting-using-of-Broni-Bedaiko-Katsriku/3ebe4aa92226fa22100dce93dc385bd93a417fd3
	- El Niño-Southern Oscillation (ENSO) is the most influential climatological phenomenon that has been intensively researched during the past years. 
	- The scientific community knows much about the underlying processes of ENSO phenomenon, however, its predictability for longer horizons, which is very important for human society and the natural environment is still a challenge in the scientific community
- #PAPER Machine learning climate variability (Hwan Park 2019): https://ml4physicalsciences.github.io/2019/files/NeurIPS_ML4PS_2019_84.pdf
	- MLP, LSTM, PCA+LSTM, ConvLSTM
	- The more sophisticated of these network architectures (ConvLSTM) is able to perform skillfully at lead times of up to about a year
- #PAPER Deep learning for multi-year ENSO forecasts (Ham 2019):  https://www.researchgate.net/publication/335896498_Deep_learning_for_multi-year_ENSO_forecasts
	- #CODE https://github.com/jeonghwan723/DL_ENSO/tree/v1.0
	- Slides: https://meso.nju.edu.cn/DFS//file/2019/11/26/201911261121480744epw3l.pdf?iid=6240
	- https://phys.org/news/2019-09-deep-application-el-nio-events.html 
	- Uses a sort of transfer learning (models and reanalysis)
- #PAPER Diagnosing Secular Variations in Retrospective ENSO Seasonal Forecast Skill Using CMIP5 Model‐Analogs (Ding 2019): https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018GL080598
- #PAPER Prediction of North Atlantic Oscillation Index with Convolutional LSTM Based on Ensemble Empirical Mode Decomposition (Yuan 2019): https://www.mdpi.com/2073-4433/10/5/252/htm
	- NAO is the most significant mode of the atmosphere in the North Atlantic, and it plays an important role in regulating the local weather and climate and even those of the entire Northern Hemisphere
	- An effective neural network model EEMD-ConvLSTM (based on ConvLSTM) with Ensemble Empirical Mode Decomposition (EEMD), is proposed for NAO index prediction
	- EEMD is applied to preprocess NAO index data, which are issued by the NOAA and NAO index data are decomposed into several Intrinsic Mode Functions (IMFs)
- #PAPER The Application of Machine Learning Techniques to Improve El Niño Prediction Skill (Dijkstra 2019): https://www.frontiersin.org/articles/10.3389/fphy.2019.00153/full
- #PAPER Sub-Seasonal Climate Forecasting via Machine Learning: Challenges, Analysis, and Advances (He, 2020): https://arxiv.org/abs/2006.07972
	- Sub-seasonal climate forecasting (SSF) focuses on predicting key climate variables such as temperature and precipitation in the 2-week to 2-month time scales
	- immense societal value, in areas such as agricultural productivity, water resource management, transportation and aviation systems, and emergency planning for extreme weather events
	- In this paper, we carefully study a variety of machine learning (ML) approaches for SSF over the US mainland
	- Among a broad suite of 10 ML approaches considered, gradient boosting performs the best, and deep learning (DL) methods show some promise with careful architecture choices
	- DL models explored: Encoder (LSTM)-Decoder (FNN), CNN-LSTM
	- Empirical results show the gradient boosting model XGBoost, the DL model Encoder (LSTM)-Decoder (FNN), and linear models, such as Lasso, consistently outperform state-of-the-art forecasts. XGBoost has the highest skill over all models, and demonstrates its predictive power
- #PAPER Choices in the Verification of S2S Forecasts and Their Implications for Climate Services (Manrique-Sunen 2020): https://journals.ametsoc.org/mwr/article/148/10/3995/353477/Choices-in-the-Verification-of-S2S-Forecasts-and
- #PAPER The influence of aggregation and statistical post‐processing on the subseasonal predictability of European temperatures (van Straaten 2020): https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.3810
- #PAPER North Atlantic climate far more predictable than models imply (Smith 2020): https://www.nature.com/articles/s41586-020-2525-0
- #PAPER The Importance of Past MJO Activity in Determining the Future State of the Midlatitude Circulation (Tseng 2020): https://journals.ametsoc.org/view/journals/clim/33/6/jcli-d-19-0512.1.xml
- #PAPER Testing the Reliability of Interpretable Neural Networks in Geoscience Using the Madden-Julian Oscillation (Toms, 2020): https://arxiv.org/abs/1902.04621
	- Tested the reliability of two neural network interpretation techniques, backward optimization and layerwise relevance propagation, within geoscientific applications by applying them to a commonly studied geophysical phenomenon, the Madden-Julian Oscillation. 
	- The Madden-Julian Oscillation is a multi-scale pattern within the tropical atmosphere that has been extensively studied over the past decades, which makes it an ideal test case to ensure the interpretability methods can recover the current state of knowledge regarding its spatial structure. 
	- The neural network identifies the phase of the Madden-Julian Oscillation twice as accurately as linear regression, which means that nonlinearities used by the neural network are important to the structure of the Madden-Julian Oscillation
	- used the interpretations to identify the seasonality of the Madden-Julian Oscillation, and find that the conventionally defined extended seasons should be shifted later by one month
	- Deep Learning for Scientific Inference from Geophysical Data: The Madden-Julian Oscillation as a Test Case (Toms, 2020): https://arxiv.org/abs/1902.04621v1
- #PAPER Improving subseasonal precipitation forecasts through a statistical–dynamical approach: application to the southwest tropical Pacific (Specq 2020): https://link.springer.com/article/10.1007/s00382-020-05355-7
- #TALK Predictable weather regimes at the S2S time scale (Cortesi 2020): https://meetingorganizer.copernicus.org/EGU2020/EGU2020-1580.html
	- #BSC Nicola Cortesi  
	- weather regime classification at the s2s time scale for enhancing s2s predictability of the frequencies of weather regimes
	- using clustering techniques (k-means) and weighting based on the anomaly correlation coeff. (ACC) 
	- using NCEP reanalysis 40 years, Euro-Atlantic region
	- forecasts from the 2018 Monthly forecast system ECMWF-MFS
- #PAPER Monthly and Quarterly Sea Surface Temperature Prediction Based on Gated Recurrent Unit Neural Network (Zhang 2020): https://www.mdpi.com/2077-1312/8/4/249/htm
	- A medium and long-term SST prediction model is designed on the basis of the gated recurrent unit (GRU) neural network algorithm
	- Data: NOAA 1/4° daily Optimum Interpolation (OISST), reanalysis. This study selects the site data from January 1982 to December 2019 and reorganizes the data on the basis of the monthly and seasonal averages
	- Model: A neural network model for the high-precision prediction of medium and long-term SSTs based on GRU and a fully connected layer is constructed. Six-layer neural network model, which includes one input layer, three GRU layers, and two dense layers. 
	- The input data are the time series of the SST. In this experiment, the time series of monthly and quarterly scales are used to verify the model, and the amount of data fed into the network at one time is determined by the length of the set learning sequence and the number of batch trainings. On the basis of the variation law of SST, the lengths of learning sequences used in monthly and quarterly trainings are set to 12 and 4, respectively.
	- The 38-year history of SST observation data is sorted on the basis of two different scales: monthly and quarterly
	- The designed SST prediction model based on GRU can efficiently fit the trend of the real SST
- #PAPER Improving seasonal forecast using probabilistic deep learning (Pan 2020): https://arxiv.org/abs/2010.14610v1
	- Conditional variational autoencoders (conditional generative model that marries probabilistic graphical models with deep learning)
	- Saliency maps
- #PAPER Predicting global patterns of long-term climate change from short-term simulations using machine learning (Mansfield 2020): https://www.nature.com/articles/s41612-020-00148-5
	- introduced a machine learning approach, which utilises a unique dataset of existing climate model simulations to learn relationships between short-term and long-term temperature responses to different climate forcing scenarios
	- done via a fast "surrogate model" to find a mapping from short-term to long-term response patterns within a given GCM
	- this approach not only has the potential to accelerate climate change projections by reducing the costs of scenario computations, but also helps uncover early indicators of modelled long-term climate responses, which is of relevance to climate change detection, predictability, and attribution
- #PAPER Prediction Skill of Extended Range 2-m Maximum Air Temperature Probabilistic Forecasts Using Machine Learning Post-Processing Methods (Peng 2020): https://www.mdpi.com/2073-4433/11/8/823/htm
- #PAPER Seasonal Arctic sea ice forecasting with probabilistic deep learning (Andersson 2021): https://eartharxiv.org/repository/view/2027/
	- present a probabilistic, deep learning sea ice forecasting system, IceNet, trained on climate simulations and observational data to forecast the next 6 months of monthly-averaged sea ice concentration maps
- #PAPER Applying machine learning for drought prediction using data from a large ensemble of climate simulations (Felsche 2021): https://nhess.copernicus.org/preprints/nhess-2021-110/
- #PAPER Subseasonal Forecasts of Opportunity Identified by an Explainable Neural Network (Mayer 2021): https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020GL092092
	- https://meetingorganizer.copernicus.org/EGU21/EGU21-9015.html
	- Layer-wise relevance propagation (LRP)
	- K-Means Clustering of LRP Maps
- #PAPER Subseasonal predictability of the North Atlantic Oscillation (Albers 2021): https://iopscience.iop.org/article/10.1088/1748-9326/abe781
- #PAPER Sub-seasonal forecasting with a large ensemble of deep-learning weather prediction models (Weyn 2021): https://arxiv.org/abs/2102.05107 ^weyn21dls2s


### Verification
- #BSC Seasonal forecasts quality assessment report (report by Marcos, ESS): https://zenodo.org/record/2391735#.X_29a9Yo9qg
- Guidance on Verification of Operational Seasonal Climate Forecasts: https://library.wmo.int/doc_num.php?explnum_id=4886
- Forecast Verification methods Across Time and Space Scales: https://www.cawcr.gov.au/projects/verification/
- Verification of climate forecasts: http://indico.ictp.it/event/a09161/session/29/contribution/17/material/0/0.pdf

- #PAPER The Discrete Brier and Ranked Probability Skill Scores (Weigel 2007): https://journals.ametsoc.org/view/journals/mwre/135/1/mwr3280.1.xml