---
title: "Probabilistic deep learning"
disableToc: false 
---

See:
- [Bayesian modelling](AI/Bayesian%20modelling.md)
- [GFlowNets](AI/Deep%20learning/GFlowNets.md)


## Resources
- [A Comprehensive Introduction to Bayesian Deep Learning](https://jorisbaan.nl/2021/03/02/introduction-to-bayesian-deep-learning.html)
- [Bayesian Neural Network tutorial](http://edwardlib.org/tutorials/bayesian-neural-network)
- [Bayesian Deep Learning - NeurIPS Workshop](http://bayesiandeeplearning.org/ )
- [Deep Learning Is Not Good Enough, We Need Bayesian Deep Learning for Safe AI](https://alexgkendall.com/computer_vision/bayesian_deep_learning_for_safe_ai/)
- [Making Your Neural Network Say “I Don’t Know” — Bayesian NNs using Pyro and PyTorch](https://towardsdatascience.com/making-your-neural-network-say-i-dont-know-bayesian-nns-using-pyro-and-pytorch-b1c24e6ab8cd)
- [Building a Bayesian deep learning classifier](https://towardsdatascience.com/building-a-bayesian-deep-learning-classifier-ece1845bc09)
- [Physics - a Gateway to Bayesian Deep Learning](https://github.com/henripal/sgld)
- [Bayesian deep learning with Fastai : how not to be uncertain about your uncertainty!](https://towardsdatascience.com/bayesian-deep-learning-with-fastai-how-not-to-be-uncertain-about-your-uncertainty-6a99d1aa686e)
	- BNNs are a way to add uncertainty handling in our models. The idea is simple, instead of having deterministic weights that we learn, we instead learn the parameters of a random variable which we will use to sample our weights during forward propagation. Then, to learn the parameters, we will use backpropagation, sometimes with a little trick to make our parameters differentiable.
	- Dropout is a way to make your Neural Networks Bayesian almost for free, and to use it during inference you just have to keep the Dropout, and sample several models, this is called MC Dropout.

 ### Monte Carlo Dropout
- [What is MC Dropout](https://datascience.stackexchange.com/questions/44065/what-is-monte-carlo-dropout)
- normal dropout (only at training time) serves as a regularization to avoid overfitting. During test time, dropout is not applied; instead, all nodes/connections are present, but the weights are adjusted accordingly (e.g. multiplied by the keep ratio, which is 1 - dropout_ratio). Such a model during test time can be understood as a *average* of an ensemble of neural networks.
- Notice that for normal dropout, at test time the prediction is *deterministic*. Without other source of randomness, given one test data point, the model will always predict the same label or value.
- For *Monte Carlo dropout*, the dropout is applied at both training and test time. At test time, the prediction is no longer deterministic, but depending on which nodes/links you randomly choose to keep. Therefore, given a same datapoint, your model could predict different values each time.
- The primary goal of MC dropout is to generate random predictions and interpret them as samples from a probabilistic distribution. 
- #TALK [Estimacion de la Incertidumbre en Redes Neuronales (Valdenegro)](https://mvaldenegro.github.io/files/DSRP-meetup-NeurIPS-2020-incertidumbre-redes-neuronales.pdf)


## Code
- #CODE [Pyro (Uber) - Deep universal probabilistic programming with Python and PyTorch](https://github.com/uber/pyro  )
	- http://pyro.ai
	- http://eng.uber.com/pyro
- #CODE [Blitz - Bayesian Layers in Torch Zoo](https://github.com/piEsposito/blitz-bayesian-deep-learning)
- #CODE [Bean machine (Meta/Facebook)](https://github.com/facebookresearch/beanmachine)
	- https://research.facebook.com/blog/2021/12/introducing-bean-machine-a-probabilistic-programming-platform-built-on-pytorch/
- #CODE Edwardlib - Edward is a Python library for probabilistic modeling, inference, and criticism
	- https://theintelligenceofinformation.wordpress.com/2017/06/02/pydata-london-2017-bayesian-deep-learning-talk-by-andrew-rowan/
	- #TALK https://www.youtube.com/watch?v=I09QVNrUS3Q
	- http://willwolf.io/2017/06/15/random-effects-neural-networks/
- #CODE [TensorFlow Probability](https://www.tensorflow.org/probability/)
	- https://towardsdatascience.com/bayesian-neural-networks-with-tensorflow-probability-fbce27d6ef6
- #CODE [keras-uncertainty](https://github.com/mvaldenegro/keras-uncertainty)
	- Monte Carlo Dropout (MC-Dropout)
	- Deep Ensembles

## Books
- #BOOK [Probabilistic Graphical Models: Principles and Techniques (Koller, 2009 MIT)](http://pgm.stanford.edu/ )
- #BOOK [Probabilistic Deep Learning - With Python, Keras and TensorFlow Probability (Durr, MANNING 2020)](https://www.manning.com/books/probabilistic-deep-learning)
	- https://tensorchiefs.github.io/dl_book/

## Courses
- #COURSE [Introductory course on probabilistic graphical models](https://ermongroup.github.io/cs228-notes/)

## References
- Review papers: 
	- #PAPER [A Survey of Uncertainty in Deep Neural Networks (Gawlikowski 2022)](https://arxiv.org/abs/2107.03342)

- #PAPER [Probabilistic machine learning and artificial intelligence (Ghahramani 2015)](https://www.nature.com/articles/nature14541)
- #PAPER [Dropout as a Bayesian Approximation:Representing Model Uncertainty in Deep Learning (Gal 2016)](https://arxiv.org/abs/1506.02142)
- #PAPER [Bayesian Neural Networks (Mullachery, 2018)](https://arxiv.org/abs/1801.07710)
- #PAPER [Deep Sub-Ensembles for Fast Uncertainty Estimation in Image Classification (Valdenegro-Toro 2019)](https://arxiv.org/abs/1910.08168)
- #PAPER [Bayesian Recurrent Neural Networks (Fortunato 2019)](https://arxiv.org/abs/1704.02798)
- #PAPER [Bayesian Deep Learning and a Probabilistic Perspective of Generalization (Gordon Wilson, 2020)](https://arxiv.org/abs/2002.08791)
	- https://github.com/izmailovpavel/understandingbdl
- #PAPER [Hands-on Bayesian Neural Networks - a Tutorial for Deep Learning Users (Jospin 2020)](https://arxiv.org/abs/2007.06823)
- #PAPER [DropConnect is effective in modeling uncertainty of Bayesian deep networks (Mobiny 2021)](https://www.nature.com/articles/s41598-021-84854-x)
	- #CODE https://github.com/hula-ai/mc_dropconnect
- #PAPER [Epistemic Neural Networks (Osband 2021)](https://arxiv.org/abs/2107.08924)
	- #CODE https://github.com/deepmind/enn
	- https://syncedreview.com/2021/07/26/deepmind-podracer-tpu-based-rl-frameworks-deliver-exceptional-performance-at-low-cost-69/
- #PAPER [Uncertainty Baselines: Benchmarks for Uncertainty & Robustness in Deep Learning (Nado 2021)](https://arxiv.org/abs/2106.04015)
	- https://ai.googleblog.com/2021/10/baselines-for-uncertainty-and.html
	- #CODE https://github.com/google/uncertainty-baselines
- #PAPER [Probabilistic Deep Learning with Probabilistic Neural Networks and Deep Probabilistic Models](https://arxiv.org/pdf/2106.00120)