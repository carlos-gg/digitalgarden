---
title: "Parameterizations"
---

> See [[AI4ES/Emulators]]

## Resources
- [Parametrization (atmospheric modeling)](https://en.wikipedia.org/w/index.php?title=Parametrization_(atmospheric_modeling)&oldid=917836406)
- #TALK [Critical challenges in the simulation of tropical clouds and climate (Maloney, Climate Informatics workshop 2018)](https://www.youtube.com/watch?v=xXUe1WQKV_E&t=1s  )
- #COURSE [ ECMWF Introduction to the parametrization of sub-grid processes](https://www.ecmwf.int/assets/elearning/parametrization/param1/story_html5.html)
- #COURSE ECMWF Cloud and precipitation parametrization 
	- [1. overview and warm-phase microphysics](https://www.ecmwf.int/en/elibrary/18666-cloud-and-precipitation-parametrization-1-overview-and-warm-phase-microphysics)
	- [2. ice and mixed-phase microphysics](https://www.ecmwf.int/en/elibrary/18667-cloud-and-precipitation-parametrization-2-ice-and-mixed-phase-microphysics)


## References
- #PAPER [Using Ensemble of Neural Networks to Learn Stochastic Convection Parameterizations for Climate and Numerical Weather Prediction Models from Data Simulated by a Cloud Resolving Model (Krasnopolsky 2013)](https://www.hindawi.com/journals/aans/2013/485913/)
- #PAPER [Modeling haboob dust storms in large-scale weather and climate models (Pantillon 2016)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1002/2015JD024349)
- #PAPER [Stochastic Parameterization: Toward a New View of Weather and Climate Models (Berner 2017)](https://journals.ametsoc.org/bams/article/98/3/565/70029/Stochastic-Parameterization-Toward-a-New-View-of)
- #PAPER [Deep learning to represent subgrid processes in climate models (Rasp 2018)](https://www.pnas.org/content/115/39/9684)
- #PAPER [Challenges and design choices for global weather and climate models based on machine learning (Dueben and Bauer 2018)](https://gmd.copernicus.org/articles/11/3999/2018/)
- #PAPER [Could Machine Learning Break the Convection Parameterization Deadlock? (Gentine 2018)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018GL078202)
- #PAPER [Prognostic Validation of a Neural Network Unified Physics Parameterization (Brenowitz and Bretherton 2018)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2018GL078510)
- #PAPER [Using Machine Learning to Parameterize Moist Convection: Potential for Modeling of Climate, Climate Change, and Extreme Events (O'Gorman and Dwyer 2018)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2018MS001351)
- #PAPER [Model Parameter Optimization: ML-guided trans-resolution tuning of physical models (Nowack 2018)](https://iopscience.iop.org/article/10.1088/1748-9326/aae2be)
- #PAPER [Applications of Deep Learning to Ocean Data Inference and Subgrid Parameterization (Bolton and Zanna 2019)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018MS001472)
- #PAPER [A data-driven approach to precipitation parameterizations using convolutional encoder-decoder neural networks (Rozas Larraondo 2019)](http://arxiv.org/abs/1903.10274)
	- ERA-Interim data, precipitation as predictant
	- encoder-decoder [[CNNs]] can be used to derive total precipitation using geopotential height as the only input
	- several popular neural network architectures, from the field of image processing, are considered and a comparison with baseline [[machine learning]] methodologies is provided. UNET show best performance
- #PAPER [Fast domain-aware neural network emulation of a planetary boundary layer parameterization in a numerical weather forecast model (Wang 2019)](https://www.geosci-model-dev.net/12/4261/2019/)
- #PAPER [Spatially Extended Tests of a Neural Network Parametrization Trained by Coarse‐Graining (Brenowitz and Bretherton, 2019)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019MS001711)
	- this article describes an NN parametrization trained by coarse‐graining a near‐global CRM simulation with a 4‐km horizontal grid spacing
	- the NN predicts the residual heating and moistening averaged over (160 km)2 grid boxes as a function of the coarse‐resolution fields within the same atmospheric column
- #PAPER [Machine Learning for Stochastic Parameterization: GANs in the Lorenz ’96Model (John Gagne II 2019)](https://arxiv.org/abs/1909.04711)
	- simulations of the atmosphere must approximate the effects of small-scale processes with simplified functions called parameterizations
	- standard parameterizations only predict one output for a given input, but stochastic parameterizations can sample from all the possible outcomes that can occur under certain conditions
	- developed a generative adversarial network machine learning stochasticparameterization of sub-grid forcing for the Lorenz ’96 dynamical mode
	- the generative adversarial networks closely reproduce the spatio-temporal cor-relations and regimes of the Lorenz ’96 system
- #PAPER [Prognostic validation of a neural network unified physics parameterization (Brenowitz and Bretherton, 2020)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018GL078510)
	- a NN based parameterization is trained using a global-scale cloud-resolving simulation. The NN predicts the apparent sources of heat and moisture averaged onto (160 km)^2 grid boxes. A numerically stable scheme is obtained by minimizing the prediction error over multiple time steps rather than single one. In prognostic single column model tests, this scheme outperforms the Community Atmosphere Model by reducing both long-term bias and short-term errors.
- #PAPER [Interpreting and Stabilizing Machine-learning Parametrizations of Convection (Brenowitz 2020)](https://www.semanticscholar.org/paper/Interpreting-and-Stabilizing-Machine-learning-of-Brenowitz-Beucler/a4782e1224121185e11bfa5926717e8f8cff8f0f)
- #PAPER [Stable machine-learning parameterization of subgrid processes for climate modeling at a range of resolutions (Li 2020)](https://arxiv.org/abs/2001.03151)
- #PAPER [Building a machine learning surrogate model for wildfire activities within a global Earth system model (Zhu 2022)](https://gmd.copernicus.org/articles/15/1899/2022/)
	- DNN scheme that surrogates the process-based wildfire model with the Energy Exascale Earth System Model (E3SM) interface. The DNN wildfire model accurately simulates observed burned area with over 90 % higher accuracy with a large reduction in parameterization time compared with the current process-based wildfire model
	- DNN: seems to be a 5-layer MLP [[AI/Deep learning/MLPs]] with softplus activation. The surrogate DNN-Fire is improved by fine-tuning the weight parameters using observations
	- The DNN wildfire model accurately simulates observed burned area with over 90 % higher accuracy with a large reduction in parameterization time compared with the current process-based wildfire model
- #PAPER [Benchmarking of machine learning ocean subgrid parameterizations in an idealized model (Slavin Ross 2022)](https://www.essoar.org/doi/10.1002/essoar.10511742.1)