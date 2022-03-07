---
title: "Multimodal learning"
disableToc: false 
---

# Resources
- General-purpose neural networks capable of handling diverse inputs and output tasks
- Multimodal Deep Learning: https://multimodal-dl.mpi-inf.mpg.de/

# Code
- #CODE Pykale (in pytorch): https://github.com/pykale/pykale
	- [[#^pykale]]

# References
Review papers:
- #PAPER Recent Advances and Trends in Multimodal Deep Learning: A Review (Summaira 2021): https://arxiv.org/abs/2105.11087

- #PAPER Multi-modal Transformer for Video Retrieval (Gabeur 2020): https://arxiv.org/abs/2007.10639
- #PAPER DALL-E - Creating Images from Text (Ramesh 2021): https://openai.com/blog/dall-e/ ^dall-e
	- https://www.technologyreview.com/2021/01/05/1015754/avocado-armchair-future-ai-openai-deep-learning-nlp-gpt3-computer-vision-common-sense/
	- Blogpost explained: https://www.youtube.com/watch?v=j4xgkjWlfL4
	- #CODE https://github.com/EleutherAI/DALLE-mtf
	- Multi-modal text and speech
	- DALL-E mini: https://wandb.ai/dalle-mini/dalle-mini/reports/DALL-E-mini--Vmlldzo4NjIxODA
- #PAPER Perceiver: General Perception with Iterative Attention (Jaegle 2021): https://arxiv.org/abs/2103.03206
	- https://www.zdnet.com/article/googles-supermodel-deepmind-perceiver-is-a-step-on-the-road-to-an-ai-machine-that-could-process-everything/
	- Multi-model with image, audio, video, 3d point clouds
- #PAPER PyKale: Knowledge-Aware Machine Learning from Multiple Sources in Python (Lu 2021): https://arxiv.org/abs/2106.09756v1 ^pykale
- #PAPER Perceiver IO: A General Architecture for Structured Inputs & Outputs (Jaegle 2021): https://arxiv.org/abs/2107.14795v2
	- #CODE https://paperswithcode.com/paper/perceiver-io-a-general-architecture-for
- #PAPER VATT: Transformers for Multimodal Self-Supervised Learning from Raw Video, Audio and Text (Akbari 2021): https://arxiv.org/abs/2104.11178v2
	- #CODE https://paperswithcode.com/paper/vatt-transformers-for-multimodal-self
	- VATT is trained to learn multimodal representations from unlabeled data using Transformer architectures
- #PAPER NÜWA: Visual Synthesis Pre-training for Neural visUal World creAtion (Wu 2021): https://arxiv.org/abs/2111.12417v1
	- #CODE https://paperswithcode.com/paper/nuwa-visual-synthesis-pre-training-for-neural
	- Paper explained: https://www.youtube.com/watch?v=InhMx1h0N40&list=WL&index=50
	- NÜWA consists of an adaptive encoder that takes either text or visual input, and a pre-trained decoder shared by 8 visual tasks
	- 3D Nearby Attention mechanism (3DNA) is proposed to reduce computational complexity and improve visual quality of results, by considering the locality characteristics for both spatial and temporal axes to better deal with the nature of the visual data
