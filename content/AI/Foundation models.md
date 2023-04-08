---
title: "Foundation models"
---

> A foundation model is a large artificial intelligence model trained on a vast quantity of unlabeled data at scale (usually by [[AI/Self-supervised learning]]) resulting in a model that can be adapted to a wide range of downstream tasks

> See:
> - [[AI/Deep learning/Multimodal learning]]
> - [[AI/Deep learning/Generative modelling]]

## Resources
- https://en.wikipedia.org/wiki/Foundation_models
- https://en.wikipedia.org/wiki/Large_language_model
- [Center for Research on Foundation Models (CRFM)](https://hai.stanford.edu/news/introducing-center-research-foundation-models-crfm)
- [Foundation Models and the Future of Multi-Modal AI](https://lastweekin.ai/p/multi-modal-ai)
- [Foundation models: 2022’s AI paradigm shift](https://venturebeat.com/ai/foundation-models-2022s-ai-paradigm-shift/)
- [Foundation Models: paradigm shift for AI or mere rebranding?](https://www.artificialintelligence.news/foundation-models-paradigm-shift-for-ai-or-mere-rebranding/)
- [ChatGPT, LLMs, and Foundation models — a closer look into the hype and implications for startups](https://betterprogramming.pub/chatgpt-llms-and-foundation-models-a-closer-look-into-the-hype-and-implications-for-startups-b2f1d82f4d46)
- [AI Image Generators Compared Side-By-Side Reveals Stark Differences](https://petapixel.com/2022/08/22/ai-image-generators-compared-side-by-side-reveals-stark-differences/)
- [Illustrating Reinforcement Learning from Human Feedback (RLHF)](https://huggingface.co/blog/rlhf)
	- [RLHF+CHATGPT: What you must know](https://www.youtube.com/watch?v=PBH2nImUM5c)
- [Langchain JS | How to Use GPT-3, GPT-4 to Reference your own Data | OpenAI Embeddings Intro](https://www.youtube.com/watch?v=veV2I-NEjaM)

### Language models
- [GPT-4](https://openai.com/product/gpt-4)
	- [OpenAI GPT-4 - The Future Is Here!](https://www.youtube.com/watch?v=7VSWyghVZIg)
- [LLaMA](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/)
- [Introducing The World’s Largest Open Multilingual Language Model: BLOOM](https://bigscience.huggingface.co/blog/bloom)
	- https://www.nature.com/articles/d41586-022-01705-z
- [YaLM-100B](https://github.com/yandex/YaLM-100B)

#### AI-based conversational models and search engines
- [Bing chat](https://www.bing.com/search?q=Bing+AI&showconv=1&FORM=hpcodx)
- [Claude](https://www.anthropic.com/index/introducing-claude)
- [ChatGPT](https://openai.com/blog/chatgpt)
	- [ChatGPT Gets Its “Wolfram Superpowers”!](https://writings.stephenwolfram.com/2023/03/chatgpt-gets-its-wolfram-superpowers/)
	- [Typingmind](https://www.typingmind.com/) - A better UI for ChatGPT
	- [ChatGPT Cheat Sheet for Data Science](https://www.datacamp.com/cheat-sheet/chatgpt-cheat-sheet-data-science)
	- [How to Train an AI Chatbot With Custom Knowledge Base Using ChatGPT API](https://beebom.com/how-train-ai-chatbot-custom-knowledge-base-chatgpt-api/)
- [Bard](https://blog.google/technology/ai/bard-google-ai-search-updates/)
- [You chat](https://you.com/search?q=who+are+you&tbm=youchat&cfr=chat)
- [Perplexity.ai](https://www.perplexity.ai/)
- [Exper AI](https://www.experai.com/)
- [Neeva](https://neeva.com/)
- [Humata](https://www.humata.ai/) - Ask AI anything about your files
- [Explainpaper](https://www.explainpaper.com/) - Understand papers instantly

### Vision Models
- [Midjourney](https://www.midjourney.com/home/)
- [DALLE-2](https://openai.com/dall-e-2/)
- [IMAGEN](https://imagen.research.google/)
- [IMAGEN video](https://imagen.research.google/video/)
- [Stable Diffusion](https://stability.ai/blog/stable-diffusion-announcement)
	- #CODE https://github.com/CompVis/stable-diffusion
	- #CODE https://github.com/divamgupta/stable-diffusion-tensorflow
	- [DreamStudio](https://beta.dreamstudio.ai) 
	- [Two minute papers](https://www.youtube.com/watch?v=nVhmFski3vg)
	- [Stable Diffusion: High-Resolution Image Synthesis with Latent Diffusion Models | ML Coding Series](https://www.youtube.com/watch?v=f6PtJKdey8E)
	- [Stable Diffusion is a really big deal](https://simonwillison.net/2022/Aug/29/stable-diffusion/)
- [Make-A-Video](https://makeavideo.studio/)
- [Leonardo.AI](https://leonardo.ai/)

## Courses
- #COURSE [Large Language Models (Stanford CS324)](https://stanford-cs324.github.io/winter2022/)

## References
- #PAPER [On the Opportunities and Risks of Foundation Models (Bommasani 2021)](https://arxiv.org/abs/2108.07258)
	- A foundation model is any model that is trained on broad data at scale and can be adapted (e.g., fine-tuned) to a wide range of downstream tasks; current examples include BERT, GPT-3, and CLIP
	- Foundation models are based on deep neural networks and self-supervised learning
	- On a technical level, foundation models are enabled by transfer learning and scale
	- The idea of transfer learning is to take the “knowledge” learned from one task (e.g., object recognition in images) and apply it to another task (e.g., activity recognition in videos).
	- Within deep learning, pretraining is the dominant approach to transfer learning: a model is trained on a surrogate task (often just as a means to an end) and then adapted to the downstream task of interest via fine-tuning
	- Transfer learning is what makes foundation models possible, but scale is what makes them powerful. Scale required three ingredients: improvements in computer hardware, the development of the Transformer model architecture that leverages the parallelism of the hardware to train much more expressive models than before and the availability of much more training data
- #PAPER [Florence: A New Foundation Model for Computer Vision (Yuan 2021)](https://arxiv.org/pdf/2111.11432)
- #PAPER [Foundation Transformers (Wang 2022)](https://arxiv.org/pdf/2210.06423)
- #PAPER [InternImage: Exploring Large-Scale Vision Foundation Models with Deformable Convolutions (Wang 2022)](https://arxiv.org/pdf/2211.05778)
- #PAPER [Towards artificial general intelligence via a multimodal foundation model (Fei 2022)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9163040/)
- #PAPER [InstructGPT - Training language models to follow instructions with human feedback (Ouyang 2022)](https://arxiv.org/abs/2203.02155)
	- https://openai.com/blog/chatgpt
	- https://en.wikipedia.org/wiki/ChatGPT
	- See GPT-3 in [[AI/Deep learning/Transformers]] 
	- ChatGPT – a generative pre-trained transformer (GPT) – was fine-tuned on top of GPT-3.5 using [[Supervised learning]] as well as [[Reinforcement learning]]. Both approaches used human trainers to improve the model's performance. In the case of supervised learning, the model was provided with conversations in which the trainers played both sides: the user and the AI assistant. In the reinforcement learning step, human trainers first ranked responses that the model had created in a previous conversation. These rankings were used to create 'reward models' that the model was further fine-tuned on using several iterations of Proximal Policy Optimization (PPO)
- #PAPER [ChatGPT is not all you need. A State of the Art Review of large Generative AI models (Gozalo-Brizuela 2023)](https://arxiv.org/pdf/2301.04655)
- #PAPER [LLaMA: Open and Efficient Foundation Language Models (Touvron 2023)](https://arxiv.org/pdf/2302.13971)
	- [Introducing LLaMA: A foundational, 65-billion-parameter large language model](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/)
	- [Paper explained](https://www.youtube.com/watch?v=E5OnoYF2oAk)
	- #CODE [Dalai](https://github.com/cocktailpeanut/dalai) - The simplest way to run LLaMA on your local machine
- #PAPER [GPT-4 Technical Report (OpenAI 2023)](https://cdn.openai.com/papers/gpt-4.pdf)
	- https://openai.com/product/gpt-4
	- [Paper explained](https://www.youtube.com/watch?v=2zW33LfffPc&t=8s)
- #PAPER [ChatGPT: Jack of all trades, master of none (Kocon 2023)](https://arxiv.org/pdf/2302.10724)
- #PAPER [OpenChatKit (Together 2023)](https://www.together.xyz/blog/openchatkit)
	- https://huggingface.co/spaces/togethercomputer/OpenChatKit
	- [Together Releases The First Open-Source ChatGPT Alternative Called OpenChatKit](https://www.marktechpost.com/2023/03/12/together-releases-the-first-open-source-chatgpt-alternative-called-openchatkit/)
- #PAPER [Alpaca: A Strong, Replicable Instruction-Following Model (Taori 2023)](https://crfm.stanford.edu/2023/03/13/alpaca.html)
	- Fine-tuned LLaMA 7B model on 52K instruction-following demonstrations produced using OpenAI API
	- Performance qualitatively similar to OpenAI’s text-davinci-003, while being surprisingly small and easy/cheap to reproduce (<600$)
	- [Alpaca dataset](https://huggingface.co/datasets/tatsu-lab/alpaca)
	- https://the-decoder.com/stanfords-alpaca-shows-that-openai-may-have-a-problem/
	- https://github.com/tatsu-lab/stanford_alpaca#fine-tuning
	- [How to finetune your own Alpaca 7B](https://www.youtube.com/watch?v=LSoqyynKU9E)
	- https://huggingface.co/mrm8488/Alpacoom
- #PAPER [Visual ChatGPT: Talking, Drawing and Editing with Visual Foundation Models (Wu 2023)](https://arxiv.org/pdf/2303.04671)
	- Visual ChatGPT opens the door of combining ChatGPT and Visual Foundation Models and enables ChatGPT to handle complex visual tasks
- #PAPER [Sparks of Artificial General Intelligence: Early experiments with GPT-4 (Bubeck 2023)](https://arxiv.org/pdf/2303.12712)
	- [Paper explained](https://www.youtube.com/watch?v=Mqg3aTGNxZ0)