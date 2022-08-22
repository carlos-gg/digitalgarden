---
title: "Extremes events"
---

> See:
> - [[AI/Anomaly and Outlier Detection]]


## Resources
- [CASCADE - multidivisional, collaborative project at Lawrence Berkeley National Laboratory (LBNL)](https://cascade.lbl.gov/)
- [CLIMATE EXTREMES (Coumou)](https://climateextremes.eu/)
- [EO-ALERT (2018-2021) - Next generation satellite processing chain for rapid civil alerts](http://eo-alert-h2020.eu/)
	- [AI for Earth observation and numerical weather prediction](http://eo-alert-h2020.eu/2019/04/22/ai-for-earth-observation-and-numerical-weather-prediction/)
- [National Meteorological Library and Archive Fact sheet 3 — Water in the atmosphere](https://www.metoffice.gov.uk/binaries/content/assets/metofficegovuk/pdf/research/library-and-archive/library/publications/factsheets/factsheet_3-water-in-the-atmosphere.pdf)
- https://www.deeprain-project.de/en/publications-2/
- [Severe weather Europe](https://www.severe-weather.eu/)

### Hurricanes
- [Hurricanes Database](https://products.climate.ncsu.edu/weather/hurricanes/database/?search=year&yr=2017)
- [Barometric Pressure & Hurricanes](https://sciencing.com/barometric-pressure-hurricanes-22734.html)

### Wildfires
- [EOS - Forest Fire Monitoring](https://eos.com/industries/forestry/forest-fires-identification/) 
- [2017 Conference on Fire Prediction Across Scales](http://extremeweather.columbia.edu/events/past-events/2017-conference-on-fire-prediction-across-scales/
- [Climate Change Increases the Risk of Wildfires](https://sciencebrief.org/briefs/wildfires)
- [Leverhulme Centre for Wildfires, Environment and Society](https://centreforwildfires.org/projects/) 

### Atmospheric rivers
- See ClimateNet dataset
- https://en.wikipedia.org/wiki/Atmospheric_river
- [About ARs (NOAA)](https://www.psl.noaa.gov/arportal/about/)


## Code
- #CODE [ecPoint-Rainfall - Global probabilistic rainfall at point-scale from ECMWF ensemble](https://www.ecmwf.int/en/elibrary/18331-ecpoint-rainfall-global-probabilistic-rainfall-point-scale-ecmwf-ensemble)
- #CODE [TECA - the Toolkit for Extreme Climate Analysis](https://github.com/LBL-EESA/TECA)
	- TECA (Toolkit for Extreme Climate Analysis) is a collection of climate analysis algorithms geared toward extreme event detection and tracking implemented in a scalable parallel framework. The core is written in modern c++ and uses MPI+thread for parallelism


## Databases
See [[AI4ES/AI4ES data#Extreme events labeled data]]
- [Copernicus Emergency Management Service (EMS)](https://emergency.copernicus.eu/mapping/ems/service-overview)
	- EMS uses satellite imagery and other geospatial data to provide free of charge mapping service in cases of natural disasters, human-made emergency situations and humanitarian crises throughout the world
	- [List of EMS Rapid Mapping Activations](https://emergency.copernicus.eu/mapping/list-of-activations-rapid)
	- Flood, wildfire, volcanic events, earthquakes
- [European Drought Observatory](https://edo.jrc.ec.europa.eu/edov2/php/index.php?id=1000)
- [IBTrACS](https://www.ncdc.noaa.gov/ibtracs/)
	- https://climetlab.readthedocs.io/en/latest/firststeps.html
- [ESWD](<[European Severe Weather Database](https://eswd.eu/cgi-bin/eswd.cgi#lookupanchor)>)  
	- "Extreme Weather Database" will be a nice thing to test because it contains events that are not resolved by the reanalysis. So will really help to identify local-scale (convective) high-impact events
	- Type of events: dust, sand- or steam devils, gustnadoes, large hail, heavy rain, tornadoes, severe wind gusts, heavy snowfalls/snowstorms, ice accumulations, avalanches, damaging lightning strikes 
- [NCEI's Severe Weather Data Inventory (US)](https://www.ncdc.noaa.gov/ncdcs-severe-weather-data-inventory)
- [TEMPEST (UK)](https://www.nottingham.ac.uk/research/groups/weather-extremes/research/tempest-database.aspx)
	- Tracking Extremes of Meteorological Phenomena Experienced in Space and Time
	- Work in progress


## References - Climate
- #PAPER [Climate and Weather Extremes (Nature paper collection)](https://www.nature.com/collections/kpzbllmxxw)
	- [Progress in subseasonal to seasonal prediction through a joint weather and climate community effort (Mariotti 2018)](https://www.nature.com/articles/s41612-018-0014-z)
	- [The sub-seasonal to seasonal prediction project (S2S) and the prediction of extreme events (Vitart 2018)](https://www.nature.com/articles/s41612-018-0013-0)
- #PAPER [Simulation and Prediction of Category 4 and 5 Hurricanes in the High-Resolution GFDL HiFLOR Coupled Climate Model (Murakami 2015)](https://journals.ametsoc.org/jcli/article/28/23/9058/34488/Simulation-and-Prediction-of-Category-4-and-5)
- #PAPER [A toolkit for climate change analysis and pattern recognition for extreme weather conditions – Case study: California-Baja California Peninsula (Vaghefi 2017)](http://www.sciencedirect.com/science/article/pii/S1364815216303188)
- #PAPER [Urban heat wave hazard and risk assessment (Jedlovec 2017)](https://www.sciencedirect.com/science/article/pii/S2211379717316686)
- #PAPER [Defining Extreme Events: A Cross‐Disciplinary Review (McPhillips, 2018)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2017EF000686)
	- Extreme events are of interest worldwide given their potential for substantial impacts on social, ecological, and technical systems
	- Many climate‐related extreme events are increasing in frequency and/or magnitude due to anthropogenic climate change 
	- A lack of coherence exists in what constitutes and defines an extreme event across these fields, which impedes our ability to holistically understand and manage these events
	- Found a wide range in definitions and thresholds, with more than half of examined papers not providing an explicit definition, and disagreement over whether impacts are included in the definition
	- Distinction should be made between extreme events and their impacts, so that we can better assess when responses to extreme events have actually enhanced resilience
- #PAPER [Sense‐making in social media during extreme events (Stieglitz, 2018)](https://onlinelibrary.wiley.com/doi/full/10.1111/1468-5973.12193)
- #PAPER [Complex networks reveal global pattern of extreme-rainfall teleconnections (Boers 2019)](https://www.nature.com/articles/s41586-018-0872-x)
- #PAPER [A ranking of concurrent precipitation and wind events for the Iberian Peninsula (Henin 2020)](https://rmets.onlinelibrary.wiley.com/doi/10.1002/joc.6829)
- #PAPER [Atmospheric convection, dynamics and topography shape the scaling pattern of hourly rainfall extremes with temperature globally (Moustakis 2020)](https://www.nature.com/articles/s43247-020-0003-0)

### Droughts
- #PAPER [Development of a Combined Drought Indicator to detect agricultural drought in Europe (Sepulcre-Canto 2012)](https://doi.org/10.5194/nhess-12-3519-2012)
- #PAPER [Seasonal Drought Prediction: Advances, Challenges, and Future Prospects (Hao 2018)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1002/2016RG000549)
- #PAPER [Machine learning–based observation-constrained projections reveal elevated global socioeconomic risks from wildfire (Yu 2022)](https://www.nature.com/articles/s41467-022-28853-0)

### Wildfires
- #PAPER [Seasonal predictions of Fire Weather Index: Paving the way for their operational applicability in Mediterranean Europe (Bedia 2018)](https://www.sciencedirect.com/science/article/pii/S2405880716300826)
	- See [[AI4ES/S2S]]
- #PAPER [Skillful forecasting of global fire activity using seasonal climate predictions (Turco 2018)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6045620/)
	- See [[AI4ES/S2S]]
- #PAPER [The Global Fire Atlas of individual fire size, duration, speed and direction (Andela 2019)](https://essd.copernicus.org/articles/11/529/2019/)

### Atmospheric rivers
- #PAPER [Daily Precipitation Extreme Events in the Iberian Peninsula and Its Association with Atmospheric Rivers (Ramos 2015)](https://journals.ametsoc.org/view/journals/hydr/16/2/jhm-d-14-0103_1.xml)
- #PAPER [On the relationship between atmospheric rivers, weather types and floods in Galicia, NW Spain (Eiras-Barca 2018)](https://nhess.copernicus.org/articles/18/1633/2018/)
- #PAPER [Predictive skill for atmospheric rivers in the western Iberian Peninsula (Ramos 2020)](https://nhess.copernicus.org/articles/20/877/2020/)
- #PAPER [Atmospheric Rivers and Associated Precipitation over France and Western Europe: 1980–2020 Climatology and Case Study (Doiteau 2021)](https://www.mdpi.com/2073-4433/12/8/1075)

### Extreme events and Climate Change
- [Extreme Climate and Weather Events in a Warmer World](https://kids.frontiersin.org/articles/10.3389/frym.2022.682759)
- [Wildfires and Climate Change](https://www.c2es.org/content/wildfires-and-climate-change/)
- [Commentary: How summer 2021 has changed our understanding of extreme weather](https://www.channelnewsasia.com/commentary/commentary-how-summer-2021-has-changed-our-understanding-extreme-weather-2098356)
- [Extreme weather: How is it connected to climate change?](https://www.bbc.com/news/science-environment-58073295)
- [Yes, climate change can affect extreme weather – but there is still a lot to learn](https://theconversation.com/yes-climate-change-can-affect-extreme-weather-but-there-is-still-a-lot-to-learn-136003)
- [Is the weather actually becoming more extreme? - R. Saravanan (TED, POPSCI)](https://www.youtube.com/watch?v=NCPTbfQyMt8)
- [Attributing extreme weather toclimate change (interactive map of studies worldwide)](https://www.carbonbrief.org/mapped-how-climate-change-affects-extreme-weather-around-the-world?utm_content=buffer4760c)
- [ClimExtreme - A research network on climate change and extreme events](https://www.climxtreme.net)
	- https://www.xces.dkrz.de/


## References - ML
- #PAPER [Machine Learning for Projecting Extreme Precipitation Intensity for Short Durations in a Changing Climate (Hu 2019)](https://www.mdpi.com/2076-3263/9/5/209/htm)
- #PAPER [Extreme precipitation events under climate change in the Iberian Peninsula (Cardoso, 2019)](https://rmets.onlinelibrary.wiley.com/doi/10.1002/joc.6269 )
	- https://www.researchgate.net/publication/335040085_Extreme_Precipitation_Events_under_Climate_Change_in_the_Iberian_Peninsula

### Supervised learning approaches
See [[AI/Supervised Learning/Supervised learning]] 
- #PAPER [Application of Deep Convolutional Neural Networks for Detecting Extreme Weather in Climate Datasets (Liu 2016)](https://arxiv.org/abs/1605.01156)
	- Detecting extreme events in large datasets is a major challenge in climate science research.   
	- Current algorithms for extreme event detection are build upon human expertise in defining events based on subjective thresholds of relevant physical variables
	- Developed deep [[AI/Deep learning/CNNs]] classification system and demonstrated the usefulness of [[AI/Deep learning/DL]]  technique  for  tackling  climate  pattern  detection problems
	- Achieved 89%-99% of accuracy in detecting extreme events (Tropical Cyclones, Atmospheric Rivers and Weather Fronts)
- #PAPER [Resolution Reconstruction of Climate Data with Pixel Recursive Model (Kim 2017)](https://ieeexplore.ieee.org/document/8215679)
	- https://www.researchgate.net/publication/322001089_Resolution_Reconstruction_of_Climate_Data_with_Pixel_Recursive_Model
	- CNNs to detect extreme climate events without handcrafted algorithmic definition: detect and localize tropical cyclone in GCM scaled low resolution reanalysis data, which suggests the possibility to reduce the computing load of conventional expensive downscaling process
	- Combined pixel recursive super resolution techniques with localization CNNs to achieve better SR performance and to improve localization accuracy
	- Implemented distributed training in pixel recursive module to fasten training using GPU
- #PAPER [Segmenting and Tracking Extreme Climate Events using Neural Networks (Mudigonda 2017)](https://www.semanticscholar.org/paper/Segmenting-and-Tracking-Extreme-Climate-Events-Mudigonda-Kim/44c74b5a8dab90153dd81394d43a9de718478dbd)
	- https://dl4physicalsciences.github.io/files/nips_dlps_2017_20.pdf
- #PAPER [Leveraging LSTM for rapid intensifications prediction of tropical cyclones (Gong Li 2017)](https://www.semanticscholar.org/paper/Leveraging-LSTM-for-rapid-intensifications-of-Li-Yang/bcd623da4eed9197dd1a25f69d496171c99a1cce)
	- TC intensity forecasting helps people prepare for the extreme weather and could save lives and properties. Rapid Intensifications (RI) of TCs are the major error sources of TC intensity forecasting
	- Experiments show that the long short-term memory (LSTM) network provides the ability to leverage past conditions to predict TC rapid intensifications
	- SHIPS (DeMaria and Kaplan 1994) database is chosen for this study as it contains most well-known environmental predictors relevant  to  TC  intensity  changes,  such  as  Reynolds  SST  (sea surface temperature), SLP (sea level pressure). 
	- These predictor values are from reanalysis fields as well as satellite derived variable values and stored as a text file in ASCII format
	- According  to  the  definition  of  RI,  if  the  maximum  wind increased more than 30 knots (15.4 m/s) over the past 24 hours (Kaplan and DeMaria 2003), the record is marked as RI case, otherwise, it is labeled UNRI
- #PAPER [A machine learning workﬂow for hurricane prediction (Kahira 2018)](https://upcommons.upc.edu/handle/2117/124992)
	- #BSC LP Caron, Leonardo Bautista 
- #PAPER [Training deep neural networks with low precision input data: a hurricane prediction case study (Kahira 2018)](https://upcommons.upc.edu/handle/2117/132833)
- #PAPER [Fused DL for Hurricane Track Forecast from Reanalysis Data (Giffard-Roisin 2018)](https://www.semanticscholar.org/paper/Fused-Deep-Learning-for-Hurricane-Track-Forecast-Giffard-Roisin-Yang/6aad16c4cfc5bf73f74671dddd01a47f63e71e30)
- #PAPER [Lightning Prediction for Australia Using Multivariate Analyses of Large-Scale Atmospheric Variables (Bates 2018)](https://journals.ametsoc.org/jamc/article/57/3/525/68263/Lightning-Prediction-for-Australia-Using)
- #PAPER [Defining heatwave thresholds using an inductive machine learning approach (Park and Kim, 2018)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0206872)
	- Establishing appropriate heatwave thresholds is important in reducing adverse human health consequences as it enables a more effective heatwave warning system and response plan
	- This paper defined such thresholds by focusing on the non-linear relationship between heatwave outcomes and meteorological variables as part of an inductive approach
	- Daily data on emergency department visitors who were diagnosed with heat illnesses and information on 19 meteorological variables were obtained for the years 2011 to 2016 from relevant government agencies
	- A Multivariate Adaptive Regression Splines (MARS) analysis was performed to explore points (referred to as “knots”) where the behaviour of the variables rapidly changed
- #PAPER [Predicting Hurricane Trajectories using a Recurrent Neural Network (Alemany 2018)](http://arxiv.org/abs/1802.02548)
- #PAPER [Exascale DL for Climate Analytics (Kurth 2018)](https://arxiv.org/abs/1810.01993)
	- #CODE https://github.com/sparticlesteve/climate-seg-benchmark
	- #TALK [Exascale Deep Learning for Climate Analytics (Thorsten Kurth, Lawrence Berkeley National Laboratory, TF Dev Summit ‘19)](https://www.youtube.com/watch?v=4uq9OODJpO0)
		- Climate change will have fundamental socio-economic impact and it is imperative for us to understand it better. This talk will show how TensorFlow was utilized on the world’s fastest supercomputer in order to extract pixel level segmentation masks of extreme weather phenomena in climate simulation data, thereby enabling climate scientists to perform high-fidelity, fine grained geo-spatial analyses of the effects of climate change 
	- DeepLabv3 — Atrous Convolution (Semantic Segmentation) 
		- https://towardsdatascience.com/review-deeplabv3-atrous-convolution-semantic-segmentation-6d818bfd1d74 
		- https://towardsdatascience.com/review-dilated-convolution-semantic-segmentation-9d5a5bd768f5 
- #PAPER [DeepTC: ConvLSTM Network for Trajectory Prediction of Tropical Cyclone using Spatiotemporal Atmospheric Simulation Data (Kim 2018)](https://www.semanticscholar.org/paper/DeepTC%3A-ConvLSTM-Network-for-Trajectory-Prediction-Kim-Kang/e342082b0a9581a89360e4327d241684ec4fc8c6)
- #PAPER [Deep-Hurricane-Tracker - Tracking and Forecasting Extreme Climate Events (Kim 2019)](https://ieeexplore.ieee.org/document/8658402)
	- http://www.joonseok.net/papers/wacv19.pdf
	- #CODE https://github.com/kim79sookyung/hurricane_detection_cnn
	- Convolutional LSTM (ConvLSTM)-based spatio-temporal models to track and predict hurricane trajectories from large-scale climate data. To address the tracking problem, we model time-sequential density maps of hurricane trajectories, enabling to capture not only the temporal dynamics but also spatial distribution of the trajectories. Furthermore, we introduce anew trajectory prediction approach as a problem of sequential forecasting from past to future hurricane density map sequences  
	- CAM5 (zonal wind (U850), meridional wind(V850),  and precipitation (PRECT)) and TECA labels (automated heuristics)
	- http://www.joonseok.net/papers/deep_tracker.pdf (Climate informatics 2018)
- #PAPER [Improving Atmospheric River Forecasts With Machine Learning (Chapman 2019)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2019GL083662)
- #PAPER [High Resolution Forecasting of Heat Waves impacts on Leaf Area Index by Multiscale Multitemporal Deep Learning (Gobbi 2019)](https://arxiv.org/abs/1909.07786)
- #PAPER [A hybrid CNN-LSTM model for typhoon formation forecasting (Cheng 2019)](https://www.semanticscholar.org/paper/A-hybrid-CNN-LSTM-model-for-typhoon-formation-Chen-Wang/41dc8080372075d3f29df7fb43bf326bbf9900d1)
	- Traditional numerical forecast models based on fluid mechanics have difficulty in predicting the intensity of typhoons. Forecasts based on statistics and machine learning fail to take into account the spatial and temporal relationships among typhoon formation variables leading to weaknesses in the predictive power of this model
	- Proposed a hybrid model, which we argue, can produce a more realist and accurate account of typhoon ‘behavior’ as it focuses on both the spatio-temporal correlations of atmospheric and oceanographic variables
	- The CNN-LSTM model introduces 3D convolutional neural networks (3DCNN) and 2D convolutional neural networks (2DCNN) as a method to better understand the spatial relationships of the features of typhoon formation. LSTM is used to examine the temporal sequence of relations in typhoon progression
- #PAPER [Deep Learning for Spatially Explicit Prediction of Synoptic-Scale Fronts (Lagerquist, 2019)](https://journals.ametsoc.org/waf/article/34/4/1137/344706/Deep-Learning-for-Spatially-Explicit-Prediction-of)
	- This paper describes the use of [[AI/Deep learning/CNNs]], a type of deep learning, to identify fronts in gridded data, followed by a novel postprocessing method that converts probability grids to objects
	- Synoptic-scale fronts are often associated with extreme weather in the mid latitudes
	- Predictors are 1000-mb (1 mb = 1 hPa) grids of wind velocity, temperature, specific humidity, wet-bulb potential temperature, and/or geopotential height from the North American Regional Reanalysis
	- Labels are human-drawn fronts from Weather Prediction Center bulletins
	- To evaluate our system, we compare the objects (predicted warm and cold fronts) with human-analyzed warm and cold fronts, matching fronts of the same type within a 100- or 250-km neighborhood distance. At 250 km our system obtains a probability of detection of 0.73, success ratio of 0.65 (or false-alarm rate of 0.35), and critical success index of 0.52. These values drastically outperform the baseline, which is a traditional method from numerical frontal analysis
- #PAPER [High Resolution Forecasting of Heat Waves impacts on Leaf Area Index by Multiscale Multitemporal Deep Learning (Gobbi 2019)](http://arxiv.org/abs/1909.07786v1)
- #PAPER [Make Thunderbolts Less Frightening -- Predicting Extreme Weather Using Deep Learning (Schon 2019)](https://arxiv.org/abs/1912.01277v2)
- #TALK [Probabilistic Detection of Extreme Weather Using Deep Learning Methods (Mahesh 2019)](https://ams.confex.com/ams/2019Annual/webprogram/Paper354370.html)
	- Atmospheric rivers (ARs) are a particularly challenging class of extreme weather event, since there is no single community-accepted AR identification algorithm
	- To represent the uncertainty expressed by contemporary, state-of-the-science AR tracking methods, we create probabilistic AR detection fields from 14 algorithms submitted to the Atmospheric River Tracking Method Intercomparison Project (ARTMIP). Each algorithm identifies grid cells associated with ARs in over 30 years of 3-hourly data from the MERRA reanalysis
	- Estimated each grid cell’s probability of AR detection as the proportion of ARTMIP algorithms that identify an AR in that grid cell 
	- [[AI/Deep learning/CNNs]] segmentation model used to generate probabilistic AR identifications that are quite close to the ARTMIP mean, with an average RMSE of 0.03
- #PAPER [DeepRI: End-to-end Prediction of Tropical Cyclone Rapid Intensification from Climate Data (Jing 2019)](https://www.semanticscholar.org/paper/DeepRI%3A-End-to-end-Prediction-of-Tropical-Cyclone-Jing/985bf8e2cb37ddfab7a912f596156018bc737e7c)
	- NeurIPS 2019
	- TC track forecasting has improved significantly in the past decades, intensity forecasting still shows large forecast error, largely due to the challenge in predicting TC rapid intensification
	- Rapid intensification (RI) is the significant strengthening in storm wind speed within a short time(e.g. >30 kt over 24 hours), and almost all historical category 4 and 5 hurricanes are RI storms
	- Data from multiple resources including visible and infrared satellite imagery provided by operational geostationary satellites and passive microwave imagery from polar-orbiting satellites. Augmented with synthetic data from climate model projections, such as HiFLOR, which is able to simulate Category 4 and 5 TCs
	- Trained separate models for RI prediction for different lead-time, i.e. 6h, 12h, 18h, 24h, and create corresponding training data sets respectively.  For each lead-time, we split independent TCs into training and test split to prevent potential correlations. Overall, this gives us by estimation roughly4000 TCs in training set, and each TC provides a series of pairs of feature map and ground truth binary label indicating whether RI happens. 
- #PAPER [Machine Learning for Generalizable Prediction of Flood Susceptibility (Sidrane 2019)](https://arxiv.org/abs/1910.06521)
- #PAPER [Forecasting El Niño with Convolutional and Recurrent Neural Networks (Mahesh 2019)](https://www.researchgate.net/publication/343794841)
- #PAPER [Spherical CNNs on unstructured grids (Jiang 2019)](https://arxiv.org/abs/1901.02039)
	- #CODE https://github.com/maxjiang93/ugscnn
	- Based on https://github.com/jonas-koehler/s2cnn
- #PAPER [A mixed model approach to drought prediction using artificial neural networks: Case of an operational drought monitoring environment (Adede 2019)](https://arxiv.org/abs/1901.04927)
	- The study uses 10 precipitation and vegetation variables that are lagged over 1, 2 and 3-month time-steps to predict drought situations
	- In the model space search for the most predictive artificial neural network (ANN) model, as opposed to the traditional greedy search for the most predictive variables, we use the General Additive Model (GAM) approach
- #PAPER [Tropical Cyclone Track Forecasting using Fused Deep Learning from Aligned Reanalysis Data (Giffard-Roisin 2020)](https://arxiv.org/abs/1910.10566)
	- Proposed a neural network model fusing past trajectory data and reanalysis atmospheric images (wind and pressure 3D fields)
	- Used a moving frame of reference that follows the storm center for the 24h tracking forecast
	- Model trained to estimate the longitude and latitude displacement of tropical cyclones and depressions from a large database from both hemispheres (more than 3000 storms since 1979, sampled at a 6 hour frequency)
- #PAPER [Tropical and Extratropical Cyclone Detection Using Deep Learning (Kumler-Bonfanti 2020)](https://arxiv.org/abs/2005.09056)
	- U-Net trained with IBTrACS labels on GOES water vapor
	- #TALK ML for Segmentation of Atmospheric Phenomena (Jebb Stewart, NOAA ESRL)
		- https://www.youtube.com/watch?v=mQ3jAxMmeRU&list=PLbelYhZAAHEIr4iC1FNcPXUUYXI0zg_96&index=14&t=0s
		- https://www2.cisl.ucar.edu/sites/default/files/1010%20June%2024%20Stewart%20%281%29.pdf
- #PAPER [Tropical and Extratropical Cyclone Detection Using Deep Learning (Kumler-Bonfanti 2020)](https://arxiv.org/abs/2005.09056v1)
	- This paper discusses four different state-of-the-art U-Net models designed for detection of tropical and extratropical cyclone Regions Of Interest (ROI) from two separate input sources: total precipitable water output from the Global Forecasting System (GFS) model and water vapor radiance images from the Geostationary Operational Environmental Satellite (GOES)
	- These models are referred to as IBTrACS-GFS, Heuristic-GFS, IBTrACS-GOES, and Heuristic-GOES. All four U-Nets are fast information extraction tools and perform with a ROI detection accuracy ranging from 80% to 99%
	- These are additionally evaluated with the Dice and Tversky Intersection over Union (IoU) metrics, having Dice coefficient scores ranging from 0.51 to 0.76 and Tversky coefficients ranging from 0.56 to 0.74
- #PAPER [Improving Emergency Response during Hurricane Season using Computer Vision (Bosch 2020)](https://arxiv.org/abs/2008.07418v2)
- #PAPER [Spatio-temporal segmentation and tracking of weather patterns with light-weight Neural Networks (Kapp-Schwoerer 2020)](https://ai4earthscience.github.io/neurips-2020-workshop/papers/ai4earth_neurips_2020_55.pdf)
	- Uses the ClimateNet [[AI4ES/AI4ES data#Extreme events labeled data]] and the CGNet architecture [[Semantic segmentation]]
	- Weather pattern recognition by deep neural networks can work remarkably better than feature engineering, such as hand-crafted heuristics, used traditionally in climate science
	- Deep Learning - based semantic segmentation of atmospheric rivers and tropical cyclones on the expert-annotated ClimateNet data set, and track individual events using a spatio-temporal overlapping approach
- #PAPER [HydroDeep -- A Knowledge Guided Deep Neural Network for Geo-Spatiotemporal Data Analysis (Sarkar 2020)](https://arxiv.org/abs/2010.04328)
	- Application to floods
	- This paper demonstrates a neural network architecture (HydroDeep) that couples a process-based hydro-ecological model with a combination of Deep Convolutional Neural Network (CNN) and Long Short-Term Memory (LSTM) Network to build a hybrid baseline model
- #PAPER [Graph Neural Networks for Improved El Niño Forecasting (Ruhling Cachay 2020)](https://arxiv.org/abs/2012.01598)

### Semi-supervised learning approaches
See [[AI/Semi-supervised learning]]
- #PAPER [Analog forecasting of extreme-causing weather patterns using deep learning (Chattopadhyay, 2020)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019MS001958) ^d42267
	- LENS data (CESM1 model), [[AI/Deep learning/CapsNets]] and [[AI/Deep learning/CNNs]], extreme temperature events
	- CapsNets are trained on midtropospheric large‐scale circulation patterns (Z500) labeled 0–4 depending on the existence and geographical region of surface temperature extremes over North America several days ahead
	- Impact‐based autolabeling strategy: Knowing the surface temperature over North America on a given day, the Z500 pattern of several days earlier is labeled as 0 (no extreme onset) or 1, 2, 3, or 4 (the cluster indices of T2m extremes)
	- The trained networks predict the occurrence/region of cold or heat waves, only using Z500, with accuracies (recalls) of 69–45% (77–48%) or 62–41% (73–47%) 1–5 days ahead

### Unsupervised learning
See [[AI/Unsupervised learning/Unsupervised learning]]
- #PAPER [Spatial clustering of summer temperature maxima from the CNRM-CM5 climate model ensembles & E-OBS over Europe (Bador 2015)](https://www.sciencedirect.com/science/article/pii/S2212094715300013)
- #PAPER [Multiscale Variability in North American Summer Maximum Temperatures and Modulations from the North Atlantic Simulated by an AGCM (Vigaud 2018)](https://journals.ametsoc.org/jcli/article/31/7/2549/89965/Multiscale-Variability-in-North-American-Summer) ^25cb40
- #PAPER [DisCo: Physics-Based Unsupervised Discovery of Coherent Structures in Spatio-temporal Systems (Rupe, 2019)](https://arxiv.org/abs/1909.11822)
	- #CODE https://github.com/adamrupe/DisCo
- #PAPER [Towards Unsupervised Segmentation of Extreme Weather Events (Rupe, 2019)](https://arxiv.org/abs/1909.07520)
	- Tests on CAM5.1 water vapor data -> extreme weather identification from unlabeled climate model simulation data
	- While the results in using TECA show that DL can improve upon it, the accuracy rates reach 97% and thus essentially just reproduce the output of TECA
	- Though an improvement over automated heuristics, expert-labeled data is still not an objective ground truth
	- To circumvent these challenges of DL-based approaches, here we take an alternative physics-based unsupervised approach, complementary to DL

### Probabilistic approaches
- #PAPER [Bayesian Anomaly Detection and Classification (Roberts, 2019)](https://arxiv.org/abs/1902.08627)
- #PAPER [A probabilistic gridded product for daily precipitation extremes over  the United States (Risser 2019)](https://arxiv.org/pdf/1807.04177)
- #PAPER [Detection Uncertainty Matters for Understanding Atmospheric Rivers (Obrien 2020)](https://journals.ametsoc.org/view/journals/bams/101/6/BAMS-D-19-0348.1.xml)

### Active learning approaches
See [[AI/Active learning]]
- #PAPER [Incorporating Expert Feedback into Active Anomaly Discovery (Das, 2016)](http://web.engr.oregonstate.edu/~tgd/publications/das-wong-dietterich-fern-emmott-incorporating-expert-feedback-into-active-anomaly-discovery-icdm2016.pdf)
- #PAPER [Incorporating Feedback into Tree-based Anomaly Detection (2017)](https://arxiv.org/abs/1708.09441)

### GANs-based approaches
See [[AI/Deep learning/GANs]]
- #PAPER [Learning to Focus and Track Extreme Climate Events (Kim 2019)](https://bmvc2019.org/wp-content/uploads/papers/0728-paper.pdf)
- #PAPER [Visualizing the Consequences of Climate Change Using Cycle-Consistent Adversarial Networks (Schmidt 2019)](https://arxiv.org/abs/1905.03709)
- #PAPER [ExGAN: Adversarial Generation of Extreme Samples (Bhatia 2021)](https://arxiv.org/abs/2009.08454)
	- #CODE https://github.com/Stream-AD/ExGAN
	- https://www.kdnuggets.com/2021/02/adversarial-generation-extreme-samples.html

### Causality studies
- [[Causal modeling in ES#^d43897]]
- [[Causal modeling in ES#^c4333d]]

### Droughts
- #PAPER [Construction of Comprehensive Drought Monitoring Model in Jing-Jin-Ji Region Based on Multisource Remote Sensing Data (Yu 2019)](https://www.mdpi.com/2073-4441/11/5/1077)
- #PAPER [Meteorological drought forecasting based on a statistical model with machine learning techniques in Shaanxi province, China (Zhang 2019)](https://www.sciencedirect.com/science/article/pii/S0048969719302281)
- #PAPER [Using LSTMs for climate change assessment studies on droughts and floods (Krazert 2019)](https://arxiv.org/abs/1911.03941)
- #PAPER [Construction of a drought monitoring model using deep learning based on multi-source remote sensing data (Shen 2019)](https://www.sciencedirect.com/science/article/abs/pii/S0303243418307803)
- #PAPER [A Global Probabilistic Dataset for Monitoring Meteorological Droughts (Turco 2020)](https://journals.ametsoc.org/bams/article/101/10/E1628/345597/A-Global-Probabilistic-Dataset-for-Monitoring)
	- #BSC Markus Donat

### Wildfires
- #PAPER [Mapping regional forest fire probability using artificial neural network model in a Mediterranean forest ecosystem (Satir 2015)](https://www.tandfonline.com/doi/full/10.1080/19475705.2015.1084541) 
- #PAPER [Global Wildfire Outlook Forecast with Neural Networks (Song 2020)](https://www.mdpi.com/2072-4292/12/14/2246/htm)
- #PAPER [Physics-Informed Machine Learning Simulator for Wildfire Propagation (Bottero 2020)](https://arxiv.org/abs/2012.06825v1) 
- #PAPER [Convolutional LSTM Neural Networks for Modeling Wildland Fire Dynamics (Burge 2021)](https://arxiv.org/abs/2012.06679v2) 

### Extreme events and climate change
- #PAPER [Fingerprinting Heatwaves and Cold Spells and Assessing Their Response to Climate Change Using Large Deviation Theory (Galfi and Licarini 2021)](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.058701)
	- https://phys.org/news/2021-08-fingerprints-extreme-weather-revealed-statistical.html

#### Attribution studies
- Attribution studies remain our best (and only) tool for understanding the impact of climate change on extreme weather and on our daily lives. They play a key role in helping [decision makers plan for, or avoid, a future where extreme weather events](https://www.climatecentre.org/news/1253/climate-attribution-work-in-mit-review-ten-a-breakthrough-technologiesa-for-2020) are more likely and intense due to global warming.
- Attribution studies are also really important within climate science as they bridge the gap between observations and model projections. They test climate models in a real-world context, allowing scientists to understand better where they can have more confidence in their projections and where model improvements are needed before projections can be used for decision making.
- https://science2017.globalchange.gov/chapter/3/
- [Detection and Attribution Methodologies Overview](https://science2017.globalchange.gov/chapter/appendix-c/)
- #PAPER [Precipitation downscaling under climate change: Recent developments to bridge the gap between dynamical models and the end user (2010)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2009RG000314)
- #PAPER [Detection and attribution of climate extremes in the observed record (Easterling 2016)](https://www.sciencedirect.com/science/article/pii/S2212094716300020)
- #PAPER [Adapting attribution science to the climate extremes of tomorrow (Harrington 2018)](https://iopscience.iop.org/article/10.1088/1748-9326/aaf4cc)
- #PAPER [Investigating the Role of the Relative Humidity in the Co‐Occurrence of Temperature and Heat Stress Extremes in CMIP5 Projections (2019)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019GL084156)
- #PAPER [Towards reliable extreme weather and climate event attribution (Bellprat 2019)](https://www.nature.com/articles/s41467-019-09729-2)
	- Showed how exploiting advanced correction techniques from the weather forecasting field, that correcting properly for model probabilities alters the attributable risk of extreme events to climate change. 
	- This study illustrates the need to correct for this type of model error in order to provide trustworthy assessments of climate change impacts.
