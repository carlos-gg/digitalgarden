---
title: "Residual and dense neural networks"
disableToc: false 
---

- https://en.wikipedia.org/wiki/Residual_neural_network
- Training and investigating Residual Nets: http://torch.ch/blog/2016/02/04/resnets.html

- #PAPER Deep Residual Learning for Image Recognition, Resnet-50 (He 2015): http://arxiv.org/abs/1512.03385 ^resnet
	- #CODE https://github.com/raghakot/keras-resnet
	- https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf
	- Explained paper: https://www.youtube.com/watch?v=GWt6Fu05voI
	- Deep convolutional neural networks have led to a series of breakthroughs for image classification. Many other visual recognition tasks have also greatly benefited from very deep models. So, over the years there is a trend to go more deeper, to solve more complex tasks and to also increase /improve the classification/recognition accuracy. But, as we go deeper; the training of neural network becomes difficult and also the accuracy starts saturating and then degrades also. Residual Learning tries to solve both these problems.
	- What is Residual Learning?
		- In general, in a deep convolutional neural network, several layers are stacked and are trained to the task at hand. The network learns several low/mid/high level features at the end of its layers. In residual learning, instead of trying to learn some features, we try to learn some residual. Residual can be simply understood as subtraction of feature learned from input of that layer. ResNet does this using shortcut connections (directly connecting input of nth layer to some (n+x)th layer. It has proved that training this form of networks is easier than training simple deep convolutional neural networks and also the problem of degrading accuracy is resolved.
		- The architecture is similar to the VGGNet consisting mostly of 3X3 filters. From the VGGNet, shortcut connection as described above is inserted to form a residual network.
- #PAPER Aggregated Residual Transformations for Deep Neural Networks, ResNeXt (Xie 2016): https://arxiv.org/abs/1611.05431 ^resnext
- #PAPER Densely Connected Convolutional Networks, DenseNet (Huang 2016): https://arxiv.org/abs/1608.06993 ^densenet
	- #CODE https://github.com/liuzhuang13/DenseNet
	- #BOOK DenseNet: https://d2l.ai/chapter_convolutional-modern/densenet.html
	- For each layer, the feature-maps of all preceding layers are used as inputs, and its own feature-maps are used as inputs into all subsequent layers. DenseNets have several compelling advantages such as alleviating the vanishing-gradient problem, strengthening the feature propagation, encouraging feature reuse, and substantially reducing the number of parameters. DenseNets outperformed ResNets whilst requiring less memory and computation to achieve high performance.
	- https://towardsdatascience.com/review-densenet-image-classification-b6631a8ef803
	- In DenseNet, each layer obtains additional inputs from all preceding layers and passes on its own feature-maps to all subsequent layers. Concatenation is used (while element-wise addition for ResNets). Each layer is receiving a “collective knowledge” from all preceding layers. 
	- https://arthurdouillard.com/post/densenet/
- #PAPER Wide Residual Networks (Zagoruyko 2016): https://arxiv.org/abs/1605.07146
	- #CODE https://github.com/szagoruyko/wide-residual-networks
- #PAPER Residual Attention Network for Image Classification (Wang 2017): https://arxiv.org/abs/1704.06904
	- Residual Attention Network, a convolutional neural network using attention mechanism which can incorporate with state-of-art feed forward network architecture in an end-to-end training fashion. The attention residual learning is used to train very deep Residual Attention Networks which can be easily scaled up to hundreds of layers.
- #PAPER ResNet strikes back: An improved training procedure in timm (Wightman 2021): https://arxiv.org/abs/2110.00476
	- Paper explained: https://www.youtube.com/watch?v=Gl0s0GDqN3c
