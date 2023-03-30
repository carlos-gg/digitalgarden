---
title: "Diffusion models"
---

> Diffusion Models are generative models that work by destroying training data through the successive addition of Gaussian noise, and then learning to recover the data by reversing this noising process. After training, the Diffusion Model can be used to generate data by simply passing randomly sampled noise through the learned denoising process

> See [[AI/Deep learning/Multimodal learning]]

## Resources
- [Diffusion models are autoencoders (Dieleman | Deepmind)](https://benanne.github.io/2022/01/31/diffusion.html "Diffusion models are autoencoders")
- [Guidance: a cheat code for diffusion models (Dieleman | Deepmind)](https://benanne.github.io/2022/05/26/guidance.html "Guidance: a cheat code for diffusion models")
- [High Fidelity Image Generation Using Diffusion Models](http://ai.googleblog.com/2021/07/high-fidelity-image-generation-using.html "High Fidelity Image Generation Using Diffusion Models")
- [Introduction to deep generative modeling: Diffusion-based Deep Generative Models](https://jmtomczak.github.io/blog/10/10_ddgms_lvm_p2.html)
- [Introduction to Diffusion Models for Machine Learning](https://www.assemblyai.com/blog/diffusion-models-for-machine-learning-introduction/)
- Improving Diffusion Models as an Alternative To GANs
	- [Part 1](https://developer.nvidia.com/blog/improving-diffusion-models-as-an-alternative-to-gans-part-1/)
	- [Part 2](https://developer.nvidia.com/blog/improving-diffusion-models-as-an-alternative-to-gans-part-2/)
- [What are Diffusion Models?](https://lilianweng.github.io/posts/2021-07-11-diffusion-models/) - Lilian Weng
- [Diffusion models from scratch in PyTorch](https://www.youtube.com/watch?v=a4Yfz2FxXiY)
- [An In-Depth Guide to Denoising Diffusion Probabilistic Models – From Theory to Implementation](https://learnopencv.com/denoising-diffusion-probabilistic-models/)

## Talks
- #TALK [Diffusion Probabilistic Models](https://www.youtube.com/watch?v=XCUlnHP1TNM) - MIT, Jascha Sohl-Dickstein
- #TALK [What are Diffusion Models?](https://www.youtube.com/watch?v=fbLgFrlTnGU) - Ari Seff, math explained
- #TALK [Diffusion models explained. How does OpenAI's GLIDE work?](https://www.youtube.com/watch?v=344w5h24-h8) - AI Coffee break with Laetitia

## Code
- #CODE [Diffusers](https://github.com/huggingface/diffusers) (huggingface)
	- Diffusers provides pretrained diffusion models across multiple modalities, such as vision and audio, and serves as a modular toolbox for inference and training of diffusion models
	- https://towardsdatascience.com/hugging-face-just-released-the-diffusers-library-846f32845e65
	- #TALK https://www.youtube.com/watch?v=UzkdOg7wWmI

## References
- #PAPER [Denoising Diffusion Probabilistic Models (Ho 2020)](https://arxiv.org/pdf/2006.11239)
	- #CODE https://github.com/hojonathanho/diffusion
	- #CODE https://keras.io/examples/generative/ddpm/
- #PAPER [Diffusion Models Beat GANs on Image Synthesis (Dhariwal 2021)](https://arxiv.org/abs/2105.05233v3)
	- #CODE https://github.com/openai/guided-diffusion
	- Diffusion models are a class of likelihood-based models that have shown to produce high-quality images with desired properties such as distribution coverage and easy scalability. These models generate samples by gradually removing noise from a signal.
	- The proposed method brings improvements to diffusions models that have worked for GANs, such as improved model architecture and a scheme to trade off diversity for quality. The proposed diffusion model achieves several state-of-the-art results, surpassing GANs on several metrics and datasets
	- [Paper explained](https://www.youtube.com/watch?v=W-O7AZNzbzQ)
- #PAPER [Improved Denoising Diffusion Probabilistic Models (Nichol 2021)](https://arxiv.org/abs/2102.09672)
- #PAPER [Cascaded Diffusion Models for High Fidelity Image Generation (Ho 2021)](https://cascaded-diffusion.github.io/)
- #PAPER [Classifier-Free Diffusion Guidance (Ho 2022)](https://arxiv.org/pdf/2207.12598)
- #PAPER #REVIEW [Understanding Diffusion Models: A Unified Perspective (Luo 2022)](https://arxiv.org/pdf/2208.11970)
- #PAPER [High-Resolution Image Synthesis with Latent Diffusion Models (Rombach 2022)](https://arxiv.org/abs/2112.10752)
- #PAPER [Palette: Image-to-Image Diffusion Models (Saharia 2022)](https://arxiv.org/pdf/2111.05826)
	- https://iterative-refinement.github.io/palette/
	- #CODE https://github.com/Janspiry/Palette-Image-to-Image-Diffusion-Models