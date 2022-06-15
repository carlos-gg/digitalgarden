---
title: "(Earth system model) Emulators and surrogates"
---

> See:
> - [[Parameterizations]]

## Resources
- [Earth system modelling](https://www.climateurope.eu/earth-system-modeling-a-definition/)
	- Earth system models (ESM) seek to simulate all relevant aspects of the Earth system. They include physical, chemical and biological processes, therefore reaching far beyond their predecessors, the global climate models (GCM), which just represented the physical atmospheric and oceanic processes.
	- At their core ESMs have the atmospheric and ocean components of a GCM however to this they add representations of the global carbon cycle, dynamic vegetation, atmospheric chemistry, ocean bio-geo-chemistry and even continental ice sheets.
- [What is an Earth System Model (ESM)?](https://soccom.princeton.edu/content/what-earth-system-model-esm)
	- A coupled climate model is a computer code that estimates the solution to differential equations of fluid motion and thermodynamics to obtain time and space dependent values for temperature, winds and currents, moisture and/or salinity and pressure in the atmosphere and ocean. 


## References
- #PAPER [Efficient surrogate modeling methods for large-scale Earth system models based on machine-learning techniques (Lu 2018)](https://gmd.copernicus.org/articles/12/1791/2019/)
	- Proposed an efficient surrogate method capable of using a few ESM runs to build an accurate and fast-to-evaluate surrogate system of model outputs over large spatial and temporal domains. 
	- SVD to reduce the output dimensions and then use Bayesian optimization techniques to generate an accurate neural network surrogate model based on limited ESM simulation samples. 
	- Our [[Machine Learning]] -based surrogate methods can build and evaluate a large surrogate system of many variables quickly
- #PAPER [Toward Data‐Driven Weather and Climate Forecasting: Approximating a Simple General Circulation Model With Deep Learning (Scher 2018)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2018GL080704)
	- Emulated the dynamics of a simple general circulation model with a deep neural network. After being trained on the model, the network can predict the complete model state several time steps ahead—which conceptually is making weather forecasts in the model world
- #PAPER [Weather and climate forecasting with neural networks: using general circulation models (GCMs) with different complexity as a study ground (Scher 2019)](https://gmd.copernicus.org/articles/12/2797/2019/)
- #PAPER [Deep learning for physical processes: incorporating prior scientific knowledge (Bezenac 2019)](https://iopscience.iop.org/article/10.1088/1742-5468/ab3195)
- #PAPER [Emulating Numeric Hydroclimate Models with Physics-Informed conditions [[GANs]] (Manepalli, 2019)](https://par.nsf.gov/servlets/purl/10137369)
	- https://slideslive.com/38922409/emulating-numeric-hydroclimate-models-with-physicsinformed-cgans 
- #PAPER [Achieving Conservation of Energy in Neural Network Emulators for Climate Modeling (Beucler 2019)](https://arxiv.org/abs/1906.06622)
	- NN models do not intrinsically conserve energy and mass, which is an obstacle to using them for long-term climate predictions. 
	- Proposed two methods to enforce linear conservation laws in neural-network emulators of physical models: Constraining (1) the loss function or (2) the architecture of the network itself. 
	- Applied to the emulation of explicitly-resolved cloud processes in a prototype multi-scale climate model, we show that architecture constraints can enforce conservation laws to satisfactory numerical precision, while all constraints help the neural-network better generalize to conditions outside of its training set, such as global warming.
- #PAPER [Deep Learning for Precipitation Estimation from Satellite and Rain Gauges Measurements (Moraux, 2019)](https://www.mdpi.com/2072-4292/11/21/2463/htm)
	- This paper proposes a multimodal and multi-task deep-learning model for instantaneous precipitation rate estimation. 
	- Using both thermal infrared satellite radiometer and automatic rain gauge measurements as input, our encoder–decoder convolutional neural network performs a multiscale analysis of these two modalities to estimate simultaneously the rainfall probability and the precipitation rate value.
- #PAPER DeepClimGAN: A High-Resolution Climate Data Generator (Puchko 2019): 
	- https://www.semanticscholar.org/paper/DeepClimGAN%3A-A-High-Resolution-Climate-Data-Puchko-Link/86b9db65ff46e8dfe0ee6e3fa8b5f16f5eee0735
	- #CODE https://github.com/JGCRI/DeepClimGAN
	- DeepClimGAN is a conditional GAN, capable of producing a spatio-temporal forecast
- #PAPER [Applying Machine Learning to Improve Simulations of a Chaotic Dynamical System Using Empirical Error Correction (Pag 2019)](https://europepmc.org/article/PMC/6618166)
	- #CODE https://github.com/PAGWatson/Lorenz96_and_neural_networks
	- Dynamical weather and climate prediction models underpin many studies of the Earth system and hold the promise of being able to make robust projections of future climate change based on physical laws
	- Simulations from these models still show many differences compared with observations
	- Tested a framework using machine learning together with physically-derived models, in which it is learnt how to correct the errors of the latter from time step to time step
	- This maintains the physical understanding built into the models, while allowing performance improvements, and also requires much simpler algorithms and less training data
	- This is tested in the context of simulating the chaotic Lorenz '96 system, and it is shown that the approach yields models that are stable and that give both improved skill in initialized predictions and better long-term climate statistics
- #PAPER [Up to two billion times acceleration of scientific simulations with deep neural architecture search (Kasim 2020)](https://arxiv.org/abs/2001.08055)
	- A promising route to accelerate simulations by building fast emulators with machine learning requires large training datasets, which can be prohibitively expensive to obtain with slow simulations. 
	- Presented a method based on neural architecture search to build accurate emulators even with a limited number of training data. 
	- The method successfully accelerates simulations by up to 2 billion times in 10 scientific cases including astrophysics, climate science, biogeochemistry, high energy density physics, fusion energy, and seismology, using the same super-architecture, algorithm, and hyperparameters
- #PAPER [DPM: A deep learning PDE augmentation method with application to large-eddy simulation (Sirignano 2020)](https://www.sciencedirect.com/science/article/pii/S0021999120305854)
	- https://techxplore.com/news/2020-11-method-physics-deep-simulate-turbulence.html
- #PAPER [Hybrid modeling: fusion of a deep learning approach and a physics-based model for global hydrological modeling (Kraft 2020)](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIII-B2-2020/1537/2020/)
	- Reichstein et al, physics-based ML
	- Presented an end-to-end hybrid modeling approach that learns and predicts spatial-temporal variations of observed and unobserved (latent) hydrological variables globally
- #PAPER [Enforcing statistical constraints in generative adversarial networks for modeling chaotic dynamical systems (Wu 2020)](https://www.sciencedirect.com/science/article/pii/S0021999119309143)
	- https://arxiv.org/abs/1905.06841
	- Confirmed statistics-conforming property of [[GANs]] for modeling dynamical systems
	- Highlighted the lack of robustness of GANs and need of explicit physical constraints
	- Improved training robustness of GANs by explicitly enforcing statistical constraints. Constraint on optimization with penalty  terms  added  into  the  optimization loss function of GANs (distance measure between two covariance structures, related to symmetrized Kullback–Leibler divergence) 
	- Demonstrated merits of statistics-informed GANs on modeling Rayleigh-Bénard convection
- #PAPER [Boosting performance in Machine Learning of Turbulent and Geophysical Flows via scale separation (Faranda 2020)](https://npg.copernicus.org/preprints/npg-2020-39/)
	- Uses [[RNNs#Echo state networks ESN]] for forecasting [[Weather forecasting, nowcasting]] dynamics of complex systems (sea level pressure data)
	- #TALK https://www.youtube.com/watch?v=qztvuflzNfQ
- #PAPER [Towards Physics-informed Deep Learning for Turbulent Flow Prediction (Wang 2020)](https://arxiv.org/abs/1911.08655)
	- Aimed to predict turbulent flow by learning its highly nonlinear dynamics from spatiotemporal velocity fields of large-scale fluid flow simulations of relevance to turbulence modeling and climate modeling
	- Introduced trainable spectral filters in a coupled model of Reynolds-averaged Navier-Stokes (RANS) and Large Eddy Simulation (LES), followed by a specialized U-net for prediction.
	- The turbulent-Flow Net (TF-Net), is grounded in a principled physics model, yet offers the flexibility of learned representations
- #TALK [Loosely Conditioned Emulation of Global Climate Models With Generative Adversarial Networks (Ayala 2020)](https://www.climatechange.ai/papers/neurips2020/61.html)
