---
title: "Diffusion models"
---


## Resources
- [Diffusion models are autoencoders (Dieleman | Deepmind)](https://benanne.github.io/2022/01/31/diffusion.html "Diffusion models are autoencoders")
- [High Fidelity Image Generation Using Diffusion Models](http://ai.googleblog.com/2021/07/high-fidelity-image-generation-using.html "High Fidelity Image Generation Using Diffusion Models")
- [Introduction to deep generative modeling: Diffusion-based Deep Generative Models](https://jmtomczak.github.io/blog/10/10_ddgms_lvm_p2.html)

## References
- #PAPER [Improved Denoising Diffusion Probabilistic Models (Nichol 2021)](https://arxiv.org/abs/2102.09672)
- #PAPER [Cascaded Diffusion Models for High Fidelity Image Generation (Ho 2021)](https://cascaded-diffusion.github.io/)
- #PAPER [Diffusion Models Beat GANs on Image Synthesis (Dhariwal 2021)](https://arxiv.org/abs/2105.05233v3)
	- #CODE https://github.com/openai/guided-diffusion
	- Diffusion models are a class of likelihood-based models that have shown to produce high-quality images with desired properties such as distribution coverage and easy scalability. These models generate samples by gradually removing noise from a signal. Previous research has shown that they improve reliably with increased compute. The proposed method brings improvements to diffusions models that have worked for GANs, such as improved model architecture and a scheme to trade off diversity for quality. The proposed diffusion model achieves several state-of-the-art results, surpassing GANs on several metrics and datasets
	- [Paper explained](https://www.youtube.com/watch?v=W-O7AZNzbzQ)
- #PAPER [Imagen - Photorealistic Text-to-Image Diffusion Models with Deep Language Understanding (Saharia 2022)](https://arxiv.org/pdf/2205.11487v1)            
	- https://imagen.research.google/
	- Imagen, a text-to-image diffusion model with an unprecedented degree of photorealism and a deep level of language understanding. Imagen builds on the power of large transformer language models in understanding text and hinges on the strength of diffusion models in high-fidelity image generation
	- #CODE https://paperswithcode.com/paper/photorealistic-text-to-image-diffusion-models