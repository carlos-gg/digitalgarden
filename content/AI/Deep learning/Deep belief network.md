---
title: "Deep belief network"
disableToc: false 
---

# Resources
- In machine learning, a deep belief network (DBN) is a generative graphical model, or alternatively a type of deep neural network, composed of multiple layers of latent variables("hidden units"), with connections between the layers but not between units within each layer. DBNs can be viewed as a composition of simple, unsupervised networks such as restricted Boltzmann machines (RBMs) or autoencoders, where each sub-network's hidden layer serves as the visible layer for the next.
- #TALK Deep Belief Nets (Hinton): https://www.cs.toronto.edu/~hinton/nipstutorial/nipstut3.pdf
- Deep-Belief Networks: https://wiki.pathmind.com/deep-belief-network
	- A deep-belief network can be defined as a stack of restricted Boltzmann machines, in which each RBM layer communicates with both the previous and subsequent layers. The nodes of any single layer don’t communicate with each other laterally.
	- This stack of RBMs might end with a a Softmax layer to create a classifier, or it may simply help cluster unlabeled data in an unsupervised learning scenario.
	- With the exception of the first and final layers, each layer in a deep-belief network has a double role: it serves as the hidden layer to the nodes that come before it, and as the input (or “visible”) layer to the nodes that come after. It is a network built of single-layer networks.
	- Deep-belief networks are used to recognize, cluster and generate images, video sequences and motion-capture data. A continuous deep-belief network is simply an extension of a deep-belief network that accepts a continuum of decimals, rather than binary data. They were introduced by Geoff Hinton and his students in 2006.