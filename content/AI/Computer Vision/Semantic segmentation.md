---
title: "Semantic segmentation"
disableToc: false 
---


See:
[[Encoder-decoder networks]] for image segmentation
[[Object detection]]

- https://en.wikipedia.org/wiki/Image_segmentation
- https://github.com/mrgloom/awesome-semantic-segmentation
- https://blog.athelas.com/a-brief-history-of-cnns-in-image-segmentation-from-r-cnn-to-mask-r-cnn-34ea83205de4
- Overview of semantic image segmentation: https://www.jeremyjordan.me/semantic-segmentation/


## Code
- #CODE DeepLab2: https://github.com/google-research/deeplab2
	- DeepLab2 is a TensorFlow library for deep labeling, aiming to provide a unified and state-of-the-art TensorFlow codebase for dense pixel labeling tasks.
- #CODE Segmentation models with pretrained backbones (PyTorch): https://github.com/qubvel/segmentation_models
- #CODE https://www.tensorflow.org/tutorials/images/segmentation
- #CODE https://github.com/yassouali/pytorch-segmentation

## References
Review papers:
- #PAPER Deep learning for cardiac imagesegmentation: A review (2019): https://arxiv.org/abs/1911.03723
- #PAPER Evolution of Image Segmentation using Deep Convolutional Neural Network: A Survey (Sultana, 2020): https://arxiv.org/abs/2001.0407430

- #PAPER Fully Convolutional Networks for Semantic Segmentation (Long 2015): https://arxiv.org/abs/1411.4038
- #PAPER CGNet: A Light-weight Context Guided Network for Semantic Segmentation (Wu 2018): https://arxiv.org/abs/1811.08201 ^cgnet
	- Context Guided (CG) block learns the joint feature of both local feature and surrounding context, and further improves the joint feature with the global context
	- CGNet captures contextual information in all stages of the network and is specially tailored for increasing segmentation accuracy 
	- CGNet is also elaborately designed to reduce the number of parameters and save memory footprint
- #PAPER Panoptic-DeepLab: A Simple, Strong, and Fast Baseline for Bottom-Up Panoptic Segmentation (Cheng 2020): https://arxiv.org/abs/1911.10194
	- #CODE https://github.com/bowenc0221/panoptic-deeplab
- #PAPER Axial-DeepLab: Stand-Alone Axial-Attention for Panoptic Segmentation (Wang 2020): https://arxiv.org/abs/2003.07853
	- #CODE https://github.com/csrhddlam/axial-deeplab
	- Paper explained: https://www.youtube.com/watch?v=hv3UO3G0Ofo
- #PAPER Towards infield, live plant phenotyping using a reduced-parameter CNN (Atanbori 2020): https://link.springer.com/article/10.1007%2Fs00138-019-01051-7