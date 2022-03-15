---
title: "Super-resolution"
disableToc: false 
---

See [Image-to-image translation](AI/Computer%20Vision/Image-to-image%20translation.md)

## Resources
- [Papers and related resources, mainly state-of-the-art and novel works in ICCV, ECCV and CVPR about image super-resolution and video super-resolution](https://github.com/HymEric/latest-development-of-ISR-VSR)
- https://github.com/ptkin/Awesome-Super-Resolution
- https://github.com/ChaofWang/Awesome-Super-Resolution
- https://keras.io/examples/vision/super_resolution_sub_pixel/
- [Image Super-Resolution: A Comprehensive Review (2020)](https://blog.paperspace.com/image-super-resolution/ )


## Talks
- #TALK [How Super Resolution Works (2019)](https://www.youtube.com/watch?v=KULkSwLk62I)
- #TALK [Can you enhance that? Single Image Super Resolution (Pydata 2019)](https://www.youtube.com/watch?v=lmUxbRY7H2I)

## Code
- #CODE [BasicSR: Open Source Image and Video Restoration Toolbox for Super-resolution, Denoise, Deblurring (Pytorch)](https://github.com/xinntao/BasicSR)
	- It includes EDSR, RCAN, SRResNet, SRGAN, ESRGAN, EDVR, etc
- #CODE [Single Image Super Resolution benchmark (Keras)](https://github.com/hieubkset/Keras-Image-Super-Resolution)
	- EDSR, SRGAN, SRFeat, RCAN, ESRGAN and ERCA (not published)
- #CODE [Single Image Super-Resolution with EDSR, WDSR and SRGAN (Keras)](https://github.com/krasserm/super-resolution)
	- http://krasserm.github.io/2019/09/04/super-resolution/


## References
### Review Papers
- #PAPER [Deep Learning for Single Image Super-Resolution: A Brief Review (2018)](https://arxiv.org/abs/1808.03344)
- #PAPER [A Deep Journey into Super-resolution: A survey (Anwar 2020)](https://arxiv.org/abs/1904.07523)
	- https://github.com/saeed-anwar/SRsurvey
- #PAPER [Deep Learning for Image Super-resolution: A Survey (Wang 2020)](https://arxiv.org/abs/1902.06068 )
- #PAPER [NTIRE 2020 Challenge on Perceptual Extreme Super-Resolution: Methods and Results (Zhang 2020)](https://arxiv.org/abs/2005.01056)
	- https://data.vision.ee.ethz.ch/cvl/ntire20/
	- Jointly with NTIRE 2020 workshop we have an NTIRE challenge on perceptual extreme super-resolution, that is,the task of super-resolving an LR image to a perceptually pleasant HR image with a magnification factor x16
- #PAPER [A Comprehensive Review of Deep Learning-based Single Image Super-resolution (Bashir 2021)](https://arxiv.org/abs/2102.09351)


### CNN-based
- #PAPER [Image Super-Resolution Using Deep Convolutional Networks, SRCNN (Dong 2015)](https://arxiv.org/abs/1501.00092)
	- #CODE https://github.com/MarkPrecursor/SRCNN-keras
	- #CODE https://github.com/yukia18/srcnn-keras
- #PAPER [Accurate Image Super-Resolution Using Very Deep Convolutional Networks (2015)](http://arxiv.org/abs/1511.04587)
- #PAPER [Deep Networks for Image Super-Resolution with Sparse Prior (Wang 2015)](http://www.ifp.illinois.edu/~dingliu2/iccv15/)
	- http://www.ifp.illinois.edu/~dingliu2/iccv15/iccv15.pdf
- #PAPER [FSRCNN - Accelerating the Super-Resolution Convolutional Neural Network (Dong 2016)](https://arxiv.org/abs/1608.00367)
	- http://mmlab.ie.cuhk.edu.hk/projects/FSRCNN.html
	- Uses deconvolution layers (transposed convolution)
	- #CODE https://github.com/GeorgeSeif/FSRCNN-Keras
- #PAPER [Deconvolution and Checkerboard Artifacts (Odena 2016)](https://distill.pub/2016/deconv-checkerboard/)
	- Identifies the learned upsample operation (often called deconvolutions) in generative networks as a source of noise
	- Overall lesson here is that if you use transposed convolutions, be careful that your kernel size is a multiple of your stride
	- However if you use a nearest neighbor or bilinear upsample approach followed by a convolution (termed the ‘resize convolution’) checkerboard artifacts should not appear
	- They have more succes with nearest neighbor than with bilinear, possibly because bilinear upsampling smooths away important high frequency signals
- #PAPER [Perceptual Losses for Real-Time Style Transfer and Super-Resolution (Johnson 2016)](http://arxiv.org/abs/1603.08155)
	- http://cs.stanford.edu/people/jcjohns/papers/fast-style/fast-style-supp.pdf
- #PAPER [ESPCN - Real-Time Single Image and Video Super-Resolution Using an Efficient Sub-Pixel Convolutional Neural Network (Shi 2016)](https://arxiv.org/abs/1609.05158)
	- https://medium.datadriveninvestor.com/review-espcn-real-time-sr-super-resolution-8dceca249350
	- #CODE https://keras.io/examples/vision/super_resolution_sub_pixel/
	- [SubPixelUpscaling implementation here](https://github.com/pavitrakumar78/Anime-Face-GAN-Keras/blob/master/misc_layers.py)
	- [Subpixel convolution is the same as pixel-shuffle](https://nico-curti.github.io/NumPyNet/NumPyNet/layers/pixelshuffle_layer.html)
	- A drawback of the interpolation upsampling is that upsampling errors are introduced that can be hard to correct sub-sequently
	- The idea of pixel shuffling is to rearrange the pixels of multiple low-resolution images, or in this case feature activations, to one high-resolution out-put image by periodic shuffling of the image points. It thus represents a learnable upsampling operation
	- Through the constant periodicity, the previous operations of the neural network can learn to distribute content across the feature dimension which is then shuffled to yield the high-resolution output
	- This allows to process the image entirely in low-resolution space
- #PAPER [Checkerboard artifact free sub-pixel convolution: A note on sub-pixel convolution, resize convolution and convolution resize (Aitken 2017)](https://arxiv.org/abs/1707.02937)
	- #CODE https://github.com/Golbstein/EDSR-Keras/blob/master/subpixel.py
- #PAPER [EDSR - Enhanced Deep Residual Networks for Single Image Super-Resolution (Lim 2017)](https://arxiv.org/abs/1707.02921)
	- #CODE https://github.com/Golbstein/EDSR-Keras
	- #CODE https://github.com/hieubkset/Keras-Image-Super-Resolution
- #PAPER [Pixel Deconvolutional Networks (Gao 2017)](https://arxiv.org/abs/1705.06820)
- #PAPER [RDN - Residual Dense Network for Image Super-Resolution (Zhang 2018)](https://arxiv.org/abs/1802.08797)
	- #CODE https://github.com/idealo/image-super-resolution
	- #CODE https://github.com/hengchuan/RDN-TensorFlow
- #PAPER [WDSR - Wide Activation for Efficient and Accurate ImageSuper-Resolution (Yu 2018)](https://arxiv.org/abs/1808.08718)
- #PAPER [RecResNet: A Recurrent Residual CNN Architecture for Disparity Map Enhancement (Batsos 2018)](https://ieeexplore.ieee.org/document/8490974)
	- https://mordohai.github.io/public/Batsos_RecResNet18.pdf
	- #CODE https://github.com/kbatsos/RecResNet
- #PAPER [RCAN - Image Super-Resolution Using Very Deep Residual Channel Attention Networks (Zhang 2018)](https://arxiv.org/abs/1807.02758)
	- #CODE https://github.com/yulunzhang/RCAN
- #PAPER [Fast and Accurate Image Super-Resolution with Deep Laplacian Pyramid Networks (Lai 2018)](http://vllab.ucmerced.edu/wlai24/LapSRN/)
- #PAPER [Super-Resolution using Convolutional Neural Networks without Any Checkerboard Artifacts (Sugawara 2018)](https://arxiv.org/abs/1806.02658v1)
- #PAPER [Single Image Super Resolution based on a Modified U-net with Mixed Gradient Loss (Lu, 2019)](https://arxiv.org/abs/1911.09428)
- #PAPER [Densely Residual Laplacian Super-Resolution (Anwar 2019)](https://arxiv.org/abs/1906.12021)
	- #CODE https://github.com/saeed-anwar/DRLN
- #PAPER [Hyperspectral Image Super-Resolution with 1D–2D Attentional Convolutional Neural Network (Li 2019)](https://www.mdpi.com/2072-4292/11/23/2859/htm)
- #PAPER [Deep Learning for Multiple-Image Super-Resolution (Kawulok 2019)](https://arxiv.org/abs/1903.00440)
- #PAPER [RUNet: A Robust UNet Architecture for Image Super-Resolution (Hu 2019)](https://openaccess.thecvf.com/content_CVPRW_2019/papers/WiCV/Hu_RUNet_A_Robust_UNet_Architecture_for_Image_Super-Resolution_CVPRW_2019_paper.pdf)
- #PAPER [Learned Image Downscaling for Upscaling using Content Adaptive Resampler (Sun 2019)](https://arxiv.org/abs/1907.12904)
	- #CODE https://github.com/sunwj/CAR
	- https://paperswithcode.com/paper/learned-image-downscaling-for-upscaling-using
	- The proposed resampler network generates content adaptive image resampling kernels that are applied to the original HR input to generate pixels on the downscaled image
	- Moreover, a differentiable upscaling (SR) module is employed to upscale the LR result into its underlying HR counterpart
	- By back-propagating the reconstruction error down to the original HR input across the entire framework to adjust model parameters, the proposed framework achieves a new state-of-the-art SR performance through upscaling guided image resamplers which adaptively preserve detailed information that is essential to the upscaling
- #PAPER [Image Super-Resolution Using Attention Based DenseNet with Residual Deconvolution (Li 2019)](https://arxiv.org/abs/1907.05282)
- #PAPER [Meta-SR: A Magnification-Arbitrary Network for Super-Resolution (Hu 2019)](https://arxiv.org/abs/1903.00875)
	- #CODE https://github.com/XuecaiHu/Meta-SR-Pytorch
	- #CODE https://github.com/smallsunsun1/Meta-SR/
	- #CODE https://github.com/jason71995/meta_sr/
	- Continuous, arbitrary scaling
- #PAPER [Pixel Transposed Convolutional Networks (Gao 2019)](https://ieeexplore.ieee.org/document/8618415)
	- The pixel transposed convolutional layer (PixelTCL) is proposed to establish direct relationships among adjacent pixels on the up-sampled feature map
	- PixelTCL can largely overcome the checkerboard problem suffered by regular transposed convolutional operations
- #PAPER [A Very Deep Spatial Transformer Towards Robust Single Image Super-Resolution (Jiang 2019)](https://ieeexplore.ieee.org/abstract/document/8679959)
- #PAPER [ASDN: A Deep Convolutional Network for Arbitrary Scale Image Super-Resolution (Shen 2020)](https://arxiv.org/abs/2010.02414v1)
- #PAPER [LIIF - Learning Continuous Image Representation with Local Implicit Image Function (Chen 2020)](https://arxiv.org/abs/2012.09161)
	- https://yinboc.github.io/liif/
	- #CODE https://github.com/yinboc/liif
	- Continuous, arbitrary scaling
- #PAPER [Fixed smooth convolutional layer for avoiding checkerboard artifacts in CNNs (Kinoshita 2020)](https://arxiv.org/abs/2002.02117v1)
- #PAPER [Efficient Image Super-Resolution Using Pixel Attention (Zhao 2020)](https://arxiv.org/abs/2010.01073) ^srwithpixelattention
	-  #CODE See code in [CNNs](AI/Deep%20learning/CNNs.md)
	-  #CODE https://github.com/zhaohengyuan1/PAN
- #PAPER [Dense U-net for super-resolution with shuffle pooling layer (Lu 2021)](https://arxiv.org/abs/2011.05490)
- #PAPER [OverNet: Lightweight Multi-Scale Super-Resolution with Overscaling Network (Behjati 2021)](https://arxiv.org/abs/2008.02382)
	- https://www.youtube.com/watch?v=_YAn5TaIJfM


### GAN-based
- #PAPER [SRGAN: Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network (Ledig 2016)](https://arxiv.org/abs/1609.04802)
	- #CODE https://github.com/idealo/image-super-resolution
	- #CODE https://github.com/tensorlayer/srgan
	- #CODE https://github.com/leftthomas/SRGAN
	- #TALK https://www.youtube.com/watch?v=BXIR_SVCrsE
	- First proposed the perceptual loss: content loss + adversarial loss
		- content loss ensures high-level content is preserved by computing the MSE in the VGG feature-space (instead of pixel image space)
		- adversarial loss ensures the reconstructed images look real (textures detail)
	- Model based on VGG architecture and DCGAN
- #PAPER [Class-Conditional Superresolution with GANs (Chen 2017)](http://cs231n.stanford.edu/reports/2017/pdfs/314.pdf )
	- #CODE https://github.com/vincentschen/cgan-superres
- #PAPER [ESRGAN: Enhanced Super-Resolution Generative Adversarial Networks (Wang 2018)](https://arxiv.org/abs/1809.00219)
		- #CODE https://github.com/xinntao/ESRGAN
- #PAPER [tempoGAN: A temporally coherent, volumetric GAN for super-resolution fluid flow (Xie 2018)](https://arxiv.org/abs/1801.09710)
- #PAPER [Unsupervised Single-Image Super-Resolution with Multi-Gram Loss (Shi 2019)](https://www.mdpi.com/2079-9292/8/8/833/htm)
- #PAPER [TecoGAN: Learning Temporal Coherence via Self-Supervision for GAN-based Video Generation (Chu 2020)](https://ge.in.tum.de/publications/2019-tecogan-chu/)
	- #CODE https://github.com/thunil/TecoGAN
	- [Paper explained](https://www.youtube.com/watch?v=MwCgvYtOLS0)
- #PAPER [TSRGAN: Generative Adversarial Network for Image Super-Resolution Combining Texture Loss (Jiang 2020)](https://www.mdpi.com/2076-3417/10/5/1729/htm)
- #PAPER [Residual Channel Attention Generative Adversarial Network for Image Super-Resolution and Noise Reduction (Cai 2020)](https://arxiv.org/abs/2004.13674)
- #PAPER [Meta-SRGAN - Arbitrary Scale Super-Resolution for Brain MRI Images (Tan 2020)](https://arxiv.org/abs/2004.02086)
	- #CODE https://github.com/pancakewaffles/metasrgan-tutorial/
- #PAPER [MSG-GAN: Multi-Scale Gradients for Generative Adversarial Networks (Karnewar 2020)](https://arxiv.org/abs/1903.06048)
- #PAPER [MRI Super-Resolution with GAN and 3D Multi-Level DenseNet: Smaller, Faster, and Better (Chen 2020)](https://arxiv.org/abs/2003.01217)
- #PAPER [Real-ESRGAN: Training Real-World Blind Super-Resolution with Pure Synthetic Data (Wnag 2021)](https://arxiv.org/abs/2107.10833v1) ^real-esrgan
	- #CODE https://github.com/xinntao/Real-ESRGAN
	- Super-resolution with a hint of image restoration
	- Proposed a high-order degradation modeling process to better simulate complex real-world degradations (blur, downsampling, noise, etc and combinations)


### Transformer-based
- #PAPER [Learning Texture Transformer Network for Image Super-Resolution (Yang 2020)](https://arxiv.org/abs/2006.04139) ^ttsr
	- #CODE https://github.com/researchmm/TTSR
	- Texture Transformer Network for Image Super-Resolution (TTSR)
	- LR and Ref images are formulated as queries and keys in a transformer, respectively
	- The proposed texture transformer consists of a learnable texture extractor which learns a jointly feature embedding for further attention computation and two attention based modules which transfer HR textures from the Ref image. 
	- Furthermore, the proposed texture transformer can be stacked in a cross-scale way with the proposed CSFI module to learn a more powerful feature representation


### Diffusion models-based
- #PAPER [Image Super-Resolution via Iterative Refinement (Saharia 2021)](https://arxiv.org/abs/2104.07636)
	- https://iterative-refinement.github.io/
	- Related to [Diffusion models](AI/Deep%20learning/Diffusion%20models.md)
	- SR3 is inspired by recent work on Denoising Diffusion Probabilistic Models (DDPM) and denoising score matching
	- SR3 adapts denoising diffusion probabilistic models to conditional image generation and performs super-resolution through a stochastic denoising process
	- Inference starts with pure Gaussian noise and iteratively refines the noisy output using a U-Net model trained on denoising at various noise levels
	- #CODE https://github.com/Janspiry/Image-Super-Resolution-via-Iterative-Refinement
	- #CODE https://paperswithcode.com/paper/image-super-resolution-via-iterative