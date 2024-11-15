---
title: "Neural processes"
---

> A Neural Process (NP) is a map from a set of observed input-output pairs to a predictive distribution over functions, which is designed to mimic other stochastic processes' inference mechanisms. NPs define distributions over functions, are capable of rapid adaptation to new observations, and can estimate the uncertainty in their predictions

## Resources
- [The Neural Process Family](https://yanndubs.github.io/Neural-Process-Family/text/Intro.html)
- [Conditional Neural Process](https://yanndubs.github.io/Neural-Process-Family/reproducibility/CNP.html)

## Code
- #CODE [Neuralprocesses](https://github.com/wesselb/neuralprocesses) - A framework for composing Neural Processes in Python
	- https://wesselb.github.io/neuralprocesses/intro.html

## References
- #PAPER [Neural Processes (Garnelo 2018)](https://arxiv.org/pdf/1807.01622)            
- #PAPER [Conditional Neural Processes (Garnelo 2018)](https://arxiv.org/abs/1807.01613)
- #PAPER [Residual Neural Processes (Lee 2020)](https://ojs.aaai.org//index.php/AAAI/article/view/5883)
- #PAPER [Convolutional Conditional Neural Processes (Gordon 2020)](https://arxiv.org/abs/1910.13556)
	- #CODE https://github.com/cambridge-mlg/convcnp
	- https://yanndubs.github.io/Neural-Process-Family/reproducibility/ConvCNP.html
	- See [[AI/Deep learning/CNNs]]
- #PAPER [The Gaussian Neural Process (Bruinsma 2021)](https://arxiv.org/pdf/2101.03606)            
- #PAPER [GP-ConvCNP: Better Generalization for Convolutional Conditional Neural Processes on Time Series Data (Petersen 2021)](https://arxiv.org/pdf/2106.04967)            
	- #CODE https://github.com/MIC-DKFZ/gpconvcnp
- #PAPER [Conditional Temporal Neural Processes with Covariance Loss (Yoo 2021)](http://proceedings.mlr.press/v139/yoo21b.html)
- #PAPER [Contrastive Conditional Neural Processes (Ye 2022)](https://arxiv.org/abs/2203.03978)
	- Conditional Neural Processes (CNPs) bridge neural networks with probabilistic inference to approximate functions of Stochastic Processes under meta-learning settings
	- Proposed to equip CNPs by 1) aligning prediction with encoded ground-truth observation, and 2) decoupling metarepresentation adaptation from generative reconstruction
- #PAPER #REVIEW [The Neural Process Family: Survey, Applications and Perspectives (Jha 2022)](https://arxiv.org/abs/2209.00517)