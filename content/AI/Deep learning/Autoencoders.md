---
title: "Autoencoders"
disableToc: false 
---

## Resources
- https://en.wikipedia.org/wiki/Autoencoder
- Dimensionality Reduction: https://www.cs.toronto.edu/~hinton/science.pdf
- The classical approach for unsupervised learning using neural networks. The basic version consists of a Multilayer Perceptron (MLP) where the input and output layer have the same size and a smaller hidden layer is trained to recover the input. Once trained, the output from the hidden layer corresponds to data representation that can be useful for clustering, dimensionality reduction, improving supervised classification and even for data compression.
- https://blog.keras.io/building-autoencoders-in-keras.html
- https://blog.insightdatascience.com/isee-removing-eyeglasses-from-faces-using-deep-learning-d4e7d935376f
- https://github.com/nanopony/keras-convautoencoder


## References
- #PAPER Stacked Denoising Autoencoders: Learning Useful Representations in a Deep Network with a Local Denoising Criterion (Vincent 2010): https://www.jmlr.org/papers/v11/vincent10a.html
- #PAPER Adversarial Autoencoders with Constant-Curvature Latent Manifolds (Grattarola 2018): https://arxiv.org/abs/1812.04314
- #PAPER Image-To-Image Translation Using a Cross-Domain Auto-Encoder and Decoder (Yoo 2019): https://www.mdpi.com/2076-3417/9/22/4780/htm 
	- Early image-to-image translation methods used convolutional neural networks (CNN), which learn to minimize the loss of a pixel value between the source domain image and the target domain image but had the limitation of failing to produce more photorealistic images 
	- Unlike other approaches… our method is not limited to a specific task, nor do we rely on predefined relationships between the source and target domains. Our method can be applied to make a general-domain solution for many image-to-image translation tasks. 


### VAEs
- Variational autoencoders are generative models. Traditional autoencoders that just do reconstruction don’t have an obvious generative interpretation. There are some cases in between, like denoising autoencoders, where it is possible to construct a Markov chain that uses the autoencoder to sample from the data distribution, but the autoencoder doesn’t give direct explicit access to an estimate of the density or the ability to sample directly.
- VAE is a type of autoencoder with added constraints on the encoded representations being learned. More precisely, it is an autoencoder that learns a latent variable model for its input data. So instead of letting your neural network learn an arbitrary function, you are learning the parameters of a probability distribution modeling your data. If you sample points from this distribution, you can generate new input data samples: a VAE is a "generative model".
- Variational Autoencoders Explained: http://kvfrans.com/variational-autoencoders-explained/
- Intuitively understanding VAEs: https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
- An Intuitive Comparison of Autoencoders with Variational Autoencoders: https://thilospinner.com/towards-an-interpretable-latent-space/
- http://blog.fastforwardlabs.com/post/148842796218/introducing-variational-autoencoders-in-prose-and
- Arxiv insights. Variational Autoencoders: https://www.youtube.com/watch?v=9zKuYvjFFS8
- From Autoencoder to Beta-VAE: https://lilianweng.github.io/lil-log/2018/08/12/from-autoencoder-to-beta-vae.html

- #PAPER Auto-Encoding Variational Bayes (Kingma 2014): https://arxiv.org/abs/1312.6114
- #PAPER An Introduction to Variational Autoencoders (Kingma 2019): https://arxiv.org/abs/1906.02691
- #PAPER NVAE: A Deep Hierarchical Variational Autoencoder (Vahdat 2020): https://arxiv.org/abs/2007.03898
	- Paper explained: https://www.youtube.com/watch?v=x6T1zMSE4Ts
