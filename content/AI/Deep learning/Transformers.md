---
title: "Transformers"
---

## Resources
- https://github.com/IDEACVR/awesome-detection-transformer
- https://github.com/Yangzhangcst/Transformer-in-Computer-Vision
- https://www.analyticsvidhya.com/blog/2019/11/comprehensive-guide-attention-mechanism-deep-learning/ (from RNNs with attention to Transformers)
- https://analyticsindiamag.com/a-complete-learning-path-to-transformers/
- https://analyticsindiamag.com/transformers-for-vision-7-works-that-indicate-fusion-is-the-future-of-ai/
- [Investigating Vision Transformer representations](https://keras.io/examples/vision/probing_vits/)
	- #CODE https://github.com/sayakpaul/probing-vits
- [Self-Supervised Learning in Vision Transformers](https://towardsdatascience.com/self-supervised-learning-in-vision-transformers-30ff9be928c)


## Courses
- #COURSE [CS25: Transformers United (Stanford)](https://web.stanford.edu/class/cs25/)
	- [Videos](https://www.youtube.com/playlist?list=PLoROMvodv4rNiJRchCzutFw5ItR_Z27CM)


## Code
- #CODE [Transformers](https://github.com/huggingface/transformers)
	- thousands of pretrained models to perform tasks on different modalities such as text, vision, and audio
	- JAX, PyTorch and TensorFlow
- #CODE [Xformers](https://github.com/facebookresearch/xformers)
- #CODE [Transformers: from NLP to CV](https://github.com/IbrahimSobh/Transformers)
- #CODE [Big vision](https://github.com/google-research/big_vision)
	- This codebase is designed for training large-scale vision models on Cloud TPU VMs. It is based on Jax/Flax libraries, and uses tf.data and TensorFlow Datasets for scalable input pipelines in the Cloud


## For NLP
- #PAPER [Attention is all you need (Vaswani 2017)](https://arxiv.org/abs/1706.03762)
	- https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html
	- [Paper explained](https://www.youtube.com/watch?v=iDulhoQ2pro)
	- The Transformer is a novel neural network architecture based on a self-attention mechanism that is well suited for language understanding. 
	- It outperforms both recurrent and convolutional models on academic English to German and English to French translation benchmarks. On top of higher translation quality, the Transformer requires less computation to train and is a much better fit for modern machine learning hardware, speeding up training by up to an order of magnitude.
	- Self-attention is the method the Transformer uses to bake the “understanding” of other relevant words into the one we’re currently processing. If you’re familiar with RNNs, think of how maintaining a hidden state allows an RNN to incorporate its representation of previous words/vectors it has processed with the current one it’s processing. 
	- The dominant sequence transduction models are based on complex recurrent or convolutional neural networks in an encoder-decoder configuration. The best performing models also connect the encoder and decoder through an attention mechanism. We propose a new simple network architecture, the Transformer, based solely on attention mechanisms, dispensing with recurrence and convolutions entirely.
	- http://jalammar.github.io/illustrated-transformer/
	- [Attention is all you need, attentional neural network models (Łukasz Kaiser)](https://www.youtube.com/watch?v=rBCqOTEfxvg)
	- [LSTM is dead, long live Transformers](https://sea-adl.org/2019/12/03/lstm-is-dead-long-live-transformers/)
- #PAPER [Tensor2tensor (Vaswani 2018)](https://arxiv.org/abs/1803.07416)
	- Tensor2Tensor, or T2T for short, is a library of deep learning models and datasets designed to make deep learning more accessible and accelerate ML research. T2T is actively used and maintained by researchers and engineers within the Google Brain team and a community of users. We're eager to collaborate with you too, so feel free to open an issue on GitHub or send along a pull request (see our contribution doc). You can chat with us on Gitter and join the T2T Google Group.
	- It includes the reference implementation of the state-of-the-art Transformer model.
- #PAPER [Improving Language Understanding by Generative Pre-Training, GPT (Radford 2018)](https://cdn.openai.com/research-covers/language-unsupervised/language_understanding_paper.pdf)
	- https://openai.com/blog/language-unsupervised/
- #PAPER [Language Models are Unsupervised Multitask Learners, GPT-2 (Radford 2018)](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)
	- #CODE https://github.com/openai/gpt-2
	- https://openai.com/blog/better-language-models/
	- Paper explained
		- https://www.youtube.com/watch?v=u1_qMdb0kYU
		- https://www.youtube.com/watch?v=UULqu7LQoHs
		- https://www.youtube.com/watch?v=8ypnLjwpzK8
- #PAPER [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding (Devlin 2019)](https://arxiv.org/abs/1810.04805)
	- #CODE [TensorFlow code and pre-trained models for BERT](https://github.com/google-research/bert)
	- [Paper explained](https://www.youtube.com/watch?v=-9evrZnBorM)
	- [BERT as a service](https://github.com/hanxiao/bert-as-service)
- #PAPER [Language Models are Few-Shot Learners, GPT-3 (Brown 2020)](https://arxiv.org/abs/2005.14165)
	- Paper explained: 
		- https://www.youtube.com/watch?v=SY5PvZrJhLE
		-  https://www.youtube.com/watch?v=_x9AwxfjxvE
- #PAPER [It's Not Just Size That Matters: Small Language Models Are Also Few-Shot Learners (Schick 2020)](https://arxiv.org/abs/2009.07118)
	- #CODE https://github.com/timoschick/pet
	- https://www.infoq.com/news/2020/10/training-exceeds-gpt3/
- #PAPER [Rethinking Attention with Performers (Choromanski 2020)](https://arxiv.org/abs/2009.14794)
	- https://syncedreview.com/2020/10/02/google-cambridge-deepmind-alan-turing-institutes-performer-transformer-slashes-compute-costs/
	- https://ai.googleblog.com/2020/10/rethinking-attention-with-performers.html
	- #CODE https://github.com/google-research/google-research/tree/master/performer/fast_self_attention
	- [Paper explained](https://www.youtube.com/watch?v=xJrKIPwVwGM)
- #PAPER [SqueezeBERT: What can computer vision teach NLP about efficient neural networks? (Iandola 2020)](https://arxiv.org/abs/2006.11316)
	- #TALK [From SqueezeNet to SqueezeBERT: Developing Efficient Deep Neural Networks](https://www.youtube.com/watch?v=kPMaEYSywdI)
	- https://www.microsoft.com/en-us/research/video/from-squeezenet-to-squeezebert-developing-efficient-deep-neural-networks/
- #PAPER [FNet: Mixing Tokens with Fourier Transforms (Lee-Thorp 2021)](https://arxiv.org/abs/2105.03824)
	- https://syncedreview.com/2021/05/14/deepmind-podracer-tpu-based-rl-frameworks-deliver-exceptional-performance-at-low-cost-19/
	- #CODE https://paperswithcode.com/paper/fnet-mixing-tokens-with-fourier-transforms?from=n10
	- Transformer architectures can be massively sped up, with limited accuracy costs, by replacing self-attention sublayers with linear transformations that "mix" input tokens
- #PAPER [Optimizing Deeper Transformers on Small Datasets (Xu 2021)](https://arxiv.org/abs/2012.15355)
- #PAPER [Infinity-former: Infinite Memory Transformer (Martins 2022)](https://arxiv.org/abs/2109.00301)
	- [Paper explained](https://www.youtube.com/watch?v=0JlB9gufTw8)
- #PAPER [Scaling Language Models: Methods, Analysis & Insights from Training Gopher (Rae 2022)](https://arxiv.org/abs/2112.11446)
	- [Paper explained](https://www.youtube.com/watch?v=aPiHhJjN3hI)
- #PAPER [LaMDA: Language Models for Dialog Applications (Thoppilan 2022)](https://arxiv.org/pdf/2201.08239)

## For Computer Vision
- #PAPER [Spatial Transformer Networks (Jaderberg 2016)](https://arxiv.org/abs/1506.02025)
	-  the use of spatial transformers results in models which learn invariance to translation, scale, rotation and more generic warping, result-ing in state-of-the-art performance on several benchmarks, and for a number of classes of transformations
	-  https://www.youtube.com/watch?v=6NnearestOQC_fl1hQ
	-  #CODE https://github.com/oarriaga/paz/tree/master/examples/spatial_transfomer_networks
- #PAPER [Image Transformer (Parmar 2018)](https://arxiv.org/abs/1802.05751)
- #PAPER [Generative Pretraining from Pixels (Chen 2020)](https://cdn.openai.com/papers/Generative_Pretraining_from_Pixels_V2.pdf) ^imagegpt
	- https://openai.com/blog/image-gpt/ 
	- #CODE https://github.com/openai/image-gpt
	- [Paper explained](https://www.youtube.com/watch?v=YBlNQK0Ao6g)
	- https://www.youtube.com/watch?v=7rFLnQdl22c
- #PAPER [DETR - End-to-End Object Detection with Transformers (Carion 2020)](https://arxiv.org/abs/2005.12872 )
	- #CODE https://paperswithcode.com/paper/end-to-end-object-detection-with-transformers
- #PAPER [Taming Transformers for High-Resolution Image Synthesis (Esser 2020)](https://arxiv.org/abs/2012.09841v1) ^tamingtransformers
	- https://compvis.github.io/taming-transformers/
	- https://github.com/CompVis/taming-transformers
	- https://www.marktechpost.com/2020/12/28/a-new-method-to-code-inductive-image-biases-into-models-using-cnn-and-transformers/
- #PAPER [ViT - An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale (2020)](https://openreview.net/forum?id=YicbFdNTTy)
	- While the Transformer architecture has become the de-facto standard for natural language processing tasks, its applications to computer vision remain limited. In vision, attention is either applied in conjunction with convolutional networks, or used to replace certain components of convolutional networks while keeping their overall structure in place. We show that this reliance on CNNs is not necessary and a pure transformer can perform very well on image classification tasks when applied directly to sequences of image patches
	- [Paper explained](https://www.youtube.com/watch?v=TrdevFK_am4)
	- #CODE https://github.com/google-research/vision_transformer
	- #CODE https://keras.io/examples/vision/image_classification_with_vision_transformer/
	- #CODE https://github.com/ashishpatel26/Vision-Transformer-Keras-Tensorflow-Pytorch-Examples
- #PAPER [Training data-efficient image transformers & distillation through attention (Touvron 2021)](https://arxiv.org/abs/2012.12877)
	- #CODE https://github.com/facebookresearch/deit
	- Propose a competitive convolution-free transformer by training on Imagenet only
	- Introduced a teacher-student strategy specific to transformers. It relies on a distillation token ensuring that the student learns from the teacher through attention
	- https://ai.facebook.com/blog/data-efficient-image-transformers-a-promising-new-technique-for-image-classification/
- #PAPER [PVT - Pyramid Vision Transformer: A Versatile Backbone for Dense Prediction without Convolutions (Wang 2021)](https://arxiv.org/abs/2102.12122) ^pvt
	- #CODE https://paperswithcode.com/paper/pyramid-vision-transformer-a-versatile
	- #CODE https://github.com/wangermeng2021/PVT-tensorflow2
	- PVT inherits the advantages from both CNN and Transformer, making it a unified backbone in various vision tasks without convolutions by simply replacing CNN backbones
- #PAPER [Vision Transformers for Dense Prediction (Ranftl 2021)](https://arxiv.org/abs/2103.13413v1)
	- #CODE https://paperswithcode.com/paper/vision-transformers-for-dense-prediction
	- Model with an encoder-decoder design, leveraging the vision transformer (ViT) as the building block of the encoder
	- The representations produced by the transformer are reassembled into image-like feature representations at various resolutions and are progressively combined into the final dense prediction using a convolutional decoder 
	- The transformer downsamples operations and keeps a representation with a constant dimensionality throughout the processing stages while keeping a global receptive field at every stage
	- These properties allows DPT to provide fine-grained and globally coherent predictions as compared to fully-convolutional networks
- #PAPER [Understanding Robustness of Transformers for Image Classification (Bhojanapalli 2021)](https://arxiv.org/abs/2103.14586v1)
- #PAPER [Medical Transformer: Gated Axial-Attention for Medical Image Segmentation (Valanarasu 2021)](https://arxiv.org/abs/2102.10662)
	- #CODE https://github.com/jeya-maria-jose/Medical-Transformer
	- https://analyticsindiamag.com/guide-to-medical-transformer-attention-for-medical-image-segmentation/
	- Trains with less data thanks to the Gated Axial-Attention model which extends the existing architectures by introducing an additional control mechanism in the self-attention module
	- To train the model effectively on medical images, we propose a Local-Global training strategy (LoGo) which further improves the performance. Specifically, we operate on the whole image and patches to learn global and local features, respectively
- #PAPER [TransGAN: Two Transformers Can Make One Strong GAN (Jiang 2021)](https://arxiv.org/abs/2102.07074v2)
	- #CODE https://paperswithcode.com/paper/transgan-two-transformers-can-make-one-strong
	-  first pilot study in building a GAN completely free of convolutions, using only pure transformer-based architectures
- #PAPER [Gansformer - Generative Adversarial Transformers (Hudson 2021)](https://arxiv.org/abs/2103.01209v2)
	- #CODE https://paperswithcode.com/paper/generative-adversarial-transformers
- #PAPER [Swin Transformer: Hierarchical Vision Transformer using Shifted Windows (Liu 2021)](https://arxiv.org/abs/2103.14030)
	- #CODE https://github.com/microsoft/Swin-Transformer
	- #CODE https://github.com/rishigami/Swin-Transformer-TF
	- #CODE https://github.com/yingkaisha/keras-vision-transformer
	- Swin Transformer serves as a general-purpose backbone for computer vision. Works for tasks such as image classification, object detection and semantic segmentation
	- involves a hierarchical Transformer whose representation is computed through a shifted windowing mechanism which limits the self-attention computation to non-overlapping local windows while still allowing for cross-window connection
	- the benefits of this hierarchical architecture are greater efficiency and flexibility to model at various scales. In addition, this model has linear computational complexity with respect to image size
- #PAPER [How to train your ViT? Data, Augmentation, and Regularization in Vision Transformers (Steiner 2021)](https://arxiv.org/abs/2106.10270v1)
	- Results show that models using a combination of AugReg (model regularization) and increased compute can attain similar performance as models trained on an order of magnitude more training data
	- ViT models of various sizes, trained on ImageNet-21k, match or outperform counterparts trained on a larger dataset (JFT-300M)
	- #CODE https://paperswithcode.com/paper/how-to-train-your-vit-data-augmentation-and
- #PAPER [Self-Attention Between Datapoints: Going Beyond Individual Input-Output Pairs in Deep Learning (Kossen 2021)](https://arxiv.org/abs/2106.02584v1)
	- #CODE https://paperswithcode.com/paper/self-attention-between-datapoints-going?from=n11
	- Authors challenge a common assumption underlying most supervised deep learning: that a model makes a prediction depending only on its parameters and the features of a single input
	- Introduced a general-purpose deep learning architecture that takes as input the entire dataset instead of processing one datapoint at a time
	- The approach uses self-attention to reason about relationships between datapoints explicitly, which can be seen as realizing non-parametric models using parametric attention mechanisms
- #PAPER [Segmenter: Transformer for Semantic Segmentation (Strudel 2021)](https://arxiv.org/abs/2105.05633)
- #PAPER [Focal Self-attention for Local-Global Interactions in Vision Transformers (Yang 2021)](https://arxiv.org/abs/2107.00641)
	- https://www.marktechpost.com/2021/08/24/microsoft-ai-open-source-the-code-for-its-focal-transformer/
- #PAPER [Do Vision Transformers See Like Convolutional Neural Networks (Raghu 2021)](https://arxiv.org/abs/2108.08810)
	- [Paper explained](https://www.youtube.com/watch?v=rk9bhIRInC0)
- #PAPER [DECIMER 1.0: deep learning for chemical image recognition using transformers (Rajan 2021)](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00538-8)
- #PAPER [Multiscale Vision Transformers (Fan 2021)](https://arxiv.org/abs/2104.11227)
	- #CODE  https://github.com/facebookresearch/SlowFast
	- https://ai.facebook.com/blog/multiscale-vision-transformers-an-architecture-for-modeling-visual-data/
- #PAPER [Swin Transformer V2: Scaling Up Capacity and Resolution (Liu 2021)](https://arxiv.org/abs/2111.09883v1)
	- #CODE https://paperswithcode.com/paper/swin-transformer-v2-scaling-up-capacity-and
- #PAPER [Transformers in Medical Imaging: A Survey (Shamshad 2022)](https://arxiv.org/abs/2201.09873v1)
	- #CODE https://paperswithcode.com/paper/transformers-in-medical-imaging-a-survey?from=n24
	- https://github.com/fahadshamshad/awesome-transformers-in-medical-imaging
- #PAPER [How Do Vision Transformers Work? (Park 2022)](https://arxiv.org/abs/2202.06709v2)
	- #CODE https://paperswithcode.com/paper/how-do-vision-transformers-work-1?from=n26
- #PAPER [EfficientFormer: Vision Transformers at MobileNet Speed (Li 2022)](https://arxiv.org/pdf/2206.01191v3)
	- #CODE https://github.com/snap-research/efficientformer
- #PAPER [Vision Transformers for Dense Prediction (Ranftl 2022)](https://arxiv.org/pdf/2103.13413) ^dpt
	- #CODE https://github.com/isl-org/DPT
	- DPT is a dense prediction architecture that is based on an encoder-decoder design that leverages a transformer as the basic computational building block of the encoder
	- used the recently proposed VIT as a backbone architecture reassembling the bag-of-words representation that is provided by ViT into image-like feature representations at various resolutions and progressively combine the feature representations into the final dense prediction using a convolutional decoder
	- it has a global receptive field at every stage
- #PAPER [HRFormer: High-Resolution Vision Transformer for Dense Predict (Yuan 2021)](https://proceedings.neurips.cc/paper/2021/hash/3bbfdde8842a5c44a0323518eec97cbe-Abstract.html)
	- #CODE https://github.com/HRNet/HRFormer
- #PAPER [ITTR: Unpaired Image-to-Image Translation with Transformers (Zheng 2022)](https://arxiv.org/pdf/2203.16015)

### Self-supervised vision transformers
- #PAPER [SiT: Self-supervised vIsion Transformer (Atito 2021)](https://arxiv.org/abs/2104.03602)
- #PAPER [DINO - Emerging Properties in Self-Supervised Vision Transformers (Caron 2021)](https://arxiv.org/abs/2104.14294)
	- https://towardsdatascience.com/on-dino-self-distillation-with-no-labels-c29e9365e382
- #PAPER [ConvMAE: Masked Convolution Meets Masked Autoencoders (Gao 2022)](https://arxiv.org/abs/2205.03892v2)
	- #CODE https://github.com/Alpha-VL/ConvMAE

### Vision transformers with convolutions
- #PAPER [CeiT - Incorporating Convolution Designs into Visual Transformers (Yan 2021)](https://arxiv.org/abs/2103.11816v1)
	- #CODE https://paperswithcode.com/paper/incorporating-convolution-designs-into-visual
	- CeiT combines the advantages of CNNs in extracting low-level features, strengthening locality, and the advantages of Transformers in establishing long-range dependencies
- #PAPER [TransUNet: Transformers Make Strong Encoders for Medical Image Segmentation (Chen 2021)](https://arxiv.org/abs/2102.04306v1)
	- #CODE https://paperswithcode.com/paper/transunet-transformers-make-strong-encoders
	- due to the intrinsic locality of convolution operations, U-Net generally demonstrates limitations in explicitly modeling long-range dependency
	- TransUNet merits both Transformers and U-Net, as a strong alternative for medical image segmentation
	- transformer encodes tokenized image patches from a convolution neural network (CNN) feature map as the input sequence for extracting global contexts
	- on the other hand, the decoder upsamples the encoded features which are then combined with the high-resolution CNN feature maps to enable precise localization
	- #TALK [Paper explained](https://www.youtube.com/watch?v=jKBJITQ8xJY)
- #PAPER [Escaping the Big Data Paradigm with Compact Transformers (Hassani 2021)](https://arxiv.org/abs/2104.05704) ^cctransformer
	- Compact Convolutional Transformer (CCT)
	- #CODE https://github.com/SHI-Labs/Compact-Transformers
	- #CODE https://keras.io/examples/vision/cct/
	- ViTs (or a typical Transformer-based architecture) do not have well-informed inductive biases (such as convolutions for processing images)
	- Attempt to combine the benefits of convolution and the benefits of Transformers in a single network architecture
	- These benefits include parameter-efficiency, and self-attention to process long-range and global dependencies (interactions between different regions in an image)
	- Patching (VIT-like) and embedding is already a convolution in itself, albeit non-overlapping. This is replaced with overlapping (regular) convolutions
	- Better performance on CIFAR-10 than VIT, so it's efficient on smaller datasets, comparable with SOTA CNNs
	- #TALK [Escaping the Big Data Paradigm with Compact Transformers (Humphrey Shi)](https://www.youtube.com/watch?v=AEWhf_hMBgs)
- #PAPER [CvT: Introducing Convolutions to Vision Transformers (Wu 2021)](https://arxiv.org/abs/2103.15808)
	- #CODE https://github.com/leoxiaobin/CvT
	- Convolutional vision Transformers (CvT) improves ViT in performance and efficienty by introducing convolutions into ViT to yield the best of both disignes
	- This is accomplished through two primary modifications: a hierarchy of Transformers containing a new convolutional token embedding, and a convolutional Transformer block leveraging a convolutional projection
	- These changes introduce desirable properties of CNNs to the ViT architecture (e.g. shift, scale, and distortion invariance) while maintaining the merits of Transformers (e.g. dynamic attention, global context, and better generalization)
- #PAPER [Combining EfficientNet and Vision Transformers for Video Deepfake Detection (Coccomini 2021)](https://arxiv.org/abs/2107.02612)
	- [Vision Transformers or Convolutional Neural Networks? Both!](https://towardsdatascience.com/vision-transformers-or-convolutional-neural-networks-both-de1a2c3c62e4)
- #PAPER [Early Convolutions Help Transformers See Better (Xiao 2021)](https://arxiv.org/abs/2106.14881)
	- https://syncedreview.com/2021/07/06/deepmind-podracer-tpu-based-rl-frameworks-deliver-exceptional-performance-at-low-cost-55/
	- replacing the ViT patchify stem with a standard convolutional stem in early visual processing results in marked improvements in terms of optimizer stability and final model accuracy
- #PAPER [ConViT: Improving Vision Transformers with Soft Convolutional Inductive Biases (d'ascoli 2021)](https://arxiv.org/abs/2103.10697)
	- #CODE https://github.com/facebookresearch/convit
	- https://ai.facebook.com/blog/computer-vision-combining-transformers-and-convolutional-neural-networks/
- #PAPER [CMT: Convolutional Neural Networks Meet Vision Transformers (Guo 2021)](https://arxiv.org/abs/2107.06263)
- #PAPER [CoAtNet: Marrying Convolution and Attention for All Data Sizes (Dai 2021)](https://arxiv.org/abs/2106.04803)
	- https://ai.googleblog.com/2021/09/toward-fast-and-accurate-neural.html
- #PAPER [UniFormer: Unifying Convolution and Self-attention for Visual Recognition (Li 2022)](https://arxiv.org/abs/2201.09450v1)
	- #CODE https://paperswithcode.com/paper/uniformer-unifying-convolution-and-self?from=n24
- #PAPER [Convolutional Xformers for Vision (Jeevan 2022)](https://arxiv.org/abs/2201.10271v1)
	- #CODE https://github.com/pranavphoenix/CXV
- #PAPER [Patches Are All You Need? (Trockman 2022)](https://arxiv.org/pdf/2201.09792)            
	- #CODE https://github.com/locuslab/convmixer
	- https://scoste.fr/posts/convmixer/index.html
	- https://medium.com/codex/an-overview-on-convmixer-patches-are-all-you-need-8502a8d87011
- #PAPER [The Fully Convolutional Transformer for Medical Image Segmentation (Tragakis 2022)](https://arxiv.org/abs/2206.00566v1)
	- #CODE https://github.com/Thanos-DB/FullyConvolutionalTransformer

## Multi-modal transformers
See [[AI/Deep learning/Multimodal learning]]

## For RL
See ^decisiontransformer in [[AI/Reinforcement learning]]