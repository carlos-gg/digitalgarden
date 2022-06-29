---
title: "Autoencoders"
---

> An autoencoder is a type of artificial neural network used to learn efficient codings of unlabeled data (unsupervised learning). The encoding is validated and refined by attempting to regenerate the input from the encoding. The autoencoder learns a representation (encoding) for a set of data, typically for dimensionality reduction, by training the network to ignore insignificant data (“noise”)

## Resources
- https://en.wikipedia.org/wiki/Autoencoder
- [Dimensionality Reduction](https://www.cs.toronto.edu/~hinton/science.pdf)
- The classical approach for unsupervised learning using neural networks. The basic version consists of a Multilayer Perceptron (MLP) where the input and output layer have the same size and a smaller hidden layer is trained to recover the input. Once trained, the output from the hidden layer corresponds to data representation that can be useful for clustering, dimensionality reduction, improving supervised classification and even for data compression.
- https://blog.keras.io/building-autoencoders-in-keras.html
- https://blog.insightdatascience.com/isee-removing-eyeglasses-from-faces-using-deep-learning-d4e7d935376f
- https://github.com/nanopony/keras-convautoencoder

### VAEs
- Variational autoencoders are generative models. Traditional autoencoders that just do reconstruction don’t have an obvious generative interpretation. There are some cases in between, like denoising autoencoders, where it is possible to construct a Markov chain that uses the autoencoder to sample from the data distribution, but the autoencoder doesn’t give direct explicit access to an estimate of the density or the ability to sample directly.
- VAE is a type of autoencoder with added constraints on the encoded representations being learned. More precisely, it is an autoencoder that learns a latent variable model for its input data. So instead of letting your neural network learn an arbitrary function, you are learning the parameters of a probability distribution modeling your data. If you sample points from this distribution, you can generate new input data samples: a VAE is a "generative model".
- [Introduction to deep generative modeling: Variational Auto-Encoders](https://jmtomczak.github.io/blog/4/4_VAE.html)
- [Introduction to deep generative modeling: Priors in VAEs](https://jmtomczak.github.io/blog/7/7_priors.html)
- [Introduction to deep generative modeling: Hierarchical VAEs](https://jmtomczak.github.io/blog/9/9_hierarchical_lvm_p1.html)
- [Variational Autoencoders Explained](http://kvfrans.com/variational-autoencoders-explained/)
- [Intuitively understanding VAEs](https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf)
- [An Intuitive Comparison of Autoencoders with Variational Autoencoders](https://thilospinner.com/towards-an-interpretable-latent-space/)
- http://blog.fastforwardlabs.com/post/148842796218/introducing-variational-autoencoders-in-prose-and
- [Variational Autoencoders (youtube)](https://www.youtube.com/watch?v=9zKuYvjFFS8)
- [From Autoencoder to Beta-VAE](https://lilianweng.github.io/lil-log/2018/08/12/from-autoencoder-to-beta-vae.html)


## Code
- #CODE [benchmark_VAE](https://github.com/clementchadebec/benchmark_VAE)
	- This library implements some of the most common (Variational) Autoencoder models
	- https://pythae.readthedocs.io/en/latest/
	- #PAPER [Pythae: Unifying Generative Autoencoders in Python -- A Benchmarking Use  Case (Chadebec 2022)](https://arxiv.org/pdf/2206.08309v1)


## References
- #PAPER [Stacked Denoising Autoencoders: Learning Useful Representations in a Deep Network with a Local Denoising Criterion (Vincent 2010)](https://www.jmlr.org/papers/v11/vincent10a.html)
- #PAPER [Adversarial Autoencoders with Constant-Curvature Latent Manifolds (Grattarola 2018)](https://arxiv.org/abs/1812.04314)
- #PAPER [Image-To-Image Translation Using a Cross-Domain Auto-Encoder and Decoder (Yoo 2019)](https://www.mdpi.com/2076-3417/9/22/4780/htm )
	- Early image-to-image translation methods used convolutional neural networks (CNN), which learn to minimize the loss of a pixel value between the source domain image and the target domain image but had the limitation of failing to produce more photorealistic images 
	- Unlike other approaches… our method is not limited to a specific task, nor do we rely on predefined relationships between the source and target domains. Our method can be applied to make a general-domain solution for many image-to-image translation tasks. 

### Variational Autoencoders (VAE)
- #PAPER [Auto-Encoding Variational Bayes (Kingma 2014)](https://arxiv.org/abs/1312.6114)
- #PAPER [An Introduction to Variational Autoencoders (Kingma 2019)](https://arxiv.org/abs/1906.02691)
- #PAPER [NVAE: A Deep Hierarchical Variational Autoencoder (Vahdat 2020)](https://arxiv.org/abs/2007.03898)
	- [Paper explained](https://www.youtube.com/watch?v=x6T1zMSE4Ts)
- #PAPER [Deep Attentive Variational Inference (Apostolopoulou 2022)](https://blog.ml.cmu.edu/2022/05/27/deep-attentive-variational-inference/)

### Masked Autoencoders (MAE)
- #PAPER [Masked Autoencoders Are Scalable Vision Learners (He 2021)](https://arxiv.org/abs/2111.06377)
	- #CODE https://github.com/facebookresearch/mae
	- #CODE https://github.com/ariG23498/mae-scalable-vision-learners
	- https://keras.io/examples/vision/masked_image_modeling/
	- Masked autoencoder (MAE) is a simple autoencoding approach that reconstructs the original signal given its partial observation
	- [Paper explained](https://www.youtube.com/watch?v=Dp6iICL2dVI)
	- See [[AI/Deep learning/Transformers]]
- #PAPER [Uniform Masking: Enabling MAE Pre-training for Pyramid-based Vision Transformers with Locality (Li 2022)](https://arxiv.org/abs/2205.10063v1)
	- #CODE https://github.com/implus/um-mae
- #PAPER [ConvMAE: Masked Convolution Meets Masked Autoencoders (Gao 2022)](https://arxiv.org/pdf/2205.03892v2)            
	- #CODE https://github.com/Alpha-VL/ConvMAE
