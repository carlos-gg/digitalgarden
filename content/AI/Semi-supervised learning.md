---
title: "Semi-supervised learning"
---

>  Semi-supervised learning is an approach to machine learning that combines a small amount of labeled data with a large amount of unlabeled data during training. Semi-supervised learning falls between unsupervised learning (with no labeled training data) and supervised learning (with only labeled training data)

## Resources
- https://en.wikipedia.org/wiki/Semi-supervised_learning
- In contrast (to active learning), semi-supervised learning attempts to automatically exploit unlabeled data in addition to labeled data to improve learning performance, where no human intervention is assumed. 
- https://deepai.org/machine-learning-glossary-and-terms/semi-supervised-learning
- https://scikit-learn.org/stable/modules/label_propagation.html

## Code
- #CODE [TorchSSL](https://github.com/TorchSSL/TorchSSL)
	- A PyTorch-based Toolbox for Semi-Supervised Learning

## References
- #PAPER [Semi-Supervised Learning Literature Survey (2008)](http://pages.cs.wisc.edu/~jerryzhu/pub/ssl_survey.pdf)
- #PAPER [Learning Loss Functions for Semi-supervised Learning via Discriminative Adversarial Networks (Nogueira Dos Santos 2017)](https://arxiv.org/abs/1707.02198)
- #PAPER [Semi-Supervised Learning with Normalizing Flows (Izmailov, 2019)](https://arxiv.org/abs/1912.13025)
	- #CODE https://github.com/izmailovpavel/flowgmm
- #PAPER [Self-training with Noisy Student improves ImageNet classification (Xie 2020)](https://arxiv.org/abs/1911.04252)
	- [Paper explained](https://www.youtube.com/watch?v=q7PjrmGNx5A)
	- Noisy Student Training, a semi-supervised learning approach that works well even when labeled data is abundant. Noisy Student Training extends the idea of self-training and distillation with the use of equal-or-larger student models and noise added to the student during learning. On ImageNet, we first train an EfficientNet model on labeled images and use it as a teacher to generate pseudo labels for 300M unlabeled images. We then train a larger EfficientNet as a student model on the combination of labeled and pseudo labeled images. We iterate this process by putting back the student as the teacher. During the learning of the student, we inject noise such as dropout, stochastic depth, and data augmentation via RandAugment to the student so that the student generalizes better than the teacher.
	- #CODE https://github.com/google-research/noisystudent
- #PAPER [Big Transfer (BiT):General Visual Representation Learning (Kolesnikov 2020)](https://arxiv.org/abs/1912.11370)
	- [Paper explained](https://www.youtube.com/watch?v=k1GOF2jmX7c)
- #PAPER [Towards a Deeper Understanding of Adversarial Losses (Dong 2020)](https://arxiv.org/abs/1901.08753)
- #PAPER [DoubleMatch: Improving Semi-Supervised Learning with Self-Supervision (Wallin 2022)](https://arxiv.org/pdf/2205.05575v1)            
	- #CODE https://paperswithcode.com/paper/doublematch-improving-semi-supervised
	- DoubleMatch combines the pseudo-labeling technique with a self-supervised loss, enabling the model to utilize all unlabeled data in the training process. We show that this method achieves state-of-the-art accuracies on multiple benchmark datasets while also reducing training times compared to existing SSL methods