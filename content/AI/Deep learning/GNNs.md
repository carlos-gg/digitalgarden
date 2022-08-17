---
title: "Graph neural networks (GNNs)"
---

> A GNN is an optimizable transformation on all attributes of the graph (nodes, edges, global-context) that preserves graph symmetries (permutation invariances). Graph Neural networks (GNNs) are being widely adopted for diverse applications and domains. This is in part due to their effectiveness on complex data structures, improved performance and scalability, and availability of approaches

## Resources
- [A Gentle Introduction to Graph Neural Networks](https://distill.pub/2021/gnn-intro/)
- [Must read papers on GNNs](https://github.com/thunlp/GNNPapers)
- [Graph Neural Networks beyond Weisfeiler-Lehman and vanilla Message Passing](https://towardsdatascience.com/graph-neural-networks-beyond-weisfeiler-lehman-and-vanilla-message-passing-bc8605fa59a)
- [Time Series Forecasting with Graph Convolutional Neural Network](https://towardsdatascience.com/time-series-forecasting-with-graph-convolutional-neural-network-7ffb3b70afcf)
- https://medium.com/dair-ai/an-illustrated-guide-to-graph-neural-networks-d5564a551783
- [Graph Convolutional Networks](http://tkipf.github.io/graph-convolutional-networks/)

## Talks
- #TALK [Intro to graph neural networks (ML Tech Talks, Deepmind)](https://www.youtube.com/watch?v=8owQBFAHw7E)

## Code
- #CODE [TensorFlow GNN](https://github.com/tensorflow/gnn)
	- #PAPER [TF-GNN: Graph Neural Networks in TensorFlow (Ferludin 2022)](https://arxiv.org/pdf/2207.03522)
	- https://blog.tensorflow.org/2021/11/introducing-tensorflow-gnn.html
	- https://venturebeat.com/2021/11/18/google-releases-tf-gnn-for-creating-graph-neural-networks-in-tensorflow/
- #CODE [DGL - Deep graph library](https://github.com/dmlc/dgl)
	- https://www.dgl.ai/
- #CODE [Pytorch geometric](https://github.com/rusty1s/pytorch_geometric)
- #CODE [Spektral - Graph Neural Networks with Keras and Tensorflow 2](https://github.com/danielegrattarola/spektral)
- #CODE [Deep Graph Library (DGL)](https://github.com/dmlc/dgl) 
	- http://dgl.ai
	- Python package built to ease deep learning on graph, on top of existing DL frameworks. 
	- It makes implementing graph neural networks (including Graph Convolution Networks, TreeLSTM, and many others) easy while maintaining high computation efficiency.
- #CODE [DIG: A Turnkey Library for Diving into Graph Deep Learning Research](https://github.com/divelab/DIG)
- #CODE [PyTorch Geometric Temporal](https://github.com/benedekrozemberczki/pytorch_geometric_temporal)
	- A Temporal Extension Library for PyTorch Geometric
- #CODE [PyNeuraLogic](https://github.com/LukasZahradnik/PyNeuraLogic)
	- https://pyneuralogic.readthedocs.io/
	- PyNeuraLogic lets you use Python to create Differentiable Logic Programs
	- https://towardsdatascience.com/beyond-graph-neural-networks-with-pyneuralogic-c1e6502c46f7

## References
Review papers:
- #PAPER [A Comprehensive Survey on Graph Neural Networks (Wu 2019)](https://arxiv.org/pdf/1901.00596)
- #PAPER [Graph neural networks: A review of methods and applications (Zhou 2020)](https://www.sciencedirect.com/science/article/pii/S2666651021000012)

- #PAPER [Dynamic Spatial-Temporal Graph Convolutional Neural Networks for Traffic Forecasting (Diao 2019)](https://www.aaai.org/ojs/index.php/AAAI/article/view/3877)
- #PAPER [A Comprehensive Survey on Graph Neural Networks (Wu 2019)](https://arxiv.org/abs/1901.00596)
- #PAPER [Graph Neural Networks for Decentralized Controllers (Gama 2020)](https://arxiv.org/abs/2003.10280 )
- #PAPER [Learning to Simulate Complex Physics with Graph Networks (Sanchez-Gonzalez 2020)](https://arxiv.org/abs/2002.09405)
	- [Two minute papers](https://www.youtube.com/watch?v=2Bw5f4vYL98)
- #PAPER [DeepSphere: a graph-based spherical CNN (Defferrard 2020)](https://arxiv.org/abs/2012.15000) ^deepsphere
	- #CODE https://github.com/deepsphere
- #PAPER [VQ-GNN: A Universal Framework to Scale up Graph Neural Networks using Vector Quantization (Ding 2021)](https://arxiv.org/abs/2110.14363)
- #PAPER [Nested Graph Neural Networks (Zhang 2021)](https://arxiv.org/abs/2110.13197)
	- #CODE https://paperswithcode.com/paper/nested-graph-neural-networks?from=n19
- #PAPER [A Heterogeneous Graph Based Framework for Multimodal Neuroimaging Fusion Learning (Shi 2021)](https://arxiv.org/abs/2110.08465)
	- #CODE https://github.com/shigen97/hebraingnn
	- self-supervised pretraining contrastive strategy based on a heterogeneous brain network to address the potential overfitting problem caused by the conflict between a large parameter size and a small medical data sample size
- #PAPER [Vision GNN: An Image is Worth Graph of Nodes (Han 2022)](https://arxiv.org/pdf/2206.00272v2)
	- #CODE https://github.com/huawei-noah/Efficient-AI-Backbones/tree/master/vig_pytorch
	- proposeD to represent the image as a graph structure and introduce a new Vision GNN (ViG) architecture to extract graph level feature for visual tasks
	- first split the image to a number of patches which are viewed as nodes, and construct a graph by connecting the nearest neighbors
	- the ViG model is built based on the graph representation of images to transform and exchange information among all the nodes
	- ViG consists of two basic modules: Grapher module with graph convolution for aggregating and updating graph information, and FFN module with two linear layers for node feature transformation
	- https://www.marktechpost.com/2022/06/08/researchers-from-china-introduce-vision-gnn-vig-a-graph-neural-network-for-computer-vision-systems/

### Graph convolutional networks
Review papers:
- #PAPER [Graph Neural Networks: A Review of Methods and Applications (Zhou 2019)](https://arxiv.org/abs/1812.08434)

- #PAPER [Structured Sequence Modeling with Graph Convolutional Recurrent Networks (Seo 2016)](https://arxiv.org/abs/1612.07659)
	- Graph Convolutional Recurrent Network (GCRN)
- #PAPER [Spatio-Temporal Graph Convolutional Networks: A Deep Learning Framework for Traffic Forecasting (Yu 2018)](https://arxiv.org/abs/1709.04875 )
