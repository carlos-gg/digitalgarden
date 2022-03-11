---
title: "Weakly supervised learning"
disableToc: false 
---

See:
[Transfer learning](AI/Transfer%20learning.md)
[Active learning](AI/Active%20learning.md)
[Semi-supervised learning](AI/Semi-supervised%20learning.md)

## Resources
- Weak supervision is a branch of machine learning where noisy, limited, or imprecise sources are used to provide supervision signal for labeling large amounts of training data in a supervised learning setting. This approach alleviates the burden of obtaining hand-labeled data sets, which can be costly or impractical. Instead, inexpensive weak labels are employed with the understanding that they are imperfect, but can nonetheless be used to create a strong predictive model.
- Other areas of machine learning exist that are likewise motivated by the demand for increased quantity and quality of labeled training data but employ different high-level techniques to approach this demand. These other approaches include [active learning](AI/Active%20learning.md), [semi-supervised learning](AI/Semi-supervised%20learning.md), and [transfer learning](AI/Transfer%20learning.md).
- Related to [One, few-shot learning](AI/One,%20few-shot%20learning.md). The most relevant problem to few-shot learning is weakly supervised learning with incomplete supervision where only a small amount of samples have supervised. By definition, weakly supervised learning with incomplete supervision includes only classification and regression, while few-shot learning also includes reinforcement learning problems. Moreover, weakly supervised learning with incomplete supervision mainly uses unlabeled data as additional information in E, while few-shot learning leverages various kinds of prior knowledge such as pretrained models, supervised data from other domains or modalities and does not restrict to using unlabeled data. Therefore, few-shot learning becomes weakly supervised learning problem only when prior knowledge is unlabeled data and the task is classification or regression.information.
- [Weakly Supervised Learning: Introduction and Best Practices](https://datasciencemilan.medium.com/weakly-supervised-learning-introduction-and-best-practices-c65f490d4a0a)


## References
- #PAPER [A brief introduction to weakly supervised learning (2018)](https://academic.oup.com/nsr/article/5/1/44/4093912 )
- #PAPER [A Graph-Based Method for Active Outlier Detection With Limited Expert Feedback (2019)](https://ieeexplore.ieee.org/document/8871105)

### Incomplete supervision
- In this case, only a (usually small) subset of training data is given with labels while the other data remain unlabeled (e.g., in image categorization the ground-truth labels are given by human annotators, and only a small subset of images can be annotated due to the human cost)
- #PAPER [Learning from Incomplete and Inaccurate Supervision (Zhang 2021)](https://ieeexplore.ieee.org/document/9361098)

### Inexact supervision
- In this case, only coarse-grained labels are given. Consider the image categorization task again. It is desirable to have every object in the images annotated; however, usually we only have image-level labels rather than object-level labels. 
- #PAPER [Labeled Data Generation with Inexact Supervision (Dai 2021)](https://arxiv.org/abs/2106.04716)

### Inaccurate supervision
- The given labels are not always ground-truth (e.g., the image annotator is careless, or some images are difficult to categorize)
 - #PAPER [Auxiliary Image Regularization for Deep CNNs with Noisy Labels (2016)](https://arxiv.org/abs/1511.07069v2)
 - #PAPER [Anomaly detection with inexact labels (2019)](https://arxiv.org/abs/1909.04807)
