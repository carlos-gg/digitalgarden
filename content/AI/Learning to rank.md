---
title: "Learning to rank"
disableToc: false 
---

## Resources
- https://en.wikipedia.org/wiki/Learning_to_rank
- Learning to rank or machine-learned ranking (MLR) is the application of machine learning, typically supervised, semi-supervised or reinforcement learning, in the construction of ranking models for information retrieval systems. Training data consists of lists of items with some partial order specified between items in each list. This order is typically induced by giving a numerical or ordinal score or a binary judgment (e.g. "relevant" or "not relevant") for each item. The ranking model's purpose is to rank, i.e. produce a permutation of items in new, unseen lists in a way which is "similar" to rankings in the training data in some sense.

### Ordinal regression (classification)
- https://en.wikipedia.org/wiki/Ordinal_regression
- OR (also called "ordinal classification" or “ranking learning”) is a type of [Regression](AI/Supervised%20Learning/Regression.md) analysis used for predicting an ordinal variable, i.e. a variable whose value exists on an arbitrary scale where only the relative ordering between different values is significant. It can be considered an intermediate problem between regression and classification.
- http://stackoverflow.com/questions/3495157/ordinal-classification-packages-and-algorithms
- http://stats.idre.ucla.edu/r/dae/ordinal-logistic-regression/

## Code
- #CODE [Adarank](https://github.com/rueycheng/AdaRank)
- #CODE [Pyltr - LambdaMART](https://github.com/jma127/pyltr)
- #CODE [Mord - Ordinal Regression in Python](https://github.com/fabianp/mord)
	- https://pythonhosted.org/mord/
	- http://fa.bianp.net/blog/2013/logistic-ordinal-regression/

## References
### DL-based ranking
- #PAPER [TF-Ranking: Scalable TensorFlow Library for Learning-to-Rank (Kumar Pasumarthi 2019)](https://research.google/pubs/pub48160/)
	- #CODE https://github.com/tensorflow/ranking
	- [New Keras-based TF-Ranking version](https://ai.googleblog.com/2021/07/advances-in-tf-ranking.html)
