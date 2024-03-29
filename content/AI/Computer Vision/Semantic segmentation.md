---
title: "Semantic segmentation"
---

> See:
> - [[AI/Deep learning/Encoder-decoder networks]] for image segmentation 
> - [[AI/Computer Vision/Object detection]]

## Resources
- https://en.wikipedia.org/wiki/Image_segmentation
- https://github.com/mrgloom/awesome-semantic-segmentation
- https://blog.athelas.com/a-brief-history-of-cnns-in-image-segmentation-from-r-cnn-to-mask-r-cnn-34ea83205de4
- [Overview of semantic image segmentation](https://www.jeremyjordan.me/semantic-segmentation/)

## Code
- #CODE [DeepLab2](https://github.com/google-research/deeplab2)
	- DeepLab2 is a TensorFlow library for deep labeling, aiming to provide a unified and state-of-the-art TensorFlow codebase for dense pixel labeling tasks.
- #CODE [Segmentation models with pretrained backbones (PyTorch)](https://github.com/qubvel/segmentation_models)
- #CODE https://github.com/qubvel/segmentation_models
	- Python library with Neural Networks for Image Segmentation based on Keras and TensorFlow
- #CODE https://www.tensorflow.org/tutorials/images/segmentation
- #CODE https://github.com/yassouali/pytorch-segmentation

## References
- #PAPER [Fully Convolutional Networks for Semantic Segmentation (Long 2015)](https://arxiv.org/abs/1411.4038)
- #PAPER [CGNet: A Light-weight Context Guided Network for Semantic Segmentation (Wu 2018)](https://arxiv.org/abs/1811.08201) 
	- Context Guided (CG) block learns the joint feature of both local feature and surrounding context, and further improves the joint feature with the global context
	- CGNet captures contextual information in all stages of the network and is specially tailored for increasing segmentation accuracy 
	- CGNet is also elaborately designed to reduce the number of parameters and save memory footprint
- #PAPER #REVIEW [Deep learning for cardiac image segmentation: A review (2019)](https://arxiv.org/abs/1911.03723)
- #PAPER [Panoptic-DeepLab: A Simple, Strong, and Fast Baseline for Bottom-Up Panoptic Segmentation (Cheng 2020)](https://arxiv.org/abs/1911.10194)
	- #CODE https://github.com/bowenc0221/panoptic-deeplab
- #PAPER [Axial-DeepLab: Stand-Alone Axial-Attention for Panoptic Segmentation (Wang 2020)](https://arxiv.org/abs/2003.07853)
	- #CODE https://github.com/csrhddlam/axial-deeplab
	- [Paper explained](https://www.youtube.com/watch?v=hv3UO3G0Ofo)
- #PAPER #REVIEW [Evolution of Image Segmentation using Deep Convolutional Neural Network: A Survey (Sultana, 2020)](https://arxiv.org/abs/2001.0407430)
- #PAPER [Towards infield, live plant phenotyping using a reduced-parameter CNN (Atanbori 2020)](https://link.springer.com/article/10.1007%2Fs00138-019-01051-7)
- #PAPER [Learning What Not to Segment: A New Perspective on Few-Shot Segmentation (Lang 2022)](https://arxiv.org/pdf/2203.07615v2)            
- #PAPER [k-means Mask Transformer (Yu 2022)](https://arxiv.org/pdf/2207.04044v1)
	- #CODE https://github.com/google-research/deeplab2
	- rethought the relationship between pixels and object queries and propose to reformulate the cross-attention learning as a clustering process
	- k-means Mask Xformer (kMaX-DeepLab) for segmentation tasks is inspired by the traditional k-means clustering algorithm

### Unsupervised or self-supervised
- #PAPER [Unsupervised Semantic Segmentation by Distilling Feature Correspondences (Hamilton 2022)](https://arxiv.org/pdf/2203.08414)            
	- https://www.engadget.com/mit-computer-vision-algorithm-identifies-images-down-to-the-pixel-130051112.html?guccounter=1