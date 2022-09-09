---
title: "Computer Vision"
---

> Computer vision is an interdisciplinary scientific field that deals with how computers can gain high-level understanding from digital images or videos. From the perspective of engineering, it seeks to understand and automate tasks that the human visual system can do

> See: 
> - [[AI/Deep learning/CNNs]]
> - "MLPs for vision and language" section in [[AI/Deep learning/MLPs]]
> - "For Computer Vision" section in [[AI/Deep learning/Transformers]]
> - "Generative models for Image data" section in [[AI/Deep learning/Generative modelling]]
> - [[AI/Deep learning/GANs]]
> - [[AI/Unsupervised learning/Sparse dictionary learning]]


## Resources
- https://github.com/jbhuang0604/awesome-computer-vision
- [Papers with code - computer vision](https://paperswithcode.com/area/computer-vision)
- https://en.wikipedia.org/wiki/Computer_vision
- [Denoising: wavelet thresholding](https://blancosilva.wordpress.com/teaching/mathematical-imaging/denoising-wavelet-thresholding/)

## Books
- #BOOK [Image Processing and Acquisition using Python (Chityala 2014)](https://www.crcpress.com/Image-Processing-and-Acquisition-using-Python/Chityala-Pudipeddi/p/book/9781466583757)
- #BOOK [Computer Vision: A Modern Approach (Forsyth, 2011 PEARSON)](https://www.pearson.com/us/higher-education/program/Forsyth-Computer-Vision-A-Modern-Approach-2nd-Edition/PGM111082.html)
	- https://github.com/yihui-he/computer-vision-tutorial/blob/master/Computer%20Vision%20A%20Modern%20Approach%202nd%20Edition.pdf
- #BOOK [Computer Vision: Models, Learning, and Inference (Prince, 2012 CAMBRIDGE)](http://www.computervisionmodels.com/)
- #BOOK [Computer vision (chapter)](https://d2l.ai/chapter_computer-vision/index.html)

## Courses
- #COURSE [Computer vision (CS543/ECE549, UIUC)](https://courses.engr.illinois.edu/cs543/sp2015/)
- #COURSE [Advances in Computer vision (MIT)](http://6.869.csail.mit.edu/fa18/)
- #COURSE [Introduction to computer vision (Udacity, Georgia Tech)](https://www.udacity.com/course/introduction-to-computer-vision--ud810)
- #COURSE [Deep Learning for Computer Vision (UPC TelecomBCN 2016)](http://imatge-upc.github.io/telecombcn-2016-dlcv/)
- #COURSE [Convolutional Neural Networks for Visual Recognition (CS231n, Stanford)](http://cs231n.github.io/)
	- [Pre-version of the course](http://karpathy.github.io/neuralnets/)
	- [Notes (Karpathy)](http://cs231n.github.io/)
	- [Videos for each lecture](https://www.youtube.com/playlist?list=PLkt2uSq6rBVctENoVBg1TpCC7OQi31AlC)
- #COURSE [Computer vision (NYU)](https://cs.nyu.edu/~fergus/teaching/vision/)
- #COURSE [Digital image processing (U Tartu)](https://sisu.ut.ee/dev/imageprocessing/avaleht)
- #COURSE [Convolutional Neural Networks for Image Recognition](https://www.youtube.com/watch?v=shVKhOmT0HE&list=PLqYmG7hTraZCDxZ44o4p3N5Anz3lLRVZF&index=3&t=1s) (DeepMind x UCL | Deep Learning Lectures)
	- https://storage.googleapis.com/deepmind-media/UCLxDeepMind_2020/L3%20-%20UUCLxDeepMind%20DL2020.pdf
- #COURSE [Advanced Models for Computer Vision](https://www.youtube.com/watch?v=_aUq7lmMfxo&list=PLqYmG7hTraZCDxZ44o4p3N5Anz3lLRVZF&index=4)(DeepMind x UCL | Deep Learning Lectures)
	- https://storage.googleapis.com/deepmind-media/UCLxDeepMind_2020/L4%20-%20UCLxDeepMind%20DL2020.pdf
- #COURSE [Rendering course (TU Wien)](https://users.cg.tuwien.ac.at/zsolnai/gfx/rendering-course/)
	- This rendering course is an MSc-level class at the Technical University of Vienna. It is about ray tracing, photorealistic rendering and global illumination
	- [Playlist](https://www.youtube.com/playlist?list=PLujxSBD-JXgnGmsn7gEyN28P1DnRZG7qi)


## Code
- #CODE [Scikit-image. Image processing in Python](https://github.com/scikit-image/scikit-image)
	- http://scikit-image.org
- #CODE [OpenCV (Open Source Computer Vision Library)](https://opencv.org/)
	- OpenCV is released under a BSD license and hence it’s free for both academic and commercial use. It has C++, Python and Java interfaces and supports Windows, Linux, Mac OS, iOS and Android. OpenCV was designed for computational efficiency and with a strong focus on real-time applications. Written in optimized C/C++, the library can take advantage of multi-core processing. Enabled with OpenCL, it can take advantage of the hardware acceleration of the underlying heterogeneous compute platform.
	- https://github.com/opencv/opencv/wiki/Deep-Learning-in-OpenCV
	- #PAPER [Real-time computer vision with OpenCV (Pulli 2012)](https://dl.acm.org/doi/10.1145/2184319.2184337)
- #CODE [SimpleCV](https://github.com/sightmachine/SimpleCV)
	- http://simplecv.org/
	- SimpleCV is an open source framework for building computer vision applications. With it, you get access to several high-powered computer vision libraries such as OpenCV – without having to first learn about bit depths, file formats, color spaces, buffer management, eigenvalues, or matrix versus bitmap storage. This is computer vision made easy.
- #CODE [Imgaug. Image augmentation for machine learning experiments](https://github.com/aleju/imgaug)
	- http://imgaug.readthedocs.io
- #CODE [ChainerCV: a Library for Computer Vision in Deep Learning](https://github.com/chainer/chainercv)
		- http://chainercv.readthedocs.io/en/stable/
		- ChainerCV is a collection of tools to train and run neural networks for computer vision tasks using Chainer
- #CODE [Openface. Free and open source face recognition with deep neural networks](https://cmusatyalab.github.io/openface/)
- #CODE Vision - The torchvision package consists of popular datasets, model architectures, and common image transformations fo CV. 
	- https://github.com/pytorch/vision
- #CODE [Scenic](https://github.com/google-research/scenic)
	- https://www.marktechpost.com/2021/10/30/google-research-introduces-scenic-an-open-source-jax-library-for-computer-vision-research/
	- A Jax Library for Computer Vision Research and Beyond
	- codebase with a focus on research around attention-based models for computer vision
	- #PAPER [SCENIC: A JAX Library for Computer Vision Research and Beyond (2021)](https://arxiv.org/abs/2110.11403)
- #CODE [Pytorch-image-models](https://github.com/rwightman/pytorch-image-models)
	- PyTorch image models, scripts, pretrained weights -- ResNet, ResNeXT, EfficientNet, EfficientNetV2, NFNet, Vision Transformer, MixNet, MobileNet-V3/V2, RegNet, DPN, CSPNet, and more
	- https://rwightman.github.io/pytorch-image-models/

## References
- #PAPER [Brief review of image denoising techniques (Fan 2019)](https://vciba.springeropen.com/articles/10.1186/s42492-019-0016-7)

### Traditional CV techniques
See [[AI/Computer Vision/Traditional CV]]

### Deep learning-based CV
See [[AI/Computer Vision/Deep CV]]


