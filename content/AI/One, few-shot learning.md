---
title: "One, few-shot learning"
disableToc: false 
---

## Resources
- https://en.wikipedia.org/wiki/One-shot_learning
- One-shot learning is an object categorization problem, found mostly in computer vision. Whereas most machine learning based object categorization algorithms require training on hundreds or thousands of samples/images and very large datasets, one-shot learning aims to learn information about object categories from one, or only a few, training samples/images.
- https://medium.com/sap-machine-learning-research/deep-few-shot-learning-a1caa289f18
- https://sorenbouma.github.io/blog/oneshot/
- https://github.com/Goldesel23/Siamese-Networks-for-One-Shot-Learning
- [Zero-Shot Visual Imitation](https://pathak22.github.io/zeroshot-imitation/)
- #TALK [Neural Networks - One Shot Learning](https://www.youtube.com/watch?v=r8LLorRACPM)


## Code
- #CODE [LibFewShot](https://github.com/rl-vig/libfewshot)
	- #PAPER [LibFewShot: A Comprehensive Library for Few-shot Learning (Li 2021)](https://arxiv.org/abs/2109.04898)
	- LibFewShot: A Comprehensive Library for Few-shot Learning (pytorch)

## References
- #PAPER [Siamese Neural Networks for One-shot Image Recognition (Koch 2015)](http://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf)
	- Few-Shot learning has seen great progress over the last years. A classic approach is based on metric learning using Siamese neural networks.
	- #CODE https://sorenbouma.github.io/blog/oneshot/
- #PAPER [One-Shot Imitation Learning (Duan 2017)](https://arxiv.org/abs/1703.07326)
- #PAPER [One-shot texture segmentation (Ustyuzhaninov 2018)](https://arxiv.org/abs/1807.02654)
	- We solve the task of one-shot texture segmentation in three steps. First, we compute embeddings of an input image and a reference patch; second, we search for the reference texture in the embedding space to produce a rough segmentation mask; and, finally, we employ a decoding network to produce the output segmentation.
- #PAPER [One-shot instance segmentation (Michaelis 2018)](https://arxiv.org/abs/1811.11507 )
	- We tackle one-shot visual search by example for arbitrary object categories: Given an example image of a novel reference object, find and segment all object instances of the same category within a scene. To address this problem, we propose Siamese Mask R-CNN. 
	- It extends Mask R-CNN by a Siamese backbone encoding both reference image and scene, allowing it to target detection and segmentation towards the reference category.
- #PAPER [FIGR: Few-shot Image Generation with Reptile (Clouatre 2019)](https://arxiv.org/abs/1901.02199)
- #PAPER [Generalizing from a Few Examples: A Survey on Few-Shot Learning (Wang 2020)](https://arxiv.org/abs/1904.05046)
- #PAPER ['Less Than One'-Shot Learning: Learning N Classes From M < N Samples (Sucholutsky 2020)](https://arxiv.org/abs/2009.08449)
	- https://www.technologyreview.com/2020/10/16/1010566/ai-machine-learning-with-tiny-data/
	- AI model able to accurately recognize more objects than the number of examples it was trained on
	- The trick, was to create images that blend multiple digits together and then feed them into an AI model with hybrid, or “soft,” labels


### Few/one-shot learning GANs 
- #PAPER [MetaGAN: An Adversarial Approach to Few-Shot Learning (Zhang 2018)](https://papers.nips.cc/paper/7504-metagan-an-adversarial-approach-to-few-shot-learning)
- #PAPER [SinGAN: Learning a Generative Model from a Single Natural Image, SinGAN (Rott Shaham, ICCV 2019 Best Paper)](https://arxiv.org/abs/1905.01164 )
	- [ Paper explained](https://www.youtube.com/watch?v=-f8sz8AExdc )
	- [ Paper explained](https://www.youtube.com/watch?v=Xc9Rkbg6IZA)
- #PAPER [DAWSON: A Domain Adaptive Few Shot Generation Framework (Liang 2020)](https://arxiv.org/abs/2001.00576)
- #PAPER [LARGE: Latent-Based Regression through GAN Semantics (Nitzan 2021)](https://arxiv.org/abs/2107.11186)
	- #CODE https://github.com/YotamNitzan/LARGE
