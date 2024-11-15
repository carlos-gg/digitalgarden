---
title: "Multimodal learning"
---

> General-purpose neural networks capable of handling diverse inputs and output tasks
> 
> See [[AI/Generative AI/Foundation models]]

## Resources
- [Multimodal Deep Learning](https://multimodal-dl.mpi-inf.mpg.de/)
- https://paperswithcode.com/methods/category/vision-and-language-pre-trained-models
- [Vision Language models: towards multi-modal deep learning](https://theaisummer.com/vision-language-models/)

## Code
- #CODE [Pykale](https://github.com/pykale/pykale) - Knowledge-Aware machine LEarning (KALE): accessible machine learning from multiple sources for interdisciplinary research
- #CODE [Unilm](https://github.com/microsoft/unilm) - Large-scale Self-supervised Pre-training Across Tasks, Languages, and Modalities

## Courses
- #COURSE [Multimodal Machine Learning (Carnegie Mellon University)](https://www.youtube.com/watch?v=VIq5r7mCAyw&list=PL-Fhd_vrvisNup9YQs_TdLW7DQz-lda0G)
	- https://cmu-multicomp-lab.github.io/mmml-course/fall2020/

## Books
- #BOOK [Multimodal Deep Learning (Akkus 2023)](https://arxiv.org/abs/2301.04856)
		- https://slds-lmu.github.io/seminar_multimodal_dl/index.html

## References
- #PAPER [Multi-modal Transformer for Video Retrieval (Gabeur 2020)](https://arxiv.org/abs/2007.10639)
- #PAPER #REVIEW [Recent Advances and Trends in Multimodal Deep Learning: A Review (Summaira 2021)](https://arxiv.org/abs/2105.11087)
- #PAPER [Perceiver: General Perception with Iterative Attention (Jaegle 2021)](https://arxiv.org/abs/2103.03206)
	- https://www.zdnet.com/article/googles-supermodel-deepmind-perceiver-is-a-step-on-the-road-to-an-ai-machine-that-could-process-everything/
	- Multi-model with image, audio, video, 3d point clouds
- #PAPER [PyKale: Knowledge-Aware Machine Learning from Multiple Sources in Python (Lu 2021)](https://arxiv.org/abs/2106.09756v1) ^pykale
- #PAPER [Perceiver IO: A General Architecture for Structured Inputs & Outputs (Jaegle 2021)](https://arxiv.org/abs/2107.14795v2)
	- #CODE https://paperswithcode.com/paper/perceiver-io-a-general-architecture-for
- #PAPER [VATT: Transformers for Multimodal Self-Supervised Learning from Raw Video, Audio and Text (Akbari 2021)](https://arxiv.org/abs/2104.11178v2)
	- #CODE https://paperswithcode.com/paper/vatt-transformers-for-multimodal-self
	- VATT is trained to learn multimodal representations from unlabeled data using Transformer architectures
- #PAPER [NÜWA: Visual Synthesis Pre-training for Neural visUal World creAtion (Wu 2021)](https://arxiv.org/abs/2111.12417v1)
	- #CODE https://paperswithcode.com/paper/nuwa-visual-synthesis-pre-training-for-neural
	- [Paper explained](https://www.youtube.com/watch?v=InhMx1h0N40&list=WL&index=50)
	- NÜWA consists of an adaptive encoder that takes either text or visual input, and a pre-trained decoder shared by 8 visual tasks
	- 3D Nearby Attention mechanism (3DNA) is proposed to reduce computational complexity and improve visual quality of results, by considering the locality characteristics for both spatial and temporal axes to better deal with the nature of the visual data
- #PAPER [data2vec: A General Framework for Self-supervised Learning in Speech, Vision and Language (Baevski 2022)](https://arxiv.org/abs/2202.03555)
	- #CODE https://github.com/pytorch/fairseq/tree/main/examples/data2vec
	- https://ai.facebook.com/blog/the-first-high-performance-self-supervised-algorithm-that-works-for-speech-vision-and-text/
- #PAPER [A Generalist Agent (Reed 2022)](https://arxiv.org/abs/2205.06175v1)
	- [Paper explained](https://www.youtube.com/watch?v=wSQJZHfAg18)
	- New approach, inspired by large-scale language models, that acts a single generalist agent. The agent, called Gato, is built to work as a multi-modal, multi-task, multi-embodiment generalist policy
- #PAPER [Language Models are General-Purpose Interfaces (Hao 2022)](https://arxiv.org/pdf/2206.06336v1)
	- #CODE https://github.com/microsoft/unilm
- #PAPER [NUWA-Infinity: Autoregressive over Autoregressive Generation for Infinite Visual Synthesis (Wu 2022)](https://arxiv.org/pdf/2207.09814)
	- #CODE https://github.com/microsoft/NUWA
	- https://nuwa-infinity.microsoft.com/#/

### Vision and language models
- #PAPER [DALL-E - Creating Images from Text (Ramesh 2021)](https://openai.com/blog/dall-e/)
	- https://www.technologyreview.com/2021/01/05/1015754/avocado-armchair-future-ai-openai-deep-learning-nlp-gpt3-computer-vision-common-sense/
	- [Blogpost explained](https://www.youtube.com/watch?v=j4xgkjWlfL4)
	- #CODE https://github.com/EleutherAI/DALLE-mtf
	- Multi-modal text and vision
	- [DALL-E mini](https://wandb.ai/dalle-mini/dalle-mini/reports/DALL-E-mini--Vmlldzo4NjIxODA)
- #PAPER [Learning Transferable Visual Models From Natural Language Supervision (Radford 2021)](https://arxiv.org/pdf/2103.00020v1)            
	- #CODE https://paperswithcode.com/paper/learning-transferable-visual-models-from#code
	- #CODE https://github.com/openai/CLIP
- #PAPER [SimVLM: Simple Visual Language Model Pretraining with Weak Supervision (Wang 2022)](https://arxiv.org/pdf/2108.10904v2)            
- #PAPER [Unifying Architectures, Tasks, and Modalities Through a Simple Sequence-to-Sequence Learning Framework (Wang 2022)](https://arxiv.org/pdf/2202.03052v1)            
- #PAPER [Flamingo: a Visual Language Model for Few-Shot Learning (Alayrac 2022)](https://arxiv.org/abs/2204.14198v1)
	- #CODE https://github.com/lucidrains/flamingo-pytorch
	- https://www.deepmind.com/blog/tackling-multiple-tasks-with-a-single-visual-language-model
- #PAPER [LViT: Language meets Vision Transformer in Medical Image Segmentation (Li 2022)](https://arxiv.org/abs/2206.14718v1) ^lvit
	- #CODE https://github.com/HUANGLIZI/LViT
- #PAPER [Scaling Autoregressive Models for Content-Rich Text-to-Image Generation (Yu 2022)](https://arxiv.org/pdf/2206.10789v1)
	- #CODE https://github.com/google-research/parti
	- https://parti.research.google/
	- Pathways Autoregressive Text-to-Image model (Parti), an autoregressive text-to-image generation model that achieves high-fidelity photorealistic image generation and supports content-rich synthesis involving complex compositions and world knowledge
- #PAPER [CogView2: Faster and Better Text-to-Image Generation via Hierarchical Transformers (Ding 2022)](https://arxiv.org/pdf/2204.14217)
	- #CODE https://github.com/THUDM/CogView2
- #PAPER [Imagen - Photorealistic Text-to-Image Diffusion Models with Deep Language Understanding (Saharia 2022)](https://arxiv.org/pdf/2205.11487v1)            
	- https://imagen.research.google/
	- Imagen, a text-to-image diffusion model with an unprecedented degree of photorealism and a deep level of language understanding. Imagen builds on the power of large transformer language models in understanding text and hinges on the strength of diffusion models in high-fidelity image generation
	- #CODE https://paperswithcode.com/paper/photorealistic-text-to-image-diffusion-models
- #PAPER [Unified-IO: A Unified Model for Vision, Language, and Multi-Modal Tasks (Lu 2022)](https://arxiv.org/pdf/2206.08916)
	- https://unified-io.allenai.org/
- #PAPER #REVIEW [A Survey of Vision-Language Pre-Trained Models (Du 2022)](https://arxiv.org/pdf/2202.10936)            
- #PAPER #REVIEW [The Creativity of Text-to-Image Generation (Oppenlaender 2022)](https://arxiv.org/pdf/2206.02904)
- #PAPER [MultiMAE: Multi-modal Multi-task Masked Autoencoders (Bachman 2022)](https://arxiv.org/pdf/2204.01678)
	- https://medium.com/syncedreview/epfls-multi-modal-multi-task-masked-autoencoder-a-simple-flexible-and-effective-vit-pretraining-3185c4aa62fc
- #PAPER [GLIGEN: Open-Set Grounded Text-to-Image Generation (Li 2023)](https://arxiv.org/pdf/2301.07093)
	- https://gligen.github.io/
	- https://huggingface.co/spaces/gligen/demo
	- https://the-decoder.com/gligen-gives-you-more-control-over-ai-image-generation/
- #PAPER [Scaling up GANs for Text-to-Image Synthesis (Kang 2023)](https://arxiv.org/pdf/2303.05511)
	- [[AI/Deep learning/GANs]]
	- [Scaling up GANs for Text-to-Image Synthesis](https://mingukkang.github.io/GigaGAN/)
- #PAPER [OpenFlamingo (Awadalla 2023)](https://laion.ai/blog/open-flamingo/)
	- An open-source framework for training vision-language models with in-context learning (like GPT-4!)
	- Includes a Python framework to train Flamingo-style LMMs, a large-scale multimodal dataset with interleaved image and text sequences, an in-context learning evaluation benchmark for vision-language tasks and a trained models (eg OpenFlamingo-9B model based on LLaMA)
	- [Demo](https://7164d2142d11.ngrok.app/)
- #PAPER [Modulating Pretrained Diffusion Models for Multimodal Image Synthesis (Ham 2023)](https://arxiv.org/pdf/2302.12764)
	- https://www.marktechpost.com/2023/03/16/one-diffusion-to-rule-diffusion-modulating-pre-trained-diffusion-models-for-multimodal-image-synthesis/
	- [[AI/Deep learning/Diffusion models]]
- #PAPER[4M-21: An Any-to-Any Vision Model for Tens of Tasks and Modalities (2024)](https://arxiv.org/pdf/2406.09406)
	-  https://4m.epfl.ch/
	- #CODE https://github.com/apple/ml-4m?tab=readme-ov-file&utm_source=pocket_shared
