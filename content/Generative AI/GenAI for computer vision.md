---
title: Generative AI for computer vision
---

>  See:
>  - [[AI/Generative AI/VLMs|VLMs]]
>  - [[AI/Computer Vision/Deep CV|Deep CV]]

## Resources
- [Text to video model arena](https://artificialanalysis.ai/text-to-video/arena?tab=Arena)
- [How Far is Video Generation from World Model: A Physical Law Perspective](https://phyworld.github.io/)

### Models
- #MODEL https://huggingface.co/genmo/mochi-1-preview
	- Mochi is an open source state-of-the-art video generation model and is released by [Genmo](https://www.linkedin.com/company/genmoai/?lipi=urn%3Ali%3Apage%3Ad_flagship3_feed%3BxZWne9ONSX6J69MqasipVw%3D%3D)
	- [genmo.ai](https://www.genmo.ai/blog?utm_source=pocket_saves)
- #MODEL [Infinite AI Artboard - Recraft](https://www.recraft.ai/)

## Code

## References
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
- #PAPER [Generating Realistic Geology Conditioned on Physical Measurements with Generative Adversarial Networks (Dupont 2018)](http://arxiv.org/abs/1802.03065) 
	- Using G and D we want to generate realistic images conditioned on a set of known pixels
	- Total loss is a combination of a Prior loss (high score of generated images from D) and a Context loss (generated image should match the known pxs)
	- For the Context loss, a mask is used with smoothing
- #PAPER [Parametric generation of conditional geological realizations using generative neural networks (Chan 2019)](https://link.springer.com/article/10.1007%2Fs10596-019-09850-7) 
- #PAPER [Parametrization of Stochastic Inputs Using Generative Adversarial Networks With Application in Geology (Chan 2020)](https://www.frontiersin.org/articles/10.3389/frwa.2020.00005/full) 
- #PAPER [Generative Models as Distributions of Functions (Dupont 2021)](https://arxiv.org/abs/2102.04776)
	- Generative models are typically trained on grid-like data such as images (tied to the underlying grid resolution)
	- Instead of discretized grids, they parametrized individual data points by continuous functions over which they learned distributions --> generative models
	- Coordinate and feature pairs are treated as point clouds (sets with underlying notion of distance). Leveraged the PointConv framekwork 
	- Their model can learn rich distributions of functions independently of data type and resolution. Application to [[AI/Computer Vision/Super-resolution]]
- #PAPER [Score-Based Generative Modeling through Stochastic Differential Equations (Song 2021)](https://arxiv.org/abs/2011.13456v2)
	- #CODE https://paperswithcode.com/paper/score-based-generative-modeling-through-1
- #PAPER [Diverse Generation from a Single Video Made Possible (Haim 2021)](https://arxiv.org/abs/2109.08591)
- #PAPER [Autoregressive Image Generation using Residual Quantization (Lee 2022)](https://arxiv.org/pdf/2203.01941v2)            
	- #CODE https://github.com/kakaobrain/rq-vae-transformer
- #PAPER [GenAI Arena: An Open Evaluation Platform for Generative Models (2024)](https://arxiv.org/pdf/2406.04485v3)
	- https://huggingface.co/spaces/TIGER-Lab/GenAI-Arena