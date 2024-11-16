---
title: "Causality"
---
> See:
> - [[Causal Inference]]
> - [[AI/Generative AI/LLMs#Causality and LLMs]]
> - [[Causality for time series]]
> - [[AI/Causality/Uplift modelling|Uplift modelling]]

## Resources
- [Causal Data Science Meeting - Home](https://www.causalscience.org/)
- [To Build Truly Intelligent Machines, Teach Them Cause and Effect](https://www.quantamagazine.org/to-build-truly-intelligent-machines-teach-them-cause-and-effect-20180515/)
- [Representing uncertain knowledge](https://glouppe.github.io/info8006-introduction-to-ai/?p=lecture5.md)
- [Reasoning over time](https://glouppe.github.io/info8006-introduction-to-ai/?p=lecture7.md)
- [Making decisions](https://glouppe.github.io/info8006-introduction-to-ai/?p=lecture8.md)
- [Causal Analysis Introduction - Examples in Python and PyMC](https://engl.is/causal-analysis-introduction-examples-in-python-and-pymc.html)
- [Causal Python: Five Novel Causal Ideas At NeurIPS 2023 | by Aleksander Molak | Towards Data Science](https://towardsdatascience.com/causal-python-five-novel-causal-ideas-at-neurips-2023-13bb68c5ed56)
- [The Causal AI Revolution is Underway | causaLens](https://causalens.com/resources/white-papers/the-causal-ai-revolution-is-happening-now/?utm_campaign=dataiku_survey&utm_medium=email&_hsmi=282014311&_hsenc=p2ANqtz-_ogV50Zs5vEL3AEFtV-ZNneyen2n0Rv8UjjkrXsqG4keU8mlZPpIUf9OJ3J8trMI8F9_blSkIUd53nM8OpoAqM8rOD7nFv86QCXT52_S5Zc96pOHI&utm_source=newsletter)
    - Causality is one of the key missing ingredients that’s needed to unlock real progress in AI. This is fast becoming the consensus view, within academia and industry
    - An appreciation of cause and effect is a necessary requirement for true intelligence
    - Counterfactual analysis has enormous transformative potential beyond healthcare, not least for AI in finance and business

## Talks
- #TALK [Human-Guided Causal Discovery - getting out of the black box of correlation based ML - YouTube](https://www.youtube.com/watch?v=mxpbMD56OS4)
	- CausaLens - DecisionOS
	- AI and data science with humans in the loop, more trustworthy
	- Correlation-based ML is not enough, no reasoning or causality
	- Predicting an outcome is not enough, we need to understand the underlying causal drivers
- #TALK [Interview - Causal Reasoning, Counterfactuals, and the Path to AGI (Judea Pearl)](https://www.youtube.com/watch?v=pEBI0vF45ic)
- #TALK Causality, Bernhard Schölkopf and Stefan Bauer, MLSS 2020: 
	- [Part I](https://www.youtube.com/watch?v=btmJtThWmhA&feature=youtu.be)
		- https://drive.google.com/file/d/1qlUYuU7wfoD6C8Qo0x4Eyz5aT2k0B_jC/view
	- [Part II](https://www.youtube.com/watch?v=9DJWJpn0DmU&feature=youtu.be)
		- https://drive.google.com/file/d/1_-bUoyY-Thfqu1ac4EwBSv6cCoS-qtnn/view
- #TALK [Yoshua Bengio Guest Talk - Towards Causal Representation Learning](https://www.youtube.com/watch?v=rKZJ0TJWvTk)
- #TALK [Lightning Talk: Deep Causal Learning - YouTube](https://www.youtube.com/watch?v=n02vx2mDg0M&ab_channel=MicrosoftResearch)
- #TALK [UCL Seminar - What is Causal AI - YouTube](https://www.youtube.com/watch?v=50VGblsPNQM&ab_channel=causaLens)
	- How to infer a causal DAG?
	    - randomized controlled trial (RCT), AB tests
	    - causal discovery upon observational data
	    - apply domain knowledge and human context
	- Causal discovery = Data + some human context
	- Conditional independence based causal discovery methods: PC, FCI
	- Estimating treatment effect (Do calculus)
	    - Instrumental variables
	    - Propensity score matching
	    - Doubly robust estimators
	    - backdoor/frontdoor adjustment criterion

## Code
- #CODE [Causalai (Salesforce)](https://github.com/salesforce/causalai) - A Fast and Scalable framework for Causal Analysis of Time Series and Tabular Data
	- https://opensource.salesforce.com/causalai/latest/index.html
- #CODE [Causalml](https://github.com/uber/causalml)
- #CODE [Causality - Tools for causal analysis](https://github.com/akelleh/causality)
	- https://medium.com/@akelleh/causal-inference-with-pandas-dataframes-fc3e64fce5d
- #CODE [CausalImpact (for R)](https://google.github.io/CausalImpact/)
- #CODE [tfcausalimpact - Google's Causal Impact Algorithm Implemented on Top of TensorFlow Probability](https://github.com/WillianFuks/tfcausalimpact)
	- https://towardsdatascience.com/implementing-causal-impact-on-top-of-tensorflow-probability-c837ea18b126


## Courses
- #COURSE [Machine Learning & Causal Inference: A Short Course | Stanford Graduate School of Business](https://www.gsb.stanford.edu/faculty-research/labs-initiatives/sil/research/methods/ai-machine-learning/short-course)

## References
- #PAPER [Causal inference with multiple time series: principles and problems (2013)](https://royalsocietypublishing.org/doi/10.1098/rsta.2011.0613)
- #PAPER [Towards a Learning Theory of Cause-Effect Inference (Lopez-Paz 2015)](https://arxiv.org/abs/1502.02398)
- #PAPER [Unsupervised Discovery of El Nino Using Causal Feature Learning on Microlevel Climate Data (Chalupka 2016)](https://arxiv.org/abs/1605.09370)
- #PAPER [Comparative Benchmarking of Causal Discovery Techniques (Singh 2017)](https://arxiv.org/abs/1708.06246)
- #PAPER [A Physics-Based Approach to Unsupervised Discovery of Coherent Structures in Spatiotemporal Systems (Rupe 2017)](https://arxiv.org/abs/1709.03184) 
- #PAPER #REVIEW [A Primer on Causal Analysis (2018)](https://arxiv.org/abs/1806.01488)
- #PAPER [DAGs with NO TEARS: Continuous Optimization for Structure Learning (Zheng 2018)](https://arxiv.org/abs/1803.01422)
	- #CODE https://github.com/xunzheng/notears
- #PAPER [Local causal states and discrete coherent structures (Rupe 2018)](https://aip.scitation.org/doi/10.1063/1.5021130) 
- #PAPER [Learning Functional Causal Models with Generative Neural Networks (Goudet 2018)](https://arxiv.org/abs/1709.05321)
- #PAPER [Variable-lag Granger Causality for Time Series Analysis (2019)](https://arxiv.org/abs/1912.10829)
- #PAPER [Learning Sparse Nonparametric DAGs (Zheng 2020)](https://arxiv.org/abs/1909.13189)
	- #CODE https://github.com/xunzheng/notears
	- #CODE https://github.com/jmoss20/notears
- #PAPER [When causal inference meets deep learning (Luo 2020)](https://www.nature.com/articles/s42256-020-0218-x)
	- Learning causal relations, rather than correlations, is a fundamental problem in both statistical Machine Learning and computer sciences
	- Bayesian networks (BNs) can capture causal relations, but learning such a network from data is NP-hard
	- Recent work has made it possible to approximate this problem as a continuous optimization task that can be solved efficiently with well-established numerical techniques
	- BNs encode the conditional independencies between variables using directed acyclic graphs (DAGs)
- #PAPER [Spacetime Autoencoders Using Local Causal States (Rupe 2020)](https://arxiv.org/abs/2010.05451)
	- #CODE https://github.com/adamrupe/spacetime_autoencoders
	- Local causal states are latent representations that capture organized pattern and structure in complex spatiotemporal systems
	- We expand their functionality, framing them as space-time autoencoders
- #PAPER [Algorithms for Causal Reasoning in Probability Trees (Genewein 2020)](https://arxiv.org/abs/2010.12237)
	- #CODE https://github.com/deepmind/deepmind-research/tree/master/causal_reasoning
	- https://syncedreview.com/2020/10/29/deepmind-introduces-algorithms-for-causal-reasoning-in-probability-trees/
- #PAPER [Off-the-shelf deep learning is not enough, and requires parsimony, Bayesianity, and causality (Vasudevan 2021)](https://www.nature.com/articles/s41524-020-00487-0)
- #PAPER [Towards Causal Representation Learning (Schölkopf 2021)](https://arxiv.org/abs/2102.11107)
- #PAPER [Causal Machine Learning: A Survey and Open Problems (2022)](https://arxiv.org/pdf/2206.15475)
- #PAPER [Salesforce CausalAI Library: A Fast and Scalable Framework for Causal Analysis of Time Series and Tabular Data (Arpit 2023)](https://arxiv.org/pdf/2301.10859)
	- [CausalAI: Answering Causality Questions Using Observational Data](https://blog.salesforceairesearch.com/causalai/)


