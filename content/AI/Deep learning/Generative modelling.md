---
title: "Generative modeling"
disableToc: false 
---

## Resources
- [Generative models](https://openai.com/blog/generative-models/ )
- [Deep Generative Models](https://www.cs.toronto.edu/~slwang/generative_model.pdf)
- [Taxonomy of Generative Models](https://christineai.blog/taxonomy/)
- Jakub Tomczak [blog](https://jmtomczak.github.io/blog.html):
	- [Introduction to deep generative modeling: Why, Where and How](https://jmtomczak.github.io/blog/1/1_introduction.html)
	- [Introduction to deep generative modeling: Energy-based Models](https://jmtomczak.github.io/blog/11/11_energy_based_models.html)

## Courses
- #COURSE [Deep Generative Modeling: VAEs and GANs (MIT 6.S191)](https://www.youtube.com/watch?v=rZufA635dq4&t=1062s)
- #COURSE [Deep Generative Models (Stanford CS236 - Fall 2021)](https://deepgenerativemodels.github.io/)


## Subtopics
### Autoencoders
See "VAEs" section in [Autoencoders](AI/Deep%20learning/Autoencoders.md)

### GANs
See [GANs](AI/Deep%20learning/GANs.md)

### Normalizing flows
See [Normalizing flows](AI/Deep%20learning/Normalizing%20flows.md)

### Diffusion models
See [Diffusion models](AI/Deep%20learning/Diffusion%20models.md)

### Generative models for Image data
See:
- [Image-to-image translation](AI/Computer%20Vision/Image-to-image%20translation.md)
- "GAN-based" section in [Image-to-image translation](AI/Computer%20Vision/Image-to-image%20translation.md)
- "GANs for representation learning and image synthesis" section in [GANs](AI/Deep%20learning/GANs.md)
- "For Computer Vision" section in [Transformers](AI/Deep%20learning/Transformers.md)
- [Diffusion models](AI/Deep%20learning/Diffusion%20models.md)

- #PAPER [Video Pixel Networks (Kalchbrenner 2016)](https://arxiv.org/abs/1610.00527)
- #PAPER [Pixel RNNs - Pixel Recurrent Neural Networks (van den Oord 2016)](https://arxiv.org/abs/1601.06759)
	- Pixel-RNN presents a novel architecture with recurrent layers and residual connections that predicts pixels across the vertical and horizontal axes. The architecture models the joint distribution of pixels as a product of conditional distributions of horizontal and diagonal pixels. The model achieves state-of-the-art in the generation of natural images.
	- https://medium.com/a-paper-a-day-will-have-you-screaming-hurray/day-4-pixel-recurrent-neural-networks-1b3201d8932d
	- https://christineai.blog/pixelcnn-and-pixelrnn/
- #PAPER [Conditional Image Generation with PixelCNN Decoders (van den Oord 2016)](https://arxiv.org/abs/1606.05328)
	-  https://medium.com/a-paper-a-day-will-have-you-screaming-hurray/day-5-conditional-image-generation-with-pixelcnn-decoders-a8fc68b103a2
	-  #CODE https://www.tensorflow.org/probability/api_docs/python/tfp/distributions/PixelCNN
	-  #CODE https://keras.io/examples/generative/pixelcnn/
- #PAPER [PixelCNN++: Improving the PixelCNN with Discretized Logistic Mixture Likelihood and Other Modifications (Salimans 2017)](https://arxiv.org/abs/1701.05517)
	- #CODE https://github.com/openai/pixel-cnn
	- https://openreview.net/forum?id=BJrFC6ceg&noteId=Bkc_sOZ4l
- #PAPER [FFJORD: Free-form Continuous Dynamics for Scalable Reversible Generative Models (Grathwohl 2018)](https://arxiv.org/abs/1810.01367 )
- #PAPER [Generating Realistic Geology Conditioned on Physical Measurements with Generative Adversarial Networks (Dupont 2018)](http://arxiv.org/abs/1802.03065) ^dupont18
	- Using G and D we want to generate realistic images conditioned on a set of known pixels
	- Total loss is a combination of a Prior loss (high score of generated images from D) and a Contexet loss (generated image should match the known pxs)
	- For the Context loss, a mask is used with smoothing
- #PAPER [Parametric generation of conditional geological realizations using generative neural networks (Chan 2019)](https://link.springer.com/article/10.1007%2Fs10596-019-09850-7) ^chan19
- #PAPER [Parametrization of Stochastic Inputs Using Generative Adversarial Networks With Application in Geology (Chan 2020)](https://www.frontiersin.org/articles/10.3389/frwa.2020.00005/full) ^chan20
- #PAPER [Generative Models as Distributions of Functions (Dupont 2021)](https://arxiv.org/abs/2102.04776)
	- Generative models are typically trained on grid-like data such as images (tied to the underlying grid resolution)
	- Instead of discretized grids, they parametrized individual data points by continuous functions over which they learned distributions --> generative models
	- Coordinate and feature pairs are treated as point clouds (sets with underlying notion of distance). Leveraged the PointConv framekwork 
	- Their model can learn rich distributions of functions independently of data type and resolution. Application to [Super-resolution](AI/Computer%20Vision/Super-resolution.md)
- #PAPER [Score-Based Generative Modeling through Stochastic Differential Equations (Song 2021)](https://arxiv.org/abs/2011.13456v2)
	- #CODE https://paperswithcode.com/paper/score-based-generative-modeling-through-1
- #PAPER [Diverse Generation from a Single Video Made Possible (Haim 2021)](https://arxiv.org/abs/2109.08591)

