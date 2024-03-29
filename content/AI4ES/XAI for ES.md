---
title: "XAI for Earth Sciences"
---

> See:
> - [[AI/XAI]]
> - [[AI4ES/Causal modeling in ES]]


## References
- #PAPER [Making the Black Box More Transparent: Understanding the Physical Implications of Machine Learning (McGovern et al. 2019)](https://journals.ametsoc.org/bams/article/100/11/2175/343787/Making-the-Black-Box-More-Transparent)
- #PAPER [Physically Interpretable Neural Networks for the Geosciences: Applications to Earth System Variability (Toms 2020)](https://arxiv.org/abs/1912.01752)
	- Showed that the interpretation of neural networks can enable the discovery of scientifically meaningful connections within geoscientific data
	- Used two methods for neural network interpretation: backwards optimization and LRP. Both project the decision pathways of a network back onto the original input dimensions
- #PAPER [Indicator patterns of forced change learned by an artificial neural network (Barnes 2020)](https://www.semanticscholar.org/paper/Indicator-patterns-of-forced-change-learned-by-an-Barnes-Toms/38018254d806f18352f2f3702380c18403aeef35)
- #PAPER [Evaluation, Tuning and Interpretation of Neural Networks for Meteorological Applications (Ebert-Uphoff 2020)](https://www.semanticscholar.org/paper/Evaluation%2C-Tuning-and-Interpretation-of-Neural-for-Ebert-Uphoff-Hilburn/b31e4e9d6ba87a8e709d743b1e96a18c8dd0bbf6)
- #PAPER [Detecting climate signals using explainable AI with single-forcing large ensembles (Labe 2021)](https://www.essoar.org/doi/10.1002/essoar.10505762.1)
- #PAPER [Using Machine Learning to Analyze Physical Causes of Climate Change: A Case Study of U.S. Midwest Extreme Precipitation (Davenport 2021)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021GL093787)
	- use a neural network to predict extreme precipitation from daily sea level pressure and 500-hPa geopotential height fields
	- CNN 2 layers to predict extreme precipitation (p95) based on the average precipitation over a rectangular region covering the Upper Mississippi Watershed and the eastern portion of the Missouri Watershed
	- use daily mean sea level pressure (SLP) and 500-hPa geopotential height (GPH) anomalies calculated from the NCEP/NCAR-R1 reanalysis, 2.5 deg resolution on a larger spatial domain that covers the continental U.S. and surrounding oceans
- #PAPER [Oceanic Harbingers of Pacific Decadal Oscillation Predictability in CESM2 Detected by Neural Networks (Gordon 2021)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2021GL095392)
- #POSTER [Mapped-PCMCI: an algorithm for causal discovery at the grid level (Tibau Alberdi 2021)](https://meetingorganizer.copernicus.org/EGU21/EGU21-5633.html)
- #PAPER [Assessing Decadal Predictability in an Earth-System Model Using Explainable Neural Networks (Toms 2021)](https://agupubs.onlinelibrary.wiley.com/doi/epdf/10.1029/2021GL093842)
- #PAPER [Predicting Slowdowns in Decadal Climate Warming Trends With Explainable Neural Networks (Labe 2022)](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022GL098173)
- #PAPER [Investigating the fidelity of explainable artificial intelligence methods for applications of convolutional neural networks in geoscience (Mamalakis 2022)](https://arxiv.org/abs/2202.03407)
- #PAPER [Neural network attribution methods for problems in geoscience: A novel synthetic benchmark dataset (Mamalakis 2022)](https://www.cambridge.org/core/journals/environmental-data-science/article/neural-network-attribution-methods-for-problems-in-geoscience-a-novel-synthetic-benchmark-dataset/DDA562FC7B9A2B30710582861920860E)
	- #CODE https://github.com/amamalak/Neural-Network-Attribution-Benchmark-for-Regression