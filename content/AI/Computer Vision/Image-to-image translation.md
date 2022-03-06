# Image-to-image translation
- The task of Image-to-image translation is to learn the mapping from a given image (X) to a specific target image (Y), e.g., mapping grayscale images to RGB images.
- Learning the mapping from one visual representation to another requires an understanding of underlying features that are shared between these representations, such features are either domain-independent or domain-specific.
- https://paperswithcode.com/task/image-to-image-translation
- https://github.com/weihaox/awesome-image-translation
- Deep Domain Adaptation In Computer Vision: https://towardsdatascience.com/deep-domain-adaptation-in-computer-vision-8da398d3167f

Review papers:
- #PAPER Image-to-Image Translation: Methods and Applications (Pang 2021): https://arxiv.org/abs/2101.08629


## CNN-based
See [[Encoder-decoder networks]]
- Related to the task of supervised semantic segmentation but changing the Y and the loss (MAE, MSE or other reconstruction loss)


## GAN-based
See [[GANs#GANs for representation learning and image synthesis]]
Review papers:
- #PAPER Deep Generative Adversarial Networks for Image-to-Image Translation: A Review (Alotaibi 2020): https://www.mdpi.com/2073-8994/12/10/1705/htm#  ^I2IGANs20
	- The powerful ability of deep feature learning to automatically utilize complex and high-level feature representations has significantly advanced the performance of state-of-the-art methods across computer applications
	- The underlying structure and distinctive (complex) features are both discovered via deep learning-based methods that can be classified further into discriminative feature-learning algorithms and generative feature-learning algorithms
	- Discriminative models focus on the classification-learning process by learning the conditional probability p (x|y) to map input x to class label y. One of the most popular methods used for image feature learning utilizes convolutional neural networks (CNN) for feature extraction and image classification (LeNet, AlexNet, VGGNet, ResNet and other supervised learning algorithms)
	- Generative models focus on the data distribution to discover the underlying features from large amounts of data in an unsupervised setting. Such models are able to generate new samples by learning the estimation of the joint probability distribution p (x,y) and predicting y
	- The most dominant and efficient deep generative models of recent years have been VAE and GAN. A variational autoencoder learns the underlying probability distribution and generates a new sample that is based on Bayesian inference by maximizing the lower bound of the data’s log-likelihood. In contrast, generative adversarial networks learn data distributions through the adversarial training process based on game theory instead of maximizing the likelihood.
	- I2I methods:
		- Supervised
			- Directional translation (Pix2Pix, StarGAN)
			- Bidirectional translation (BicycleGAN, CEGAN)
		- Unsupervised
			- Cyclic consistency (CycleGAN, DiscoGAN, DualGAN, QGAN, XGAN)
			- Autoencoder-based (UNIT, BranchGAN)
			- Disentangler representation (MUNIT, DIRT, DosGAN)

### Paired (supervised) translation 
- #PAPER Image-to-Image Translation with Conditional Adversarial Networks, pix2pix (Isola 2016): https://arxiv.org/abs/1611.07004 ^pix2pix
	- Loss function learned by the network itself instead of L2, L1 norms
	- UNET generator, CNN discriminator
	- Euclidean distance is minimized by averaging all plausible outputs, which causes blurring.  Coming up with loss functions that force the CNN to do what we really want– e.g., output sharp, realistic images – is an open problem and generally requires expert knowledge 
	- Evaluating the quality of synthesized images is an open and difficult problem. Traditional metrics such as per-pixel mean-squared error do not assess joint statistics of the result, and therefore do not measure the very structure that structured losses aim to capture
	- #CODE https://github.com/phillipi/pix2pix
	- #CODE https://www.tensorflow.org/tutorials/generative/pix2pix 
	- #CODE https://github.com/He-Jian/pix2pix-keras
	- https://affinelayer.com/pixsrv/
	- https://medium.com/deep-math-machine-learning-ai/ch-14-2-pix2pix-gan-and-cycle-gan-55cd84318fb8 
	- https://machinelearningmastery.com/how-to-develop-a-conditional-generative-adversarial-network-from-scratch/
	- https://machinelearningmastery.com/how-to-develop-a-pix2pix-gan-for-image-to-image-translation/
	- Image-to-Image Translation in Tensorflow: https://affinelayer.com/pix2pix/
	- Two minutes papers: https://www.youtube.com/watch?v=u7kQ5lNfUfg
	- Paper walkthrough: https://www.youtube.com/watch?v=9SGs4Nm0VR4
	- Stochastic inference: 
		- https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix/issues/152
			- tried a few ways of adding z to the nets, e.g., adding z to a latent state, concatenating with a latent state, applying dropout, etc. The output tended not to vary much as a function of z
			- see follow up paper by Zhu et al 2017 (BicycleGAN). Shows one way of getting z to actually have a substantial effect
		- https://machinelearningmastery.com/how-to-implement-pix2pix-gan-models-from-scratch-with-keras/ 
			- unlike traditional generator models in the GAN architecture, the U-Net generator does not take a point from the latent space as input. Instead, dropout layers are used as a source of randomness both during training and when the model is used to make a prediction, e.g. generate an image at inference time
			- similarly, batch normalization is used in the same way during training and inference, meaning that statistics are calculated for each batch and not fixed at the end of the training process. This is referred to as instance normalization, specifically when the batch size is set to 1 as it is with the Pix2Pix model
			- "At inference time, we run the generator net in exactly the same manner as during the training phase. This differs from the usual protocol in that we apply dropout at test time, and we apply batch normalization using the statistics of the test batch, rather than aggregated statistics of the training batch."
			- in Keras, layers like Dropout and BatchNormalization operate differently during training and in inference model. We can set the “training” argument when calling these layers to “True” to ensure that they always operate in training-model, even when used during inference
- #PAPER Toward Multimodal Image-to-Image Translation, BicycleGAN (Zhu 2017): https://arxiv.org/abs/1711.11586 ^bicyclegan
	- #CODE https://github.com/junyanz/BicycleGAN
	- #CODE https://github.com/clvrai/BicycleGAN-Tensorflow
	- #CODE https://github.com/prakashpandey9/BicycleGAN
	- Aimed to model a distribution of possible outputs in a conditional generative modeling setting
	-  The ambiguity of the mapping is distilled in a low-dimensional latent vector, which can be randomly sampled at test time. A generator learns to map the given input, combined with this latent code, to the output. 
	- Encouraged the connection between output and the latent code to be invertible. This helps prevent a many-to-one mapping from the latent code to the output during training, also known as the problem of mode collapse, and produces more diverse results
- #PAPER Bayesian Conditional Generative Adverserial Networks (Ehsan Abbasnejad 2017): https://arxiv.org/abs/1706.05477
- #PAPER Image-to-image translation with conditional GAN (Hu 2018): https://cs230.stanford.edu/projects_spring_2018/reports/8289557.pdf
- #PAPER High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs (Wang 2018): https://tcwang0509.github.io/pix2pixHD/
	- #CODE https://github.com/NVIDIA/pix2pixHD
	- https://youtu.be/3AIpPlzM_qs
- #PAPER StarGAN: Unified Generative Adversarial Networks for Multi-Domain Image-to-Image Translation (Choi 2018): https://arxiv.org/abs/1711.09020
	- #CODE https://github.com/yunjey/stargan
- #PAPER Reversible GANs for Memory-efficient Image-to-Image Translation (van der Ouderaa 2019): https://arxiv.org/abs/1902.02729
- #PAPER StarGAN v2: Diverse Image Synthesis for Multiple Domains (Choi 2020): https://arxiv.org/abs/1912.01865
	- #CODE https://github.com/clovaai/stargan-v2


### Unpaired (unsupervised) translation
- #PAPER Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks, CycleGAN (Zhu, 2017): https://arxiv.org/abs/1703.10593 
	- #TALK https://www.youtube.com/watch?v=Fea4kZq0oFQ 
	- #CODE https://github.com/clvrai/CycleGAN-Tensorflow
	- https://junyanz.github.io/CycleGAN/
	- CycleGAN is an approach to training deep convolutional networks for Image-to-Image translation tasks. Unlike other GANs models for image translation tasks, CycleGAN learns a mapping between one image domain and another using an unsupervised approach. This is done by training Generator Networks to learn a mapping from domain X into an image that looks like it came from domain Y (and vice-versa)
	- for the generator, residual functions (residual block) are used
	- https://medium.com/deep-math-machine-learning-ai/ch-14-2-pix2pix-gan-and-cycle-gan-55cd84318fb8 
	- https://towardsdatascience.com/image-to-image-translation-using-cyclegan-model-d58cfff04755
	- https://www.tensorflow.org/tutorials/generative/cyclegan 
	- https://machinelearningmastery.com/cyclegan-tutorial-with-keras/
	- https://yanjia.li/gender-swap-and-cyclegan-in-tensorflow-2-0/
- #PAPER Learning to Discover Cross-Domain Relations with Generative Adversarial Networks (Kim 2017): https://arxiv.org/abs/1703.05192
	- #CODE https://github.com/SKTBrain/DiscoGAN
	- #CODE https://github.com/clvrai/DiscoGAN-Tensorflow
	- This paper introduced an awesome framework for finding one-to-one mapping between two domains in an unsupervised way. The high-level idea is the joint training of two GAN model G1 and G2 in parallel (one for A->B and the other one for B->A)
	- Besides the adversarial loss, there is also reconstruction loss to ensure the consistency. Specifically, we restrict that G2(G1(A)) = A and G1(G2(B)) = B
- #PAPER Unsupervised Image-to-Image Translation Networks (Liu 2018): https://arxiv.org/abs/1703.00848
	- #CODE https://github.com/mingyuliutw/UNIT/
	- https://www.youtube.com/watch?v=dqxqbvyOnMY&feature=youtu.be
	- https://medium.com/@theehiproject/unet-unit-for-fast-unsupervised-image2image-translation-using-fastai-e366408eddb4
- #PAPER MUNIT: Multimodal UNsupervised Image-to-image Translation (Huang 2018): https://arxiv.org/abs/1804.04732
	- #CODE https://github.com/NVlabs/MUNIT
- #PAPER Fixed-point GAN - Learning Fixed Points in Generative Adversarial Networks: From Image-to-Image Translation to Disease Detection and Localization (Siddiquee 2019): https://arxiv.org/abs/1908.06965 ^fixedpointGAN
	- #CODE https://github.com/mahfuzmohammad/Fixed-Point-GAN
- #PAPER Contrastive Learning for Unpaired Image-to-Image Translation (Park 2020): https://arxiv.org/abs/2007.15651
	- https://taesung.me/ContrastiveUnpairedTranslation/
	- #CODE https://github.com/taesungp/contrastive-unpaired-translation
	- #TALK https://www.youtube.com/watch?v=jSGOzjmN8q0
- #PAPER Rethinking the Truly Unsupervised Image-to-Image Translation, TUNIT (Baek 2020): https://arxiv.org/abs/2006.06500
	- #CODE https://github.com/clovaai/tunit
	- Paper explained: https://www.youtube.com/watch?v=sEG8hD64c_Q
- #PAPER Implicit Pairs for Boosting Unpaired Image-to-Image Translation (Ginger 2020): https://arxiv.org/abs/1904.06913v4


## Flow-based
- #CODE Image-to-image translation with flow-based generative model: https://github.com/yenchenlin/pix2pix-flow

- #PAPER Flow-based Image-to-Image Translation with Feature Disentanglement (Kondo 2019): https://papers.nips.cc/paper/2019/file/ffedf5be3a86e2ee281d54cdc97bc1cf-Paper.pdf
- #PAPER AlignFlow: Cycle Consistent Learning from Multiple Domains via Normalizing Flows (Grover, 2019): https://arxiv.org/abs/1905.12892
	-  A generative modeling framework that models each domain via a normalizing flow
	-  The use of normalizing flows allows for
		- flexibility in specifying learning objectives via adversarial training, maximum likelihood estimation, or a hybrid of the two methods
		- learning and exact inference of a shared representation in the latent space of the generative model. 
- #PAPER Flow-based Deformation Guidance for Unpaired Multi-Contrast MRI Image-to-Image Translation (Duc Bui 2020): https://arxiv.org/abs/2012.01777v1
	- Normalizing flows for unpaired image-to-image translation
	- Utilized the temporal information between consecutive slices to provide more constraints to the optimization for transforming one domain to another in un-paired volumetric medical image