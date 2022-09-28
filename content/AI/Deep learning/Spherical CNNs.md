---
title: "Spherical CNNs"
---

> For computer vision and the natural sciences problems that require the analysis of spherical data, where representations may be learned efficiently by encoding equivariance to rotational symmetries

## Resources
- [Geometric Deep Learning for Spherical Data](https://towardsdatascience.com/geometric-deep-learning-for-spherical-data-55612742d05f)

## Code
- #CODE [DeepSphere](https://github.com/deepsphere)
	- Learning on the sphere (with a graph-based ConvNet). Used so far for cosmology, geophysics, 3D object recognition.

## References
- #PAPER [Spherical CNNs (Cohen 2018)](https://arxiv.org/pdf/1801.10130)
- #PAPER [Learning SO(3) Equivariant Representations with Spherical CNNs (Esteves 2018)](https://arxiv.org/pdf/1711.06721)
	- #TALK https://www.youtube.com/watch?v=Y86rzE4UzKs
	- #CODE https://github.com/daniilidis-group/spherical-cnn
- #PAPER [Spherical CNNs on unstructured grids (Jiang 2019)](https://arxiv.org/abs/1901.02039)
	- #CODE https://github.com/maxjiang93/ugscnn
	- Based on https://github.com/jonas-koehler/s2cnn
- #PAPER [Spherical convolution and other forms of informed machine learning for deep neural network based weather forecasts (Scher 2020)](https://arxiv.org/abs/2008.13524)
	- CNN-based weather forecasting solutions are are usually trained on atmospheric data represented as regular latitude-longitude grids, neglecting the curvature of the Earth
	- Showed the benefit of replacing the convolution operations with a spherical convolution operation, which takes into account the geometry of the underlying data, including correct representations near the poles
	- Additionally, studied the effect of including the information that the two hemispheres of the Earth have “flipped” properties - for example cyclones circulating in opposite directions - into the structure of the network
	- Using spherical convolution leads to an additional improvement in forecast skill, especially close to the poles in the first days of the forecast
	- The spherical convolution is implemented flexibly and scales well to high resolution datasets, but is still significantly more expensive than a standard convolution operation
	- See [[AI4ES/Weather forecasting, nowcasting]]
- #PAPER [DeepSphere: a graph-based spherical CNN (Defferrard 2020)](https://arxiv.org/abs/2012.15000) 
	- #CODE https://github.com/deepsphere
- #PAPER [Efficient Generalized Spherical CNNs (Cobb 2021)](https://arxiv.org/pdf/2010.11661)
	- https://towardsdatascience.com/efficient-generalized-spherical-cnns-1493426362ca