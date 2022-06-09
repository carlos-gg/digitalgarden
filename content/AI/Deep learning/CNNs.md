---
title: "Convolutional Neural Networks (CNNs)"
---

> A convolutional neural network (CNN, or ConvNet) is a class of deep neural networks, most commonly applied to analyzing visual imagery. They are also known as shift invariant or space invariant artificial neural networks, based on their shared-weights architecture and translation invariance characteristics

## Resources 
- https://github.com/kjw0612/awesome-deep-vision
- https://en.wikipedia.org/wiki/Convolutional_neural_network
- [CNNs chapter in d2l.ai](https://d2l.ai/chapter_convolutional-neural-networks/index.html)
- [Convolutional Neural Networks cheatsheet](https://stanford.edu/~shervine/teaching/cs-230/cheatsheet-convolutional-neural-networks)
- http://cs231n.github.io/convolutional-networks/
- http://cs231n.github.io/understanding-cnn/
- https://neurdiness.wordpress.com/2018/05/17/deep-convolutional-neural-networks-as-models-of-the-visual-system-qa/
* [Best deep CNN architectures and their principles: from AlexNet to EfficientNet](https://theaisummer.com/cnn-architectures/)

### Convolutions
- [Understanding convolutions](http://colah.github.io/posts/2014-07-Understanding-Convolutions/)
- [An Introduction to different Types of Convolutions in DL](https://towardsdatascience.com/types-of-convolutions-in-deep-learning-717013397f4d)
- https://towardsdatascience.com/a-comprehensive-introduction-to-different-types-of-convolutions-in-deep-learning-669281e58215
- https://towardsdatascience.com/types-of-convolutions-in-deep-learning-717013397f4d
- [Depthwise separable convolution](https://towardsdatascience.com/a-basic-introduction-to-separable-convolutions-b99ec3102728)
- https://stackoverflow.com/questions/42883547/intuitive-understanding-of-1d-2d-and-3d-convolutions-in-convolutional-neural-n 
- https://medium.com/mlreview/a-guide-to-receptive-field-arithmetic-for-convolutional-neural-networks-e0f514068807
- [Convolutions Over Volumes (channels)](https://www.youtube.com/watch?v=KTB_OFoAQcc )

### 1x1 convolutions
- 1x1 convolutions: https://d2l.ai/chapter_convolutional-neural-networks/channels.html#times-1-convolutional-layer
- [1x1 convolutions](https://www.youtube.com/watch?v=qVP574skyuM)
- [Networks in Networks and 1x1 Convolutions](https://www.youtube.com/watch?v=vcp0XvDAX68)
- https://iamaaditya.github.io/2016/03/one-by-one-convolution/
- https://towardsdatascience.com/1x1-convolution-5219bbc09027
- https://medium.com/analytics-vidhya/talented-mr-1x1-comprehensive-look-at-1x1-convolution-in-deep-learning-f6b355825578
- https://machinelearningmastery.com/introduction-to-1x1-convolutions-to-reduce-the-complexity-of-convolutional-neural-networks/
	- A convolutional layer with a 1×1 filter is used at any point in a CNN to control the number of feature maps. It's often referred to as a projection operation or projection layer, or even a feature map or channel pooling layer


## Code 
- #CODE [Modern Convolutional Neural Network Architectures](https://github.com/Nyandwi/ModernConvNets)
- #CODE [Keras Layers (for TensorFlow 2.x)](https://github.com/mvoelk/keras_layers)
- #CODE [Model Zoo - Discover open source deep learning code and pretrained models](https://modelzoo.co/)
- #CODE https://github.com/microsoft/computervision-recipes


### Channel/visual attention
- #CODE [Visual-attention-tf](https://github.com/vinayak19th/Visual_attention_tf) ^tfvisualattention
	- Pixel Attention
	- Channel Attention (CBAM)
	- Efficient Channel Attention
- #CODE [Convolution Variants](https://github.com/JinLi711/Convolution_Variants) ^kerasconvvariants
	- Attention Augmented (AA) Convolution Layer
	- Mixed Depthwise Convolution Layer
	- Drop Block
	- Efficient Channel Attention (ECA) Layer
	- Convolutional Block Attention Module (CBAM) Layer


## References
- #PAPER [A guide to convolution arithmetic for deep learning (Dumoulin, 2016)](https://arxiv.org/abs/1603.07285)
	- #CODE https://github.com/vdumoulin/conv_arithmetic
- #PAPER [Xception: Deep Learning with Depthwise Separable Convolutions (Chollet 2017)](https://arxiv.org/abs/1610.02357)
- #PAPER [3D Depthwise Convolution: Reducing Model Parameters in 3D Vision Tasks (Ye 2018)](https://arxiv.org/abs/1808.01556)
- #PAPER [Making Convolutional Networks Shift-Invariant Again (Zhang 2019)](https://arxiv.org/pdf/1904.11486v2)
- #PAPER [A Survey of the Recent Architectures of Deep Convolutional Neural Networks (Khan 2020)](https://arxiv.org/abs/1901.06032v7)
- #PAPER [Revisiting Spatial Invariance with Low-Rank Local Connectivity (Elsayed 2020)](https://arxiv.org/abs/2002.02959)
	- #CODE https://github.com/google-research/google-research/tree/master/low_rank_local_connectivity
- #THESIS/PHD [Multi-modal Medical Image Processing with Applications in HybridX-ray/Magnetic Resonance Imaging (Stimpel 2021)](https://opus4.kobv.de/opus4-fau/frontdoor/deliver/index/docId/15697/file/Dissertation_Bernhard_Stimpel.pdf)
- #PAPER [Involution: Inverting the Inherence of Convolution for Visual Recognition (Li 2021)](https://arxiv.org/abs/2103.06255)
	- #CODE https://github.com/d-li14/involution
	- #CODE https://github.com/PrivateMaRyan/keras-involution2Ds
	- [Paper explained](https://www.youtube.com/watch?v=pH2jZun8MoY)
- #PAPER [Non-deep Networks (Goyal 2021)](https://arxiv.org/abs/2110.07641)
	- #CODE https://paperswithcode.com/paper/non-deep-networks-1?from=n19
	- use parallel subnetworks instead of stacking one layer after another. This helps effectively reduce depth while maintaining high performance
* #PAPER [ConvNext: A ConvNet for the 2020s (Liu 2022)](https://arxiv.org/abs/2201.03545) ^convnext
	* #CODE https://github.com/facebookresearch/ConvNeXt
	* #CODE https://github.com/bamps53/convnext-tf/
	* #CODE https://github.com/sayakpaul/ConvNeXt-TF
	* Paper explained: 
		* https://www.youtube.com/watch?v=WvKsMI4Iemk&t=330s
		* https://www.youtube.com/watch?v=idiIllIQOfU&list=WL&index=55
		* https://www.youtube.com/watch?v=QqejV0LNDHA
	* https://twitter.com/papers_daily/status/1481937771732566021
	* ConvNeXt essentially takes a ResNet and gradually "modernizes" it to discover components that contribute to performance gains. ConvNeXt applies several tricks like larger kernels, layer norm, fewer activation functions, separate downsampling layers to name a few. 
	* These results show that hybrid models are promising and that different components can still be optimized further and composed more effectively to improve the overall model on a wide range of vision tasks.
- #PAPER [Scaling Up Your Kernels to 31x31: Revisiting Large Kernel Design in CNNs (Ding 2022)](https://arxiv.org/pdf/2203.06717v3)            
	- #CODE https://paperswithcode.com/paper/scaling-up-your-kernels-to-31x31-revisiting
- #PAPER [Learning to Resize Images for Computer Vision Tasks (Talebi 2021)](https://arxiv.org/pdf/2103.09950v1)            


## Subtopics and applications
### Sequence (time series) modelling
- #PAPER [An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling (Bai 2018)](https://arxiv.org/abs/1803.01271)
  - Temporal convolutional networks (TCN)
  - #CODE https://github.com/philipperemy/keras-tcn
  - [Implementing Temporal Convolutional Networks](https://medium.com/the-artificial-impostor/notes-understanding-tensorflow-part-3-7f6633fcc7c7)
	  - The most important component of TCNs is dilated causal convolution. “Causal” simply means a filter at time step t can only see inputs that are no later than t. The point of using dilated convolution is to achieve larger receptive field with fewer parameters and fewer layers. 
	  - A residual block stacks two dilated causal convolution layers together, and the results from the final convolution are added back to the inputs to obtain the outputs of the block. 
  - [Temporal convolutional networks for sequence modeling](https://dida.do/blog/temporal-convolutional-networks-for-sequence-modeling)
- #PAPER [Convolutions Are All You Need (For Classifying Character Sequences) (Wood-doughty 2018)](https://www.aclweb.org/anthology/W18-6127/)
- #PAPER [InceptionTime: Finding AlexNet for time series classification (Fawaz 2021)](https://link.springer.com/article/10.1007/s10618-020-00710-y)
	- #CODE https://github.com/hfawaz/InceptionTime
	- https://arxiv.org/abs/1909.04939


### Object classification, image recognition
See [[AI/Computer Vision/Object classification, image recognition]]

### Semantic segmentation
See [[AI/Computer Vision/Semantic segmentation]]

### Object detection
See [[AI/Computer Vision/Object detection]]

### Video segmentation and prediction
See [[AI/Computer Vision/Video segmentation and prediction]]

### Image and video captioning
See [[AI/Computer Vision/Image and video captioning]]

### Image-to-image translation
See [[AI/Computer Vision/Image-to-image translation]]

### Super-resolution 
See "CNN-based" section in [[AI/Computer Vision/Super-resolution]]

### Inpainting
See "CNN-based" section in [[AI/Computer Vision/Inpainting and restoration]]

### Background subtraction, foreground detection
See "CNN-based" section in [[AI/Computer Vision/Background subtraction]]

### Edge detection
- #PAPER [DeepEdge: A Multi-Scale Bifurcated Deep Network for Top-Down Contour Detection](http://arxiv.org/pdf/1412.1123)
- #PAPER [DeepContour: A Deep Convolutional Feature Learned by Positive-Sharing Loss for Contour Detection](http://mc.eistar.net/UpLoadFiles/Papers/DeepContour_cvpr15.pdf)


### Human pose estimation and activity recognition
- https://en.wikipedia.org/wiki/Activity_recognition
- https://machinelearningmastery.com/deep-learning-models-for-human-activity-recognition/
- https://github.com/cbsudux/awesome-human-pose-estimation
- https://github.com/topics/human-pose-estimation
- https://www.learnopencv.com/deep-learning-based-human-pose-estimation-using-opencv-cpp-python/

- #PAPER [Human activity recognition with smartphone sensors using deep learning neural networks (Ann Ronao 2016)](https://www.sciencedirect.com/science/article/abs/pii/S0957417416302056)
- #PAPER [Convolutional pose machines (Wei 2016)](https://arxiv.org/abs/1602.00134)
- #PAPER [Fast Human Pose Estimation (Zhang 2019)](https://arxiv.org/abs/1811.05419)


### Motion detection, tracking
- #PAPER [FlowNet: Learning Optical Flow with Convolutional Networks (Fischer 2015)](https://arxiv.org/abs/1504.06852)


### Deconvolution
- #PAPER [Deep Convolutional Neural Network for Image Deconvolution (Xu 2014)](http://lxu.me/projects/dcnn/)


### Visual/Channel attention and Saliency
See "Neural Networks explainability" section in [[AI/XAI]]

 - #PAPER [Squeeze-and-Excitation Networks, SENets (Hu 2017)](https://arxiv.org/abs/1709.01507) ^senets
	- Features can incorporate global context
	- Since SENet only revolves around providing channel attention by using dedicated global feature descriptors, which in this case is Global Average Pooling (GAP), there is a loss of information and the attention provided is point-wise. This means that all pixels are mapped in the spatial domain of a feature map uniformly, and thus not discriminating between important or class-deterministic pixels versus those which are part of the background or not containing useful information.
	- Thus, the importance/need for spatial attention is justified to be coupled with channel attention. One of the prime examples of the same is CBAM (published at ECCV 2018) 
	- #CODE https://github.com/hujie-frank/SENet
	- #CODE https://github.com/yoheikikuta/senet-keras
	- https://blog.paperspace.com/channel-attention-squeeze-and-excitation-networks/
	- https://programmerclick.com/article/4934219785/
	- https://pyimagesearch.com/2022/05/30/attending-to-channels-using-keras-and-tensorflow/
 - #PAPER [CBAM: Convolutional Block Attention Module (Woo 2018)](https://arxiv.org/abs/1807.06521) ^cbam
	 - #CODE https://kobiso.github.io//research/research-CBAM/
	 - https://medium.com/visionwizard/understanding-attention-modules-cbam-and-bam-a-quick-read-ca8678d1c671
	 - https://blog.paperspace.com/attention-mechanisms-in-computer-vision-cbam/
- #PAPER [ECA-Net: Efficient Channel Attention for Deep Convolutional Neural Networks (Wang 2020)](https://arxiv.org/abs/1910.03151)
	- this paper proposes an Efficient Channel Attention (ECA) module, which only involves a handful of parameters while bringing clear performance gain
	- proposed a local cross-channel interaction strategy without dimensionality reduction, which can be efficiently implemented via 1D convolution
- #PAPER See ^srwithpixelattention in [Super-resolution](AI/Computer%20Vision/Super-resolution.md)
- #PAPER [Attention Mechanisms in Computer Vision: A Survey (Guo 2021)](https://arxiv.org/abs/2111.07624v1)
	- https://github.com/MenghaoGuo/Awesome-Vision-Attentions
- #PAPER [Visual Attention Network (Guo 2022)](https://arxiv.org/abs/2202.09741)
	- #CODE https://paperswithcode.com/paper/visual-attention-network?from=n26
	- This work presents an approach that decomposes a large kernel convolution operation to capture long-range relationship. After obtaining long-range relationship, it estimates the importance of a point and generates attention map
