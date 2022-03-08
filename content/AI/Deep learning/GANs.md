---
title: "Generative Adversarial Networks (GANs)"
disableToc: false 
---

## Resources
- A GAN consists of two networks; a generator (G) and a discriminator (D), given a set of training examples, G will generate outputs and D will classify them as either being from the same distribution as the training examples or not. In doing so D is optimized so as to be able to discriminate between examples from the training example and from the generator network which in turn is optimized to fool D into classifying its output as being drawn from the training examples. After such training G can now generate samples with properties very similar to those of the training examples. GANs tend to be devilishly hard to train. 
- List of papers and other on Generative Adversarial Networks: https://github.com/pshams55/GAN-Case-Study
- Generative Adversarial Networks: https://spectra.pub/ml/gans
- #TALK GANs for Good - A Virtual Expert Panel by DeepLearning.AI: https://www.youtube.com/watch?v=9d4jmPmTWmc
- Generative adversarial networks: https://deepgenerativemodels.github.io/notes/gan/ 
- Generative adversarial networks for beginners: https://www.oreilly.com/learning/generative-adversarial-networks-for-beginners
- Intuitive explanation of GANs. Subtypes. https://tryolabs.com/blog/2016/12/06/major-advancements-deep-learning-2016/
- https://adeshpande3.github.io/adeshpande3.github.io/Deep-Learning-Research-Review-Week-1-Generative-Adversarial-Nets
- http://www.openias.org/hybrid-generative-discriminative
- http://edwardlib.org/tutorials/gan
- Play with GANs in your browser: https://poloclub.github.io/ganlab/
- Do GANs actually do distribution learning?: http://www.offconvex.org/2017/07/06/GANs3/
- The GAN Zoo - A list of all named GANs! https://deephunt.in/the-gan-zoo-79597dc8c347
- Advances in Generative Adversarial Networks: https://beyondminds.ai/advances-in-generative-adversarial-networks-gans/ ^advancesingans
	- Drawbacks of using GANs: Mode collapse, Convergence, Quality evaluation, Metrics
	- Techniques for Improving Performance:
		- Alternative Loss Functions: One of the most popular fixes to the shortcomings of GANs is the Wasserstein GAN. It essentially replaces the Jensen Shannon divergence of conventional GANs with the Earth Mover distance (Wasserstein-1 distance or EM distance)
		- Two Timescale Update Rule (TTUR): In this method, we use a different learning rate for the discriminator and the generator. Typically, a slower update rule is used for the generator and a faster update rule is used for the discriminator
		- Gradient Penalty: In the paper [GANs#^wgangp](#%5Ewgangp), a simple gradient penalty was introduced which is added to the loss function to avoid exploding vanishing gradients and optimization issues (caused by weight clipping)
		- Spectral Normalization: weight normalization technique that is typically used on the Discriminator to enhance the training process
		- Unrolling and Packing: http://aiden.nibali.org/blog/2017-01-18-mode-collapse-gans/
		- Stacking GANs: use multiple GANs placed consecutively, where each GAN solves an easier version of the problem.  For instance, FashionGAN used two GANs to perform localized image translation. Progressive GANs (ProGANs) can generate high quality images of excellent resolution.
		- Relativistic GANs: Conventional GANs measure the probability of the generated data being real. Relativistic GANs measure the probability of the generated data being “more realistic” than the real data. We can measure this “relative realism” using an appropriate distance measure, as mentioned in the RGAN [GANs#^190c58](#%5E190c58) paper
		- Self Attention Mechanism [GANs#^sagan](#%5Esagan):  The authors of Self Attention GANs claim that convolutions used for generating images look at information that are spread locally. That is, they miss out on relationships that span globally due to their restrictive receptive field. Self-Attention Generative Adversarial Network allows attention-driven, long-range dependency modeling for image generation tasks. 
		- Miscellaneous Techniques: Feature Matching, Mini Batch Discrimination, Historical Averaging, One-sided Label Smoothing, Virtual Batch Normalization. See [GANs#^improvedgans](#%5Eimprovedgans)

## Courses
- #COURSE Generative Adversarial Networks ( DeepMind x UCL | Deep Learning Lectures | 9/12): https://www.youtube.com/watch?v=wFsI2WqUfdA&t=850s

## Code
- #CODE Keras-GAN - Collection of Keras implementations of GANs: https://github.com/eriklindernoren/Keras-GAN
- #CODE Pytorch-GAN - Collection of Pytorch implementations of GANs: https://github.com/eriklindernoren/PyTorch-GAN
- #CODE Generative models in Tensorflow and Pytorch: https://github.com/wiseodd/generative-models
- #CODE Tensorflow generative model collection: https://github.com/hwalsuklee/tensorflow-generative-model-collections
- #CODE ydata-synthetic: https://github.com/ydataai/ydata-synthetic
	- This repository contains material related with GANs for synthetic data generation, in particular regular tabular data and time-series


## References
Review papers:
- #PAPER A Survey on Generative Adversarial Networks: Variants, Applications,and Training (Jabbar 2020): https://arxiv.org/abs/2006.05132
- #PAPER A Review on Generative Adversarial Networks: Algorithms, Theory, and Applications (Gui 2020): https://arxiv.org/abs/2001.06937

- #PAPER Generative Adversarial Networks (Goodfellow 2014): http://arxiv.org/abs/1406.2661
	- Paper explained: https://www.youtube.com/watch?v=eyxmSmjmNS0
- #PAPER GAN to convert text descriptions into images (Reed 2016): https://arxiv.org/abs/1605.05396
- #PAPER Unsupervised representation learning with GANs (Radford 2016): https://arxiv.orga/abs/1511.06434v2
	- Although GANs were already introduced in 2014 by Ian Goodfellow, it wasn't until the publication of this paper detailing a deep convolutional architecture (DCGAN) that GANs really took off 
	- https://www.tensorflow.org/tutorials/generative/dcgan
	- https://towardsdatascience.com/dcgans-deep-convolutional-generative-adversarial-networks-c7f392c2c8f8
	- #CODE https://github.com/tensorflow/models/blob/master/research/slim/nets/dcgan.py
- #PAPER Deconvolution and Checkerboard Artifacts (Odena 2016): https://distill.pub/2016/deconv-checkerboard/
- #PAPER InfoGAN: Interpretable Representation Learning by Information Maximizing Generative Adversarial Nets (Chen 2016): https://arxiv.org/abs/1606.03657
	- https://wiseodd.github.io/techblog/2017/01/29/infogan/
- #PAPER Checkerboard artifact free sub-pixel convolution: A note on sub-pixel convolution, resize convolution and convolution resize (Aitken 2017): https://arxiv.org/abs/1707.02937
- #PAPER Wasserstein GAN (Arjovsky 2017): https://arxiv.org/abs/1701.07875
	- From GAN to Wasserstein GAN: https://lilianweng.github.io/lil-log/2017/08/20/from-GAN-to-WGAN.html#wasserstein-gan-wgan 
- #PAPER Improved Training of Wasserstein GANs (Gulrajani 2017): https://arxiv.org/abs/1704.00028 ^wgangp
- #PAPER Bayesian GAN (Saatchi 2017): https://arxiv.org/abs/1705.09558
	- #CODE https://github.com/andrewgordonwilson/bayesgan
- #PAPER WaterGAN: Unsupervised Generative Network to Enable Real-time Color Correction of Monocular Underwater Images (Li 2017): https://arxiv.org/abs/1702.07392 
- #PAPER A Style-Based Generator Architecture for Generative Adversarial Networks, StyleGAN (Karras 2018): https://arxiv.org/abs/1812.04948 
	- #TALK https://youtu.be/kSLJriaOumA 
	- #CODE https://github.com/NVlabs/stylegan 
	- FFHQ: https://github.com/NVlabs/ffhq-dataset 
- #PAPER The relativistic discriminator: a key element missing from standard GAN (Jolicoeur-Martineau 2018): https://arxiv.org/abs/1807.00734 ^190c58
- #PAPER From GAN to WGAN (Wenb 2019): https://arxiv.org/abs/1904.08994
- #PAPER Time Series Simulation by Conditional Generative Adversarial Net (Fu 2019): https://arxiv.org/abs/1904.11419
- #PAPER HoloGAN: Unsupervised learning of 3D representations from natural images (Nguyen-Phuoc 2019): https://arxiv.org/abs/1904.01326 
	- https://www.monkeyoverflow.com/#/hologan-unsupervised-learning-of-3d-representations-from-natural-images/ 
	- #TALK https://www.youtube.com/watch?v=z2DnFOQNECM
- #PAPER Implicit competitive regularization in GANs (Schafer 2020): https://arxiv.org/abs/1910.05852
- #PAPER Training Generative Adversarial Networks with Limited Data (Karras 2020): https://arxiv.org/abs/2006.06676
- #PAPER Gradient-Guided Dynamic Efficient Adversarial Training (Waag 2021): https://arxiv.org/abs/2103.03076
	- #CODE https://github.com/locuslab/fast_adversarial
	- The goal of DEAT is to improve adversarial training while maintaining effectiveness. It begins by training one batch replay and gradually increases it during training
	- This method reduces large amount of computation when doing backpropagation and consequently achieves a more efficient training paradigm


## Subtopics

### GANs for super-resolution
See [Super-resolution#GAN-based](AI/Computer%20Vision/Super-resolution.md#GAN-based)


### GANs for missing data, imputation and inpainting
See [Inpainting#GAN-based](AI/Computer%20Vision/Inpainting.md#GAN-based)


### Image-to-image translation. Conditional GANs
See [Image-to-image translation#GAN-based](AI/Computer%20Vision/Image-to-image%20translation.md#GAN-based)


### GANs for spatio-temporal data generation
- #PAPER COT-GAN: Generating Sequential Data via Causal Optimal Transport (Xu 2020): https://arxiv.org/abs/2006.08571
- #PAPER SPATE-GAN: Improved Generative Modeling of Dynamic Spatio-Temporal Patterns with an Autoregressive Embedding Loss (Klemmer 2021): https://arxiv.org/abs/2109.15044# ^spate-gan
	- #CODE https://github.com/konstantinklemmer/spate-gan


### GANs for representation learning and image synthesis 
- #PAPER Deep Generative Image Models using a Laplacian Pyramid of Adversarial Networks, Laplacian GAN (Denton 2015): https://arxiv.org/abs/1506.05751
- #PAPER Adversarial feature learning, BiGAN (Donahue 2017): https://arxiv.org/abs/1605.09782
- #PAPER Large Scale Adversarial Representation Learning, BigBiGAN (Donahue 2019): https://arxiv.org/abs/1907.02544
- #PAPER Large Scale GAN Training for High Fidelity Natural Image Synthesis, BigGAN (Brock 2019): https://arxiv.org/abs/1809.11096
- #PAPER Self-Attention GANs, SAGAN (Zhang 2019): https://arxiv.org/abs/1805.08318 ^sagan
	- #CODE https://github.com/brain-research/self-attention-gan
- #PAPER In-domain GAN Inversion for Real Image Editing (Zhu 2020): https://genforce.github.io/idinvert/
	- Paper explained: https://www.youtube.com/watch?v=2qMw8sOsNg0
- #PAPER High-Fidelity Generative Image Compression (Mentzer 2020): https://arxiv.org/abs/2006.09965
	- https://hific.github.io/
- #PAPER Generative Adversarial Networks for Image and Video Synthesis: Algorithms and Applications (Liu 2020): https://arxiv.org/abs/2008.02793
- #PAPER Image Synthesis with Adversarial Networks: a Comprehensive Survey and Case Studies (Shamsolmoali 2020): https://arxiv.org/abs/2012.13736
- #PAPER Cross-Modal Contrastive Learning for Text-to-Image Generation (Zhang 2021): https://arxiv.org/abs/2101.04702
	- https://ai.googleblog.com/2021/05/cross-modal-contrastive-learning-for.html
	- text-to-image generation by learning to maximize the mutual information between image and text using inter-modal (image-text) and intra-modal (image-image) contrastive losses
- #PAPER TriGAN: image-to-image translation for multi-source domain adaptation (Roy 2021): https://link.springer.com/article/10.1007/s00138-020-01164-4
	- approach for multi-source domain adaptation (MSDA) based on generative adversarial networks
- #PAPER Sketch Your Own GAN (Wang 2021): https://arxiv.org/abs/2108.02774
- #PAPER Instance-Conditioned GAN (Casanova 2021): https://arxiv.org/abs/2109.05070
	- #CODE https://paperswithcode.com/paper/instance-conditioned-gan?from=n17


### Semi-supervised GANs
- #PAPER Improved Techniques for Training GANs (Saliman 2016): https://arxiv.org/abs/1606.03498 ^improvedgans
	- https://towardsdatascience.com/semi-supervised-learning-with-gans-9f3cb128c5e
	- https://hjweide.github.io/semi-supervised-dcgan
- #PAPER Semi-Supervised Learning with Generative Adversarial Networks (Odena 2016): https://arxiv.org/abs/1606.01583
	- #CODE https://github.com/tryambak2019/SGAN
- #PAPER Semi and Weakly Supervised Semantic Segmentation Using Generative Adversarial Network (Suoly 2017): https://arxiv.org/abs/1703.09695
- #PAPER Semi-supervised Learning in Generative Adversarial Networks, review (2018): https://farzadab.github.io/assets/projects/pdf/Review__SSL_in_GANs.pdf
    - The GAN framework can be integrated with almost any available neural network classifier in order to make use of unlabeled data


### Few/one-shot learning GANs 
See [One, few-shot learning#Few one-shot learning GANs](AI/One,%20few-shot%20learning.md#Few%20one-shot%20learning%20GANs)


### GANs for anomaly detection
- #PAPER A Survey on GANs for Anomaly Detection (Di Mattia 2019): https://arxiv.org/abs/1906.11632 
- #PAPER TadGAN: Time Series Anomaly Detection Using Generative Adversarial Networks (Geiger 2020): https://arxiv.org/abs/2009.07769
	- #CODE [[#^oriontfanomalies]]
	- https://analyticsindiamag.com/hands-on-guide-to-tadgan-with-python-codes/
