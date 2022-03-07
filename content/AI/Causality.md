---
title: "Causality"
disableToc: false 
---

# Resources
- To Build Truly Intelligent Machines, Teach Them Cause and Effect: https://www.quantamagazine.org/to-build-truly-intelligent-machines-teach-them-cause-and-effect-20180515/
- Representing uncertain knowledge: https://glouppe.github.io/info8006-introduction-to-ai/?p=lecture5.md
- Reasoning over time: https://glouppe.github.io/info8006-introduction-to-ai/?p=lecture7.md
- Making decisions: https://glouppe.github.io/info8006-introduction-to-ai/?p=lecture8.md
- Causal Analysis Introduction - Examples in Python and PyMC: https://engl.is/causal-analysis-introduction-examples-in-python-and-pymc.html
- Granger causality: 
	- https://en.wikipedia.org/wiki/Granger_causality
	- The Granger causality test is a statistical hypothesis test for determining whether one time series is useful in forecasting another, first proposed in 1969
	- Granger causality is a fundamental technique for causal inference in time series data, commonly used in the social and biological sciences
- PCMCI:
	- https://jakobrunge.github.io/tigramite/#tigramite-pcmci-pcmci
	- PCMCI causal discovery for time series datasets. It is a 2-step causal discovery method for large-scale time series datasets. The first step is a condition-selection followed by the MCI conditional independence test.

- #TALK Interview - Causal Reasoning, Counterfactuals, and the Path to AGI (Judea Pearl): https://www.youtube.com/watch?v=pEBI0vF45ic
- #TALK Causality, Bernhard Schölkopf and Stefan Bauer, MLSS 2020: 
	- Part I: https://www.youtube.com/watch?v=btmJtThWmhA&feature=youtu.be
		- https://drive.google.com/file/d/1qlUYuU7wfoD6C8Qo0x4Eyz5aT2k0B_jC/view
	- Part II: https://www.youtube.com/watch?v=9DJWJpn0DmU&feature=youtu.be
		- https://drive.google.com/file/d/1_-bUoyY-Thfqu1ac4EwBSv6cCoS-qtnn/view


# Code
- #CODE Causality - Tools for causal analysis: https://github.com/akelleh/causality
	- https://medium.com/@akelleh/causal-inference-with-pandas-dataframes-fc3e64fce5d
- #CODE CausalImpact (for R): https://google.github.io/CausalImpact/
- #CODE tfcausalimpact - Google's Causal Impact Algorithm Implemented on Top of TensorFlow Probability: https://github.com/WillianFuks/tfcausalimpact
	- https://towardsdatascience.com/implementing-causal-impact-on-top-of-tensorflow-probability-c837ea18b126
  
  # References
- #PAPER Causal inference with multiple time series: principles and problems (2013): https://royalsocietypublishing.org/doi/10.1098/rsta.2011.0613
- #PAPER Towards a Learning Theory of Cause-Effect Inference (Lopez-Paz 2015): https://arxiv.org/abs/1502.02398
- #PAPER Unsupervised Discovery of El Nino Using Causal Feature Learning on Microlevel Climate Data (Chalupka 2016): https://arxiv.org/abs/1605.09370
- #PAPER Comparative Benchmarking of Causal Discovery Techniques (Singh 2017): https://arxiv.org/abs/1708.06246
- #PAPER A Physics-Based Approach to Unsupervised Discovery of Coherent Structures in Spatiotemporal Systems (Rupe 2017): https://arxiv.org/abs/1709.03184 ^rupe17
- #PAPER A Primer on Causal Analysis (2018): https://arxiv.org/abs/1806.01488
- #PAPER DAGs with NO TEARS: Continuous Optimization for Structure Learning (Zheng 2018): https://arxiv.org/abs/1803.01422
	- #CODE https://github.com/xunzheng/notears
- #PAPER Local causal states and discrete coherent structures (Rupe 2018): https://aip.scitation.org/doi/10.1063/1.5021130 ^f00b92
	- see [[#^rupe17]]
- #PAPER Learning Functional Causal Models with Generative Neural Networks (Goudet 2018): https://arxiv.org/abs/1709.05321
- #PAPER Variable-lag Granger Causality for Time Series Analysis (2019): https://arxiv.org/abs/1912.10829
- #PAPER Learning Sparse Nonparametric DAGs (Zheng 2020): https://arxiv.org/abs/1909.13189
	- #CODE https://github.com/xunzheng/notears
	- #CODE https://github.com/jmoss20/notears
- #PAPER When causal inference meets deep learning (Luo 2020): https://www.nature.com/articles/s42256-020-0218-x
	- Learning causal relations, rather than correlations, is a fundamental problem in both statistical [[Machine Learning]] and computer sciences
	- Bayesian networks (BNs) can capture causal relations, but learning such a network from data is NP-hard
	- Recent work has made it possible to approximate this problem as a continuous optimization task that can be solved efficiently with well-established numerical techniques
	- BNs encode the conditional independencies between variables using directed acyclic graphs (DAGs)
- #PAPER Spacetime Autoencoders Using Local Causal States (Rupe 2020): https://arxiv.org/abs/2010.05451
	- #CODE https://github.com/adamrupe/spacetime_autoencoders
	- Local causal states are latent representations that capture organized pattern and structure in complex spatiotemporal systems
	- We expand their functionality, framing them as space-time autoencoders
- #PAPER Algorithms for Causal Reasoning in Probability Trees (Genewein 2020): https://arxiv.org/abs/2010.12237
	- #CODE https://github.com/deepmind/deepmind-research/tree/master/causal_reasoning
	- https://syncedreview.com/2020/10/29/deepmind-introduces-algorithms-for-causal-reasoning-in-probability-trees/
- #PAPER Off-the-shelf deep learning is not enough, and requires parsimony, Bayesianity, and causality (Vasudevan 2021): https://www.nature.com/articles/s41524-020-00487-0



