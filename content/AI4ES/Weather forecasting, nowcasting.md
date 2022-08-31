---
title: "Weather forecasting, nowcasting"
---

> See:
> - [[AI4ES/Emulators]]
> - [[AI/Computer Vision/Video segmentation and prediction]]
> - [[AI/Deep learning/CNNs]]
> - [[AI/Deep learning/RNNs]]
> - [[AI/Deep learning/Fourier Neural Operators]]


## Code
- #CODE [PySTEPS - Python framework for short-term ensemble prediction systems](https://github.com/pySTEPS/pysteps)
	- https://pysteps.github.io/

## Courses
- #COURSE [ Sources of uncertainty (Buizza, ECMWF)](https://www.ecmwf.int/en/elibrary/19274-sources-uncertainty)
- #COURSE [Using stochastic physics to represent model uncertainty](https://www.ecmwf.int/assets/elearning/stochphysics/stochphysics1/story_html5.html)


## References
- #PAPER [ConvLSTM: Convolutional LSTM Network- A Machine Learning Approach for Precipitation Nowcasting (Shi 2015)](https://arxiv.org/abs/1506.04214)
	- #CODE https://keras.io/examples/conv_lstm/
- #PAPER [Deep Learning for Precipitation Nowcasting: A Benchmark and A New Model, trajGRU (Shi 2017)](https://arxiv.org/abs/1706.03458)
	- https://github.com/CNALeon007/TrajGRU
