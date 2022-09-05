---
title: "Object classification, image recognition"
---

> See: 
> - [[AI/Deep learning/CNNs]]
> - [[AI/Computer Vision/Object detection]]
> - [[AI/Computer Vision/Semantic segmentation]]
> - [[AI/Deep learning/Residual and dense neural networks]]

## Resources
- https://cv-tricks.com/cnn/understand-resnet-alexnet-vgg-inception/
- https://blog.paralleldots.com/data-science/must-read-path-breaking-papers-about-image-classification/

## References
- #PAPER [AlexNet: ImageNet Classification with Deep Convolutional Neural Networks (2012)](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks)
	- This architecture was one of the first deep networks to push ImageNet Classification accuracy by a significant stride in comparison to traditional methodologies. It is composed of 5 convolutional layers followed by 3 fully connected layers.
	- AlexNet, proposed by Alex Krizhevsky, uses ReLu(Rectified Linear Unit) for the non-linear part, instead of a Tanh or Sigmoid function which was the earlier standard for traditional neural networks. Another problem that this architecture solved was reducing the over-fitting by using a Dropout layer after every FC layer.
- #PAPER [Visualizing and Understanding Convolutional Networks (Zeiler and Fergus 2013)](https://arxiv.org/abs/1311.2901)
- #PAPER [Very Deep Convolutional Networks for Large-Scale Image Recognition, VGG16 (Symonian 2014)](https://arxiv.org/abs/1409.1556)
	- This architecture is from VGG group, Oxford. It makes the improvement over AlexNet by replacing large kernel-sized filters (11 and 5 in the first and second convolutional layer, respectively) with multiple 3X3 kernel-sized filters one after another.
- #PAPER [Going Deeper with Convolutions (Szegedy 2015)](https://ai.google/research/pubs/pub43022)
	- GoogLeNet (Inception-V1, 2015)
	- http://nicolovaligi.com/history-inception-deep-learning-architecture.html
	- GoogLeNet devised a module called inception module that approximates a sparse CNN with a normal dense construction(shown in the figure). Since only a small number of neurons are effective as mentioned earlier, the width/number of the convolutional filters of a particular kernel size is kept small. Also, it uses convolutions of different sizes to capture details at varied scales(5X5, 3X3, 1X1). Another salient point about the module is that it has a so-called bottleneck layer(1X1 convolutions in the figure). It helps in the massive reduction of the computation requirement. Another change that GoogLeNet made, was to replace the fully-connected layers at the end with a simple global average pooling which averages out the channel values across the 2D feature map, after the last convolutional layer. 
- #PAPER See Resnet in [Residual and dense neural networks](AI/Deep%20learning/Residual%20and%20dense%20neural%20networks.md)
- #PAPER See Resnext in [Residual and dense neural networks](AI/Deep%20learning/Residual%20and%20dense%20neural%20networks.md)
- #PAPER See Densenet in [Residual and dense neural networks](AI/Deep%20learning/Residual%20and%20dense%20neural%20networks.md)
- #PAPER [SqueezeNet: AlexNet-level accuracy with 50x fewer parameters and <0.5MB model size (Iandola 2016)](https://arxiv.org/abs/1602.07360)
	- [Paper explained](https://www.youtube.com/watch?v=ge_RT5wvHvY )
	- https://towardsdatascience.com/squeeze-and-excitation-networks-9ef5e71eacd7
- #PAPER See SENets in [CNNs](AI/Deep%20learning/CNNs.md)
- #PAPER [Aggregated Residual Transformations for Deep Neural Networks (Xie 2017)](https://arxiv.org/abs/1611.05431)
	- #CODE https://github.com/taki0112/SENet-Tensorflow
- #PAPER [Local Relation Networks for Image Recognition (Hu 2019)](https://arxiv.org/abs/1904.11491)
- #PAPER [Designing Network Design Spaces (Radosavovic 2020)](https://arxiv.org/abs/2003.13678v1)
- #PAPER [NFNets. High-Performance Large-Scale Image Recognition Without Normalization (Brock 2021)](https://arxiv.org/abs/2102.06171)
	- #CODE https://github.com/deepmind/deepmind-research/tree/master/nfnets
	- https://towardsdatascience.com/deepmind-releases-a-new-state-of-the-art-image-classification-model-nfnets-75c0b3f37312
- #PAPER [Patches Are All You Need? (2021)](https://openreview.net/forum?id=TVHS5Y4dNvM)
	- #CODE https://github.com/tmp-iclr/convmixer
	- https://syncedreview.com/2021/10/12/deepmind-podracer-tpu-based-rl-frameworks-deliver-exceptional-performance-at-low-cost-121/
- #PAPER [CoAtNet: Marrying Convolution and Attention for All Data Sizes (Dai 2021)](https://arxiv.org/abs/2106.04803)
	- https://ai.googleblog.com/2021/09/toward-fast-and-accurate-neural.html
	- https://analyticsindiamag.com/a-guide-to-coatnet-the-combination-of-convolution-and-attention-networks/
