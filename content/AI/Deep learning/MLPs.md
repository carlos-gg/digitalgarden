---
title: "Multilayer perceptrons (MLPs)"
disableToc: false 
---

# Resources
- A multilayer perceptron (MLP) is a feed forward artificial neural network model that maps sets of input data onto a set of appropriate outputs. An MLP consists of multiple layers of nodes in a directed graph, with each layer fully connected to the next one. Except for the input nodes, each node is a neuron (or processing element) with a non linear activation function. 
- MLP utilizes a supervised learning technique called back propagation for training the network
- MLP is a modification of the standard linear perceptron and can distinguish data that is not linearly separable
- Multilayer Perceptron (MLP) vs Convolutional Neural Network in Deep Learning: https://medium.com/data-science-bootcamp/multilayer-perceptron-mlp-vs-convolutional-neural-network-in-deep-learning-c890f487a8f1

# Code
- #CODE MLP for MNIST: https://github.com/fchollet/keras/blob/master/examples/mnist_mlp.py
- #CODE Sklearn MLP implementation: 
	- https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html
	- https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html#sklearn.neural_network.MLPRegressor


# Perceptron
- History of the Perceptron: https://medium.com/@Jaconda/a-concise-history-of-neural-networks-2070655d3fec
- https://www.neuraldesigner.com/blog/perceptron-the-main-component-of-neural-networks
- https://fr.mathworks.com/help/nnet/ug/perceptron-neural-networks.html
- http://www.andreykurenkov.com/writing/a-brief-history-of-neural-nets-and-deep-learning/
- http://sebastianraschka.com/Articles/2015_singlelayer_neurons.html


# MLPs for vision and language
- #PAPER MLP-Mixer: An all-MLP Architecture for Vision (Tolstikhin 2021): https://arxiv.org/abs/2105.01601v2
	- #CODE https://paperswithcode.com/paper/mlp-mixer-an-all-mlp-architecture-for-vision?from=n9
	- CNNs are widely regarded as the go-to model for dealing with computer vision tasks. Attention-based architectures have also emerged as promising approaches that produce good performance on a variety of vision tasks. Despite this trend and the successes of attention and CNN architectures, this paper proposes a simple alternative architecture, MLP-Mixer, based on multi-layer perceptions, that produces competitive results on image classification benchmarks
	- MLP-Mixer contains two types of layers. One layer of MLPs applied independently to image patches and another layer of MLPs applied across patches. These layers achieve the effect of mixing per-location features and mixing spatial information, respectively 
	- MLP-Mixer achieves competitive results on the ImageNet benchmark
- #PAPER RepMLP: Re-parameterizing Convolutions into Fully-connected Layers for Image Recognition (Ding 2021): https://arxiv.org/abs/2105.01883v1
	- #CODE https://github.com/DingXiaoH/RepMLP
- #PAPER ResMLP: Feedforward networks for image classification with data-efficient training (Touvron 2021): https://arxiv.org/abs/2105.03404
- #PAPER Pay Attention to MLPs (Liu 2021): https://arxiv.org/abs/2105.08050v2
	- #CODE https://paperswithcode.com/paper/pay-attention-to-mlps?from=n10
	- https://www.infoq.com/news/2021/10/google-mlp-vision-language/
	- Researchers at Google Brain have announced Gated Multi-Layer Perceptron (gMLP), a deep-learning model that contains only basic multi-layer perceptrons
	- gMLP aims to show that these simplified architectures can perform as well as Transformers on key vision and language applications. According to the authors, the results and comparisons show that attention is not critical for Vision Transformers
	- In fine-tuning tasks, gMLP can close the gap on Transformers by simply making the model substantially larger
	- gMLP can scale as well as Transformers over increased data and compute
- #PAPER MAXIM: Multi-Axis MLP for Image Processing (Tu 2022): https://arxiv.org/abs/2201.02973v1
	- #CODE https://paperswithcode.com/paper/maxim-multi-axis-mlp-for-image-processing?from=n23
