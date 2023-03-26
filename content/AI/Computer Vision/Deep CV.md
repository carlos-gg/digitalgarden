---
title: "Deep CV"
---

> DL is used in the domain of digital image processing to solve difficult problems (e.g.image colorization, classification, segmentation and  detection). DL methods such as CNNs mostly improve prediction performance using big data and plentiful computing resources and have pushed the boundaries of what was possible. Problems which were assumed to be unsolvable are now solved with super-human accuracy (eg image classification). Since being reignited by Krizhevsky, Sutskever and Hinton in 2012, DL has dominated the domain ever since due to a substantially better performance compared to traditional methods.

> See:
> - [[AI/Deep learning/CNNs]]
> - [[AI/Deep learning/GANs]]
> - [[AI/Deep learning/Normalizing flows]] 
> - "For Computer Vision" section in [[AI/Deep learning/Transformers]]
> - [[AI/Computer Vision/Deep image prior]]


## Resources
- https://github.com/kjw0612/awesome-deep-vision
- https://github.com/timzhang642/3D-Machine-Learning
- https://medium.com/@taposhdr/medical-image-analysis-with-deep-learning-i-23d518abf531
- http://danielnouri.org/notes/2014/12/17/using-convolutional-neural-nets-to-detect-facial-keypoints-tutorial/

### Applications
See:
- [[AI/Computer Vision/Background subtraction]]
- [[AI/Computer Vision/Image and video captioning]] 
- [[AI/Computer Vision/Image-to-image translation]]
- [[AI/Computer Vision/Inpainting and restoration]]
- [[AI/Computer Vision/Object classification, image recognition]]
- [[AI/Computer Vision/Object detection]]
- [[AI/Computer Vision/Semantic segmentation]]
- [[AI/Computer Vision/Super-resolution]]
- [[AI/Computer Vision/Video Frame Interpolation]]
- [[AI/Computer Vision/Video segmentation and prediction]]

## Code
- #CODE [ChainerCV: a Library for Computer Vision in Deep Learning](https://github.com/chainer/chainercv)
		- http://chainercv.readthedocs.io/en/stable/
- #CODE [Openface. Free and open source face recognition with deep neural networks](https://cmusatyalab.github.io/openface/)
- #CODE [Vision](https://github.com/pytorch/vision) - The torchvision package consists of popular datasets, model architectures, and common image transformations fo CV
- #CODE [Scenic](https://github.com/google-research/scenic) - A Jax Library for Computer Vision Research and Beyond
	- https://www.marktechpost.com/2021/10/30/google-research-introduces-scenic-an-open-source-jax-library-for-computer-vision-research/
	- codebase with a focus on research around attention-based models for computer vision
	- #PAPER [SCENIC: A JAX Library for Computer Vision Research and Beyond (2021)](https://arxiv.org/abs/2110.11403)
- #CODE [Pytorch-image-models](https://github.com/rwightman/pytorch-image-models)
	- PyTorch image models, scripts, pretrained weights -- ResNet, ResNeXT, EfficientNet, EfficientNetV2, NFNet, Vision Transformer, MixNet, MobileNet-V3/V2, RegNet, DPN, CSPNet, and more
	- https://rwightman.github.io/pytorch-image-models/
- #CODE [Imgaug. Image augmentation for machine learning experiments](https://github.com/aleju/imgaug)
	- http://imgaug.readthedocs.io

## References
- #PAPER #REVIEW [Deep Learning for Computer Vision: A Brief Review (Voulodimos 2017)](https://www.hindawi.com/journals/cin/2018/7068349/)
- #PAPER [Deep Learning vs. Traditional Computer Vision (O'Mahony 2019)](https://arxiv.org/abs/1910.13796)
- #PAPER [Deep learning encodes robust discriminative neuroimaging representations to outperform standard machine learning (Abrol 2021)](https://www.nature.com/articles/s41467-020-20655-6)
- #PAPER #REVIEW [Deep learning-enabled medical computer vision (Esteva 2021)](https://www.nature.com/articles/s41746-020-00376-2)
- #PAPER [Involution: Inverting the Inherence of Convolution for Visual Recognition, a brand new neural operator (Li 2021)](https://arxiv.org/abs/2103.06255)
	- #CODE https://github.com/d-li14/involution
	- #CODE https://github.com/PrivateMaRyan/keras-involution2Ds
	- [Paper explained](https://www.youtube.com/watch?v=pH2jZun8MoY)
	- https://keras.io/examples/vision/involution/
	- [Involution: Inverting the Inherence of Convolution for Visual Recognition](https://medium.com/analytics-vidhya/involution-a-step-towards-a-new-generation-of-neural-networks-for-visual-recognition-3b8ad75eb818)
	- involution is a general-purpose neural primitive that is versatile for a spectrum of deep learning models on different vision tasks
	- involution bridges convolution and self-attention in design, while being more efficient and effective than convolution, simpler than self-attention in form
	- the proposed involution operator could be leveraged as fundamental bricks to build the new generation of neural networks for visual recognition, powering different deep learning models on several prevalent benchmarks
- #PAPER [Unifying Nonlocal Blocks for Neural Networks (Zhu 2021)](https://arxiv.org/abs/2108.02451v3)
	- #CODE https://github.com/zh460045050/SNL_ICCV2021
- #PAPER [X-volution: On the unification of convolution and self-attention (Chen 2021)](https://arxiv.org/pdf/2106.02253)
- #PAPER [Bivolution: A Static and Dynamic Coupled Filter (Hu 2022)](https://aaai-2022.virtualchair.net/poster_aaai2015)
	- #CODE https://github.com/neuralchen/Bivolution	
- #PAPER [Convolution of Convolution: Let Kernels Spatially Collaborate (Zhao 2022)](https://www.semanticscholar.org/paper/Convolution-of-Convolution%3A-Let-Kernels-Spatially-Zhao-Li/87e0f7adce75bac24f944f0b8fb7e2441b36cfb4)
	- #CODE https://github.com/Genera1Z/ConvolutionOfConvolution
