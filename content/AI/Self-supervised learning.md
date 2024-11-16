---
title: "Self-supervised learning"
---

> Self-supervised learning deals with learning from unlabeled sample data. It can be regarded as an intermediate form between [[AI/Supervised Learning/Supervised learning]] and [[AI/Unsupervised learning/Unsupervised learning]]

> See [[AI/Deep learning/Transformers#Self-supervised vision transformers]]

## Resources
- https://github.com/jason718/awesome-self-supervised-learning
- https://en.wikipedia.org/wiki/Self-supervised_learning
- https://hackernoon.com/self-supervised-learning-gets-us-closer-to-autonomous-learning-be77e6c86b5a
- [Self-Supervised Representation Learning](https://lilianweng.github.io/lil-log/2019/11/10/self-supervised-learning.html)
- [Self-Supervised Vision Models (2021, Dr. Ishan Misra - FAIR)](https://www.youtube.com/watch?v=EXJmodhu4_4)
- [Self-supervised learning: The dark matter of intelligence](https://ai.facebook.com/blog/self-supervised-learning-the-dark-matter-of-intelligence/)
	- The general technique of self-supervised learning is to predict any unobserved or hidden part (or property) of the input from any observed or unhidden part of the input
	- [Blog post explained](https://www.youtube.com/watch?v=Ag1bw8MfHGQ&t=6s)
- [Grokking self-supervised (representation) learning: how it works in computer vision and why](https://theaisummer.com/self-supervised-representation-learning-computer-vision/)
- [Self-supervised learning tutorial: Implementing SimCLR with pytorch lightning](https://theaisummer.com/simclr/)
	
## Code
- #CODE [VISSL](https://github.com/facebookresearch/vissl)
	- FAIR's library of extensible, modular and scalable components for SOTA Self-Supervised Learning with images
- #CODE [Solo-learn](https://github.com/vturrisi/solo-learn)
	- A library of self-supervised methods for unsupervised visual representation learning powered by PyTorch Lightning
	- Methods available: Barlow Twins, BYOL, DeepCluster V2, DINO, MoCo V2+, NNCLR, ReSSL, SimCLR + Supervised Contrastive Learning, SimSiam, Swav, VICReg, W-MSE
	- https://arxiv.org/abs/2108.01775v2
- #CODE [Lightly](https://github.com/lightly-ai/lightly)
	- A python library for self-supervised learning on images
- #CODE [OpenSelfSup](https://github.com/open-mmlab/OpenSelfSup)
	- Self-Supervised Learning Toolbox and Benchmark
- #CODE [Curator](https://github.com/spaceml-org/Self-Supervised-Learner)
	- A No-Code, Self-Supervised Learning and Active Labeling Tool to Create Labeled Image Datasets from Petabyte-Scale Imagery


## References
- #PAPER [Self-Supervised Learning of Pretext-Invariant Representations (Misra 2019)](https://arxiv.org/abs/1912.01991)
- #PAPER [A Framework For Contrastive Self-Supervised Learning And Designing A New Approach (Falcon 2020)](https://arxiv.org/abs/2009.00104)
	- https://towardsdatascience.com/a-framework-for-contrastive-self-supervised-learning-and-designing-a-new-approach-3caab5d29619
- #PAPER [RegNet - Designing Network Design Spaces (Radosavovic 2020)](https://arxiv.org/abs/2003.13678v1)
- #PAPER [Transferable Visual Words: Exploiting the Semantics of Anatomical Patterns for Self-supervised Learning (Haghighi 2021)](https://arxiv.org/abs/2102.10680)
- #PAPER [Instance Localization for Self-supervised Detection Pretraining (Yang 2021)](https://arxiv.org/abs/2102.08318)
- #PAPER [Supervised Contrastive Learning (Khosla 2021)](https://arxiv.org/abs/2004.11362)
	- #CODE https://github.com/google-research/google-research/tree/master/supcon
	- #CODE https://keras.io/examples/vision/supervised-contrastive-learning/
	- extended the self-supervised batch contrastive approach to the fully-supervised setting, allowing us to effectively leverage label information
	- clusters of points belonging to the same class are pulled together in embedding space, while simultaneously pushing apart clusters of samples from different classes
- #PAPER [Efficient Self-supervised Learning with Contextualized Target Representations for Vision, Speech and Language (Auli 2022)](https://ai.facebook.com/research/publications/efficient-self-supervised-learning-with-contextualized-target-representations-for-vision-speech-and-language)
	- [Data2vec 2.0: Highly efficient self-supervised learning for vision, speech and text](https://ai.facebook.com/blog/ai-self-supervised-learning-data2vec/)
	- #CODE https://github.com/facebookresearch/fairseq/tree/main/examples/data2vec