- #PAPER [Automating weather forecasts based on CNNs (Rozas Larraondo 2017)](https://deepstruct.github.io/ICML17/1stDeepStructWS_paper_2.pdf)
- [#THESIS/PHD Application of machine learning techniques to weather forecasting (Rozas Larraondo 2019)](https://addi.ehu.es/handle/10810/32532)
- #PAPER [A Generative Adversarial Gated Recurrent Unit Model for Precipitation Nowcasting (Tian, 2019)](https://ieeexplore.ieee.org/document/8777193)
- #PAPER [Can machines learn to predict weather? Using deep learning to predict gridded 500‐hPa geopotential height from historical weather data (Weyn 2019)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019MS001705)
- #PAPER [Reversible Deep Generative Models for Climate Informatics (Rosenfeld 2019)](https://sailinglab.github.io/pgm-spring-2019/assets/project/final-reports/project7.pdf)
- #PAPER [Prediction of Rainfall Using Intensified LSTM Based Recurrent Neural Network with Weighted Linear Units (Poornima 2019)](https://www.mdpi.com/2073-4433/10/11/668)
- #PAPER [Data-driven predictions of a multiscale Lorenz 96 chaotic system using machine-learning methods: reservoir computing, artificial neural network, and LSTM (Chattopadhyay 2019)](https://arxiv.org/abs/1906.08829)
	- #CODE https://github.com/ashesh6810/RCESN_spatio_temporal
- #PAPER [Deep Uncertainty Quantification: A Machine Learning Approach for Weather forecasting (Wang 2019)](https://arxiv.org/abs/1812.09467)
	- Proposed data-driven method augmented by an effective information fusion mechanism to learn from historical data that incorporates prior knowledge from NWP
	- Weather forecasting problem posed as an end-to-end deep learning problem and solve it by proposing a novel negative log-likelihood error (NLE) loss function
	- A notable advantage of our proposed method is that it simultaneously implements single-value forecasting and uncertainty quantification, which we refer to as deep uncertainty quantification (DUQ)
	- The proposed DUQ is based on sequence-to-sequence (seq2seq, a.k.a Encoder-Decoder)
	- DUQ predicts two values at each timestep corresponding to the predicted mean and variance to parameterize the Gaussian distributions
- #PAPER [Computer Vision in Precipitation Nowcasting: Applying Image Quality Assessment Metrics for Training Deep Neural Networks (Tran 2019)](https://www.mdpi.com/2073-4433/10/5/244/htm)
- #PAPER [Technical note: DL for creating surrogate models of precipitation in Earth system models (Weber 2020)](https://www.atmos-chem-phys.net/20/2303/2020/)
	- Precipitation forecasting using resnets		
	- #CODE https://github.com/hutchresearch/deep_climate_emulator
- #PAPER [Improving data-driven global weather prediction using deep CNNs on a cubed sphere (Weyn 2020)](https://arxiv.org/abs/2003.11927) ^bd4b0a
	- https://github.com/jweyn/DLWP-CS
	- New developments in this framework include an offline volume-conservative mapping to a cubed-sphere grid, improvements to the CNN architecture (U-NET), and the minimization of the loss function over multiple steps in a prediction sequence.
	- The cubed-sphere remapping minimizes the distortion on the cube faces on which convolution operations are performed and provides natural boundary conditions for padding in the CNN. 
	- Our improved model produces weather forecasts that are indefinitely stable and produce realistic weather patterns at lead times of several weeks and longer
	- #TALK [S2S forecasting using large ensembles of data-driven global weather prediction models](https://www.youtube.com/watch?v=Yk0eSNs7nbs)
- #PAPER [A Machine-Learning-Based Global Atmospheric Forecast Model (Szunyogh 2020)](https://www.essoar.org/doi/10.1002/essoar.10502527.2)
	- The paper investigates the applicability of machine learning (ML) to weather prediction by building a reservoir-computing-based, low-resolution, global prediction model. 
	- The model is designed to take advantage of the massively parallel architecture of a modern supercomputer. 
	- The forecast performance of the model is assessed by comparing it to that of daily climatology, persistence, and a numerical (physics-based) model of identical prognostic state variables and resolution
- #PAPER [MetNet: A Neural Weather Model for Precipitation Forecasting (Sonderby 2020)](https://arxiv.org/abs/2003.12140)
	- #TALK https://vimeo.com/417618472
		- https://www.ecmwf.int/sites/default/files/medialibrary/2020-05/12_May.pdf
- #PAPER [TRU-NET: A Deep Learning Approach to High Resolution Prediction of Rainfall (Adewoyin 2020)](https://arxiv.org/abs/2008.09090v1)
	- #CODE https://github.com/Akanni96/TRUNET
- #PAPER [Predicting clustered weather patterns: A test case for applications of convolutional neural networks to spatio-temporal climate data (Chattopadhyay, 2020)](https://www.nature.com/articles/s41598-020-57897-9) ^e83f4e
	- Introduced an unsupervised auto-labeling strategy that can facilitate exploring the capabilities of supervised deep learning techniques such as CNNs in studying problems in climate and environmental sciences
	- Applied this strategy to clustered daily large-scale weather patterns over North America
		- focused on re-identifying and predicting the daily weather patterns over North America in summer and winter
		- focus on daily averaged geopotential height at 500 hPa (Z500 hereafter), whose isolines are approximately the streamlines of the large-scale circulation at mid-troposphere and are often used to represent weather patterns
		- used data from the Large Ensemble (LENS) Community Project, which consists of a 40-member ensemble of fully-coupled Community Earth System Model version 1 (CESM1) simulations with historical radiative forcing from 1920 to 2005
		- daily Z500 from 1980 to 2005 provides  ~95000 samples for summer months and for winter months over North America
		- the K-means algorithm is used to classify the winter days and summer days (separately) into n = 4 clusters
		- the clustering analysis is performed on zonal-mean-removed daily Z500 anomalies projected on 22 EOFS that retain approximately 95% of the variance
		- the computed cluster index for each day is used to label the full Z500 pattern of that day and 5 days earlier
		- full Z500 fields are used, rather than the computed anomalies (or any other type of anomalies), because one hopes to use CNN with minimally pre-processed data
		- task: re-identifying and predicting the clusters in the full Z500 fields, which include complex temporal variabilities such as the seasonal cycle and non-stationarity resulting from the low-frequency coupled ocean-atmosphere modes and changes in the radiative forcing between 1980 and 2005
		- network: trivial CNN for classification with a final output of 4 values (categorical cross-entropy)
	- Showed the outstanding performance of CNNs in re-identifying and predicting patterns in chaotic, multi-scale, non-stationary, spatio-temporal data with minimal pre-processing
	- CNNs are not used as a clustering technique, as clusters are already found using an unsupervised method (the K-means algorithm). Rather, CNNs are used to predict which cluster index a Z500 pattern will belong to in 1–5 days in the future
	- The cluster-based forecasting of circulation patterns that is presented here, again if performed using a CNN trained on reanalysis data and using more input variables, might help with prediction of low-frequency variability in the S2S timescales (see [[S2S]])
	- The scaling (of the prediction accuracy of the CNNs) that is found here shows a nonlinear relation between accuracy and N, and suggests that the amount of data currently available from reanalysis since 1979 can be enough to successfully train an accurate CNN for applications involving daily large-scale weather patterns
	- Follow up paper using CapsNets and extreme temperature clusters [[AI4ES/Extremes events#^d42267]]
- #PAPER [A review of radar-based nowcasting of precipitation and applicable machine learning techniques (Prudden, 2020)](https://arxiv.org/abs/2005.04988)
- #PAPER [Boosting performance in machine learning of geophysical flows via scale separation (Faranda 2020)](https://npg.copernicus.org/preprints/npg-2020-39/)
- #PAPER [DeepClimGAN: A High-Resolution Climate Data Generator (Puchko 2020)](https://arxiv.org/abs/2011.11705)
	- [[GANs]] for spatio-temporal forecasting
	- https://www.climatechange.ai/CameraReadySubmissions%202-119/52/CameraReadySubmission/nips2019_icml.pdf
- #PAPER [A generative adversarial network approach to (ensemble) weather prediction (Bihlo 2020)](https://arxiv.org/abs/2006.07718)
	- Implemented a deep convolutional [[GANs]] to predict the geopotential height of the 500 hPa pressure level, the two-meter temperature and the total precipitation for the next 24 hours over Europe
	- The proposed models are trained on 4 years of ERA5 reanalysis data from 2015–2018 with the goal to predict the associated meteorological fields in 2019
	- The forecasts show a good qualitative and quantitative agreement with the true reanalysis data for the geopotential height and two-meter temperature, while failing for total precipitation, thus indicating that weather forecasts based on data alone may be possible for specific meteorological parameters
- #PAPER [Ensemble methods for neural network-based weather forecasts (Scher 2020)](https://arxiv.org/abs/2002.05398v2)
	- #CODE https://github.com/sipposip/ensemble-neural-network-weather-forecasts
	- Aimed to transform a deterministic neural network weather forecasting system into an ensemble forecasting system
	- Tested four methods to generate the ensemble: random initial perturbations, retraining of the neural network, use of random dropout in the network, and the creation of initial perturbations with singular vector decomposition
	- The latter method is widely used in numerical weather prediction models, but is yet to be tested on neural networks
	- The ensemble mean forecasts obtained from these four approaches all beat the unperturbed neural network forecasts, with the retraining method yielding the highest improvement
	- The skill of the neural network fore-casts is systematically lower than that of state-of-the-art numerical weather prediction models
- #PAPER [Spherical convolution and other forms of informed machine learning for deep neural network based weather forecasts (Scher 2020)](https://arxiv.org/abs/2008.13524)
	- CNN-based weather forecasting solutions are are usually trained on atmospheric data represented as regular latitude-longitude grids, neglecting the curvature of the Earth
	- Showed the benefit of replacing the convolution operations with a spherical convolution operation, which takes into account the geometry of the underlying data, including correct representations near the poles
	- Additionally, studied the effect of including the information that the two hemispheres of the Earth have “flipped” properties - for example cyclones circulating in opposite directions - into the structure of the network
	- Using spherical convolution leads to an additional improvement in forecast skill, especially close to the poles in the first days of the forecast
	- The spherical convolution is implemented flexibly and scales well to high resolution datasets, but is still significantly more expensive than a standard convolution operation
- #THESIS/PHD [Artificial intelligence in weather and climate prediction (Scher 2020)](https://www.diva-portal.org/smash/get/diva2:1425352/FULLTEXT01.pdf ^2e6f0f)
- #THESIS/MSC [Geometric deep learning for medium-range weather prediction (Llorens 2020)](https://infoscience.epfl.ch/record/278138)
	- #CODE https://github.com/illorens/weather_prediction
	- Spherical CNNs benchmarking
- #PAPER [Temporal convolutional neural (TCN) network for an effective weather forecasting using time-series data from the local weather station (Hewage 2020)](https://link.springer.com/article/10.1007/s00500-020-04954-0)
- #PAPER [Optimization of Deep Learning Precipitation Models Using Categorical Binary Metrics (Rozas Larraondo 2020)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019MS001909)
	- #CODE https://github.com/prl900/weather_encoders
	- This work introduces a methodology for optimizing neural network models using a combination of continuous and categorical binary indices in the context of precipitation forecasting
	- Proposed an alternative formulation for these categorical indices that are differentiable and we demonstrate how they can be used to optimize the skill of precipitation neural network models defined as a multiobjective optimization problem
- #PAPER [Localized Convolutional Neural Networks for Geospatial Wind Forecasting (Uselis 2020)](https://www.mdpi.com/1996-1073/13/13/3440/htm) ^uselis20
	- #CODE https://github.com/oshapio/Localized-CNNs-for-Geospatial-Wind-Forecasting
	- In a convolutional layer, each neuron has a fixed local receptive field of the layer input and shares its weights with all the other (repeated) neurons arranged in a lattice corresponding to the dimensions of the input
	- Typically, an element-wise nonlinear function is applied to the results of the convolution which gives a lattice of identical weighted-sum-and-non linearity neurons each looking at a different k×k size patch of the input image
	- Convolutions give CNNs some unique benefits, compared to regular MLPs: less trainable weights (faster and with less overfitting), every filter is trained on every k×k patch of every input image g(·,·), which utilizes the training data well, the architecture and learned weights of the convolutional layer do not depend on the size of the input image (easier to reuse), convolutions give translation invariance (the features are detected the same way, no matter where they are in the image)
	- Translation invariance is very important for good generalization when objects being detected are randomly framed in the images. Translation invariance, however, is absolute in convolutional layers
	- This location agnosticism might not always be optimal even for images as not all objects or features are equally likely to appear in every part of them. This is especially evident when the images have a constant static framing, eg., geospatial ad meteorological data
	- While the same laws of atmospheric physics apply at every location, each location typically also has its own unique features like altitude, terrain, land use, large objects, sun absorption, the heat capacity of the ground,heat sources, etc. that affect the dynamics
	- The complete location agnosticism in CNNs can be remedied in several ways by supplying different additional static location-dependent features:
		- The explicit coordinates of each location like in CoordConv 
		- A combination of local random static location-dependent inputs, that could potentially allow us to uniquely “identify” each location as well
		- The above mentioned real-world relevant unique location-specific features if they are explicitly available (typically not all of them are)
	- Additionally, location-based differences could be learned more directly by introducing additional (at every input lattice location): 
		- Learnable local inputs/latent variables
		- Learnable local transformations of the inputs in the form of local weights
	- “Localized CNNs” - models that learn to treat the different locations/pixels in the input similarly, but not identically
- #PAPER [Deep spatial transformers for autoregressive data-driven forecasting of geophysical turbulence (Chattopadhyay 2020)](https://dl.acm.org/doi/10.1145/3429309.3429325)
	- https://eartharxiv.org/repository/view/118/
- #PAPER [Data-driven medium-range weather prediction with a Resnet pretrained on climate simulations: A new model for WeatherBench (Rasp 2021)](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020MS002405)
	- There are three fundamental techniques for creating data‐driven forecasts: direct, continuous and iterative. For direct forecasts, a separate model is trained directly for each desired forecast time. In continuous models, time is an additional input and a single model is trained to predict all forecast lead times (as in MetNet). Finally, iterative forecasts are created by training a direct model for a short forecast time (e.g., 6 h) and then running the model several times using its own output from the previous iteration. As mentioned above, this is the approach taken by Weyn et al. 2020
	- First train our model using the 150 years of CMIP data described above. We then take the pretrained model and fine‐tune it using the ERA data
- #PAPER [Evaluation and interpretation of convolutional long short-term memory networks for regional hydrological modelling (Anderson 2022)](https://hess.copernicus.org/articles/26/795/2022/hess-26-795-2022.html)
	- #CODE https://github.com/andersonsam/cnn_lstm_era
- #PAPER [FourCastNet: A Global Data-driven High-resolution Weather Model using Adaptive Fourier Neural Operators (Pathak 2022)](https://arxiv.org/abs/2202.11214)            
	- [Accelerating Extreme Weather Prediction with FourCastNet](https://www.youtube.com/watch?v=nuT_U1AQz3g)
	- #TALK [Building Digital Twins of the Earth for NVIDIA's Earth-2 Initiative](https://www.youtube.com/watch?v=IBTVAC82xtQ)
	- #CODE https://github.com/NVlabs/FourCastNet
	- #CODE (NOT OFFICIAL) https://github.com/HFAiLab/FourCastNet
	- ERA5 0.25 deg, 20 variables, from 1979 (~50k training samples)
	- Unparalleled accuracy at forecast lead times of up to one week, challenging variables such as surface winds and precipitation
	- FourCastNet has eight times greater resolution than state-of-the-art DL-based global weather models
	- FourCastNet’s predictions are comparable to the IFS model on metrics of RMSE and Anomaly Correlation Coefficient (ACC) at lead times of up to three days
	- FourCastNet’s reliable, rapid, and computationally inexpensive forecasts facilitate the generation of very large ensembles, thus enabling estimation of well-calibrated and constrained uncertainties in extremes with higher confidence than current NWP ensembles
	- The AFNO model is unique in that it frames the mixing operation as continuous global convolution, implemented efficiently in the Fourier domain with FFTs, which allows modeling dependencies across spatial and channel dimensions flexibly and scalably
- #PAPER [Forecasting large-scale circulation regimes using deformable convolutional neural networks and global spatiotemporal climate data (Holm Nielsen 2022)](https://arxiv.org/abs/2202.04964)
	- supervised machine learning approach based on deformable convolutional neural networks (deCNNs) and transfer learning to forecast the North Atlantic-European weather regimes during extended boreal winter for 1 to 15 days into the future
	- authors could extract and learn transformation-invariant spatial patterns across large geographical areas using deformable convolutions, which is not possible with regular CNNs
	- used pre-training (training on the large 20CRv3 reanalysis dataset spanning from 1836 to 1980, then transfer learning)
	- using a interpretation technique called integrated gradients, we could attribute each variable’s contributions for a particular observation on a grid-point basis. This is especially important if we want to understand global climate processes better and explain drivers behind specific weather regimes that account for major uncertainty in NWP models days to weeks ahead
- #PAPER [Towards physics-inspired data-driven weather forecasting: integrating data assimilation with a deep spatial-transformer-based U-NET in a case study with ERA5 (Chattopadhyay 2022)](https://gmd.copernicus.org/articles/15/2221/2022/)
- #PAPER [Earthformer: Exploring Space-Time Transformers for Earth System Forecasting (Gao 2022)](https://arxiv.org/pdf/2207.05833)
	- Earthformer is a space-time Transformer for Earth system forecasting. Earthformer is based on a generic, flexible and efficient space-time attention block, named Cuboid Attention
	- The idea is to decompose the data into cuboids and apply cuboid-level self-attention in parallel. These cuboids are further connected with a collection of global vectors