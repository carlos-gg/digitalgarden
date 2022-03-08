---
title: "Active learning"
disableToc: false 
---

## Resources
* https://en.wikipedia.org/wiki/Active_learning_(machine_learning)
* Active learning refers to algorithms that take an active role in the selection of which ex-amples are labeled. Active learning assumes that there is an ‘oracle’, such as a human expert, that can be queried to get ground-truth labels for selected unlabeled instances. 
* There are situations in which unlabeled data is abundant but manually labeling is expensive. In such a scenario, learning algorithms can actively query the user/teacher for labels. This type of iterative supervised learning is called active learning. Since the learner chooses the examples, the number of examples to learn a concept can often be much lower than the number required in normal supervised learning. With this approach, there is a risk that the algorithm be overwhelmed by uninformative examples.
- Overview of Active Learning for Deep Learning: https://jacobgil.github.io/deeplearning/activelearning
- #PAPER An open source machine learning framework for efficient and transparent systematic reviews (van de Schoot 2021): https://www.nature.com/articles/s42256-020-00287-7
	- #CODE https://github.com/asreview/asreview

## References
- #PAPER Active learning literature survey (Settles 2010): http://burrsettles.com/pub/settles.activelearning.pdf
- #PAPER Active Learning for Convolutional Neural Networks: A Core-Set Approach (2018): https://openreview.net/forum?id=H1aIuk-RW
- #PAPER Rethinking deep active learning: Using unlabeled data at model training (Simeoni 2019): https://arxiv.org/abs/1911.08177
- #PAPER Deep Batch Active Learning by Diverse, Uncertain Gradient Lower Bounds (2020): https://openreview.net/forum?id=ryghZJBKPS 


### Active learning for anomaly discovery
- #PAPER Incorporating Expert Feedback into Active Anomaly Discovery (Das 2016): https://ieeexplore.ieee.org/document/7837915
	- http://web.engr.oregonstate.edu/~tgd/publications/das-wong-dietterich-fern-emmott-incorporating-expert-feedback-into-active-anomaly-discovery-icdm2016.pdf
- #PAPER Deep Active Learning for Anomaly Detection (Pimentel 2018): https://arxiv.org/abs/1805.09411