---
title: "Inpainting"
disableToc: false 
---

- https://en.wikipedia.org/wiki/Inpainting
- Inpainting is a conservation process where damaged, deteriorating, or missing parts of an artwork are filled in to present a complete image
- https://www.nvidia.com/research/inpainting/
- An Introduction to Image Inpainting using Deep Learning: https://wandb.ai/ayush-thakur/image-impainting/reports/An-Introduction-to-Image-Inpainting-using-Deep-Learning--Vmlldzo3NDU0Nw


## References
Review papers:
- #PAPER Image inpainting: A review (Elharrouss 2019): https://arxiv.org/abs/1909.06399

### CNN-based
- #PAPER Feature Learning by Inpainting (Pathak 2016): https://arxiv.org/abs/1604.07379v1
	- #CODE https://github.com/pathak22/context-encoder
- #PAPER Image Inpainting for Irregular Holes Using Partial Convolutions (Liu 2018): https://arxiv.org/abs/1804.07723
	- https://nv-adlr.github.io/publication/partialconv-inpainting
	- #CODE https://github.com/NVIDIA/partialconv
	- #CODE https://github.com/naoto0804/pytorch-inpainting-with-partial-conv
	- #CODE https://github.com/MathiasGruber/PConv-Keras
	- #CODE Various Keras Layers that can be used with TensorFlow 2.x: https://github.com/mvoelk/keras_layers
- #PAPER Partial Convolution based Padding (Liu 2018): https://arxiv.org/pdf/1811.11718
- #PAPER Probabilistic Semantic Inpainting with Pixel Constrained CNNs (Dupont 2019): https://arxiv.org/abs/1810.03728
	- #CODE https://github.com/Schlumberger/pixel-constrained-cnn-tf
- #PAPER A Flexible Deep [[CNNs]] Framework for Image Restoration (2020): https://ieeexplore.ieee.org/document/8820082
	- https://www.researchgate.net/profile/Zhi_Jin6/publication/335500109_A_Flexible_Deep_CNN_Framework_for_Image_Restoration/links/5da7c1a9299bf1c1e4c837c3/A-Flexible-Deep-CNN-Framework-for-Image-Restoration.pdf
- #PAPER Deep learning-Based 3D inpainting of brain MR images (Kwan Kang 2021): https://www.nature.com/articles/s41598-020-80930-w 


### GAN-based
- GANs and Missing Data Imputation: https://towardsdatascience.com/gans-and-missing-data-imputation-815a0cbc4ece

- #PAPER VIGAN: Missing View Imputation with Generative Adversarial Networks (Shang 2017): https://arxiv.org/abs/1708.06724
	- #CODE https://github.com/chaoshangcs/VIGAN
- #PAPER Patch-Based Image Inpainting with [[GANs]] (Demir 2018): https://arxiv.org/abs/1803.07422
- #PAPER GAIN: Missing Data Imputation using [[GANs]] (Yoon 2018): https://arxiv.org/abs/1806.02920
	- #CODE https://github.com/jsyoon0823/GAIN
- #PAPER MisGAN: Learning from Incomplete Data with Generative Adversarial Networks (Li 2019): https://arxiv.org/abs/1902.09599
- #PAPER CollaGAN : Collaborative GAN for Missing Image Data Imputation (Li 2019): https://arxiv.org/abs/1901.09764
- #PAPER DeepGIN: Deep Generative Inpainting Network for Extreme Image Inpainting (Li 2020): https://arxiv.org/abs/2008.07173
	- #CODE https://github.com/rlct1/DeepGIN
	- https://medium.com/analytics-vidhya/review-of-deepgin-deep-generative-inpainting-network-for-extreme-image-inpainting-de5b191562b0
- #PAPER The image inpainting algorithm used on multi-scale generative adversarial networks and neighbourhood (Mo 2020): https://www.tandfonline.com/doi/full/10.1080/00051144.2020.1821535