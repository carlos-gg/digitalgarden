---
title: "Transfer learning"
disableToc: false 
---

## Resources
- https://en.wikipedia.org/wiki/Transfer_learning
- Transfer learning (TL) is a research problem in machine learning (ML) that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem
- https://github.com/artix41/awesome-transfer-learning
- [Domain adaptation](https://en.wikipedia.org/wiki/Domain_adaptation)
	- Domain adaptation is a field associated with machine learning and transfer learning. This scenario arises when we aim at learning from a source data distribution a well performing model on a different (but related) target data distribution


## Code
- #CODE [pytorch-adapt](https://github.com/KevinMusgrave/pytorch-adapt)
	- Domain adaptation made easy. Fully featured, modular, and customizable
	- https://kevinmusgrave.github.io/pytorch-adapt/
- #CODE [TLlib](https://github.com/thuml/Transfer-Learning-Library)
	- open-source and well-documented library for Transfer Learning. It is based on pure PyTorch with high performance and friendly API
- #code [Salad](https://github.com/domainadaptation/salad)
	- https://domainadaptation.org/
- #code [Robustness](https://github.com/bethgelab/robustness)
	- https://domainadaptation.org/robusta/


## References
- #PAPER [A Brief Review of Domain Adaptation (Farahani 2020)](https://arxiv.org/abs/2010.03978)
- #PAPER [On the Opportunities and Risks of Foundation Models (Bommasani 2021)](https://arxiv.org/abs/2108.07258)
	- A foundation model is any model that is trained on broad data at scale and can be adapted (e.g., fine-tuned) to a wide range of downstream tasks; current examples include BERT, GPT-3, and CLIP
	- Foundation models are based on deep neural networks and self-supervised learning
	- On a technical level, foundation models are enabled by transfer learning and scale
	- The idea of transfer learning is to take the “knowledge” learned from one task (e.g., object recognition in images) and apply it to another task (e.g., activity recognition in videos).
	- Within deep learning, pretraining is the dominant approach to transfer learning: a model is trained on a surrogate task (often just as a means to an end) and then adapted to the downstream task of interest via fine-tuning
	- Transfer learning is what makes foundation models possible, but scale is what makes them powerful. Scale required three ingredients: improvements in computer hardware, the development of the Transformer model architecture that leverages the parallelism of the hardware to train much more expressive models than before and the availability of much more training data