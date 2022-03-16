
---
title: "Video segmentation and prediction"
disableToc: false 
---

See: 
- [Encoder-decoder networks](AI/Deep%20learning/Encoder-decoder%20networks.md)
- "Deep learning for multi-dimensional data" section in [Deep learning](AI/Deep%20learning/Deep%20learning.md)
- [RNNs](AI/Deep%20learning/RNNs.md)

## Resources
- Spatiotemporal classification and regression
- Hybrid convolutional and recurrent networks, 3dconv and related approaches
- https://github.com/jinwchoi/awesome-action-recognition
- http://blog.qure.ai/notes/deep-learning-for-videos-action-recognition-review
- https://stackoverflow.com/questions/55926841/convolving-across-channels-in-keras-cnn-conv1d-depthwise-separable-conv-cccp
- https://towardsdatascience.com/a-basic-introduction-to-separable-convolutions-b99ec3102728


## Courses
- #COURSE [Advanced Models for Computer Vision (DeepMind x UCL | Deep Learning Lectures)](https://www.youtube.com/watch?v=_aUq7lmMfxo&list=PLqYmG7hTraZCDxZ44o4p3N5Anz3lLRVZF&index=4)
	- https://storage.googleapis.com/deepmind-media/UCLxDeepMind_2020/L4%20-%20UCLxDeepMind%20DL2020.pdf


## References
- #PAPER [Learning Spatiotemporal Features with 3D Convolutional Networks. C3D, 3D CNNs (Tran 2015)](https://arxiv.org/abs/1412.0767)
- #PAPER [Unsupervised Learning of Video Representations using LSTMs (Srivastava 2016)](https://arxiv.org/abs/1502.04681)
- #PAPER [Convolutional Gated Recurrent Networks for Video Segmentation (Siam 2016)](https://arxiv.org/abs/1611.05435)
	- Hybrid convolutional and recurrent networks
- #PAPER [LRCN: Long-term Recurrent Convolutional Networks for Visual Recognition and Description (Donahue 2016)](https://arxiv.org/abs/1411.4389)
	- Hybrid convolutional and recurrent networks
- #PAPER [Convolutional Two-Stream Network Fusion for Video Action Recognition (Feichtenhofer 2016)](https://arxiv.org/abs/1604.06573)
- #PAPER [Deep Predictive Coding Networks for Video Prediction and Unsupervised Learning (Lotter 2016)](https://arxiv.org/abs/1605.08104)
	- https://coxlab.github.io/prednet/
- #PAPER [ContextVP: Fully Context-Aware Video Prediction (Byeon 2018)](https://arxiv.org/abs/1710.08518)
	- http://on-demand.gputechconf.com/gtc/2018/presentation/s8713-fully-context-aware-video-prediction.pdf 
- #PAPER [Machine Learning for Spatiotemporal Sequence Forecasting: A Survey (Shi, 2018)](https://arxiv.org/abs/1808.06865)
- #PAPER [Residual Convolutional LSTM for Tweet Count Prediction (Wei 2018)](https://dl.acm.org/doi/fullHtml/10.1145/3184558.3191571)
- #PAPER [A Closer Look at Spatiotemporal Convolutions for Action Recognition (Tran 2018)](https://arxiv.org/abs/1711.11248)
	- #CODE https://github.com/facebookresearch/VMZ
	- #CODE See Ghadiyaram 2019 below
	- #CODE https://github.com/juenkhaw/action_recognition_project
	- demonstrate that 3D ResNets significantly outperform 2D ResNets for the same depth when trained and evaluated on large-scale,challenging action recognition benchmarks
	- introduce two new forms of spatio temporal convolution that can be viewed as middle grounds between the extremes of 2D (spatial convolution) and full 3D: mixed convolution (MC) and consists in employing 3D convolutions only in the early layers of the network, with 2D convolutions in the top layers, and the R(2+1)D spatiotemporal conv block which explicitly factorizes 3D convolution into two separate and successive operations, a 2D spatial convolution and a 1D temporal convolution
	- the first advantage is an additional nonlinear rectification between these two operations. This effectively doubles the number of non-linearities compared to a network using full 3D convolutions for the same number of parameters, thus rendering the model capable of representing more complex functions.The second potential benefit is that the decomposition facilitates the optimization, yielding in practice both a lower training loss and a lower testing loss
- #PAPER [Video Classification with Channel-Separated Convolutional Networks (Tran 2019)](https://arxiv.org/abs/1904.02811)
	- #CODE https://github.com/facebookresearch/VMZ
- #PAPER [Dilated 3D Convolutional Neural Networks for Brain MRI Data Classification (Wang 2019)](https://ieeexplore.ieee.org/abstract/document/8840843)
- #PAPER [Deep Learning for Spatio-Temporal Data Mining: A Survey (Wang 2019)](https://arxiv.org/abs/1906.04928)
- #PAPER [Large-scale weakly-supervised pre-training for video action recognition (Ghadiyaram 2019)](https://arxiv.org/abs/1905.00561)
	- #CODE https://github.com/microsoft/computervision-recipes/tree/master/scenarios/action_recognition
- #PAPER [Eidetic 3D LSTM A Model for Video Prediction and Beyond, E3D-LSTM (Wang 2019)](https://openreview.net/forum?id=B1lKS2AqtX)
	- #CODE https://github.com/google/e3d_lstm
- #PAPER [Late Temporal Modeling in 3D CNN Architectures with BERT for Action Recognition (Esat Kalfaoglu 2020)](https://arxiv.org/abs/2008.01232)
- #PAPER [An Image is Worth 16x16 Words, What is a Video Worth? (Sharir 2021)](https://arxiv.org/abs/2103.13915)
- #PAPER [UNETR: Transformers for 3D Medical Image Segmentation (Hatamizadeh 2021)](https://arxiv.org/abs/2103.10504)
	- https://theaisummer.com/medical-segmentation-transformers/
	- UNETR is the first successful transformer architecture for 3D medical image segmentation
- #PAPER [Dense Unsupervised Learning for Video Segmentation (Araslanov 2021)](https://arxiv.org/abs/2111.06265)
	- https://github.com/visinf/dense-ulearn-vos
	- methods that learns spatio-temporal correspondences without any supervision ([Unsupervised learning](AI/Unsupervised%20learning/Unsupervised%20learning.md)), and achieves state-of-the-art accuracy of video object segmentation
	- #TALK https://www.youtube.com/watch?v=tSBWZ6nYld0
- #PAPER [Mask2Former for Video Instance Segmentation (Cheng 2021)](https://arxiv.org/abs/2112.10764v1)
	- #CODE https://github.com/facebookresearch/Mask2Former
