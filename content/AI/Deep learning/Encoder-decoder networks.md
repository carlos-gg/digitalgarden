---
title: "Encoder-decoder networks"
disableToc: false 
---

## Resources
- Very common models for semantic segmentation tasks
- [Deep learning](AI/Deep%20learning/Deep%20learning.md)] architectures composed of two paths, an encoding and a decoding one. [Autoencoders](AI/Deep%20learning/Autoencoders.md)] are similar but unsupervised (reconstructions loss)
- U-NETs are a type of encoder-decoder [CNNs](AI/Deep%20learning/CNNs.md)] model with skipped connections trained in a [Supervised learning](AI/Supervised%20Learning/Supervised%20learning.md)] context for image segmentation and related tasks
- https://www.slideshare.net/PetteriTeikariPhD/multiphoton-vasculature-segmentation-5-unet


## References
- #PAPER [U-Net: Convolutional Networks for Biomedical Image Segmentation (Ronneberger 2015)](https://arxiv.org/abs/1505.04597 )
	- https://towardsdatascience.com/review-u-net-biomedical-image-segmentation-d02bf06ca760 
	- https://github.com/karolzak/keras-unet 
	- https://tuatini.me/practical-image-segmentation-with-unet/ 
	- https://github.com/divamgupta/image-segmentation-keras/blob/master/keras_segmentation/models/unet.py 
	- [diagram example](https://www.researchgate.net/publication/323302730/figure/fig1/AS:596310398881793@1519182886358/U-Net-architecture-consisted-with-convolutional-encoding-and-decoding-units-that-take.png )
- #PAPER [3D U-Net: Learning Dense Volumetric Segmentation from Sparse Annotation (Cicek 2016)](https://arxiv.org/abs/1606.06650)
	- https://towardsdatascience.com/review-3d-u-net-volumetric-segmentation-medical-image-segmentation-8b592560fac1 
- #PAPER [V-Net: Fully Convolutional Neural Networks for Volumetric Medical Image Segmentation (Milletari 2016)](https://arxiv.org/abs/1606.04797)
	- https://towardsdatascience.com/review-v-net-volumetric-convolution-biomedical-image-segmentation-aa15dbaea974 
- #PAPER [Volumetric ConvNets with Mixed Residual Connections for Automated Prostate Segmentation from 3D MR Images, 3D UNET+Resnet (Yu 2017)](https://aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14719)
	- https://towardsdatascience.com/review-3d-u-net-resnet-volumetric-convolutions-long-short-residual-connections-biomedical-3a7da3f98dae
- #PAPER [Automatic 3D Cardiovascular MR Segmentation with Densely-Connected Volumetric ConvNets, DenseVoxNet (Yu 2017)](https://arxiv.org/abs/1708.00573 )
	- https://medium.com/@sh.tsang/review-densevoxnet-volumetric-brain-segmentation-biomedical-image-segmentation-9136bb6128dd 
- #PAPER [Road Extraction by Deep Residual U-Net, ResUNET (Zhang 2017)](https://arxiv.org/abs/1711.10684)
	- https://github.com/nikhilroxtomar/Deep-Residual-Unet
- #PAPER [Recurrent Residual Convolutional Neural Network based on U-Net (R2U-Net) for Medical Image Segmentation (Alom 2018)](https://www.researchgate.net/publication/323302730_Recurrent_Residual_Convolutional_Neural_Network_based_on_U-Net_R2U-Net_for_Medical_Image_Segmentation)
- #PAPER [UNet++: A Nested U-Net Architecture for Medical Image Segmentation (Zhou 2018)](https://arxiv.org/abs/1807.10165)
	- https://medium.com/@sh.tsang/review-unet-a-nested-u-net-architecture-biomedical-image-segmentation-57be56859b20 
- #PAPER [H-DenseUNet: Hybrid Densely Connected UNet for Liver and Tumor Segmentation from CT Volumes (Li 2018)](https://arxiv.org/abs/1709.07330  )
	- https://medium.com/@sh.tsang/review-h-denseunet-2d-3d-denseunet-for-intra-inter-slice-features-biomedical-image-f3e526e81fe7 
	- #CODE https://github.com/xmengli999/H-DenseUNet/
- #PAPER [Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation, DeepLabv3+ (Chen 2018)](https://arxiv.org/abs/1802.02611)
	- #CODE https://github.com/ChoiDM/pytorch-deeplabv3plus-3D 
- #PAPER [ResUNet-a: a deep learning framework for semantic segmentation of remotely sensed data (Diakogiannis 2019)](https://arxiv.org/abs/1904.00592)
- #PAPER [ResUNet++: An Advanced Architecture for Medical Image Segmentation (Jha 2019)](https://arxiv.org/abs/1911.07067)
- #PAPER [M-Net: U-Net with Multi-stream Feature Fusion and Multi-scale Dilated Convolutions (Fu 2019)](https://ieeexplore.ieee.org/document/8864993 )
	- https://www.researchgate.net/publication/336455527_M-Net_A_Novel_U-Net_with_Multi-stream_Feature_Fusion_and_Multi-scale_Dilated_Convolutions_for_Bile_Ducts_and_Hepatolith_Segmentation_September_2019 
- #PAPER [Channel-Unet: A Spatial Channel-Wise Convolutional Neural Network for Liver and Tumors Segmentation (Chen 2019)](https://www.frontiersin.org/articles/10.3389/fgene.2019.01110/full)
- #PAPER [Bi-Directional ConvLSTM U-Net with Densely Connected Convolutions (Azad 2019)](https://arxiv.org/abs/1909.00166)
    - #CODE https://github.com/rezazad68/BCDU-Net/blob/master/Retina%20Blood%20Vessel%20Segmentation/models.py
- #PAPER [LSTM-UNET - Microscopy Cell Segmentation via Convolutional LSTM Networks (Arbelle 2019)](https://arxiv.org/abs/1805.11247)
	#CODE https://github.com/arbellea/LSTM-UNet
- #PAPER [USE-Net: incorporating Squeeze-and-Excitation blocks into U-Net for prostate zonal segmentation of multi-institutional MRI datasets (Rundo 2019)](https://arxiv.org/abs/1904.08254)
- #PAPER [Evaluation of Multi-Slice Inputs to Convolutional Neural Networks for Medical Image Segmentation (Vu 2019)](https://arxiv.org/abs/1912.09287)
- #PAPER [Making a Case for 3D Convolutions for Object Segmentation in Videos (Mahadevan 2020)](https://arxiv.org/abs/2008.11516)
	- proposed a simple and fast network architecture consisting entirely of 3D  convolutions that is capable of effectively learning spatio-temporal features
	- used a 3D ResNet pretrained for video action classification as an encoder, and a novel decoder architecture inspired by existing 2D convolutional networks
- #PAPER [nnU-Net: a self-configuring method for deep learning-based biomedical image segmentation (Isensee 2020)](https://www.nature.com/articles/s41592-020-01008-z)
	- https://www.sciencedaily.com/releases/2020/12/201207112253.htm
	- #CODE https://github.com/MIC-DKFZ/nnUNet
- #PAPER [MCNN, Multi-resolution convolutional neural networks for inverse problems (Wang 2020)](https://www.nature.com/articles/s41598-020-62484-z)
	- #CODE https://github.com/fengwang/MCNN
	- #CODE https://github.com/fengwang/mcnn-demo/tree/master/demo