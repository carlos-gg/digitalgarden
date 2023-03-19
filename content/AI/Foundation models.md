---
title: "Foundation models"
---

> A foundation model is a large artificial intelligence model trained on a vast quantity of unlabeled data at scale (usually by [[AI/Self-supervised learning]]) resulting in a model that can be adapted to a wide range of downstream tasks

> See [[AI/Deep learning/Multimodal learning]]

## Resources
- https://en.wikipedia.org/wiki/Foundation_models
- [Center for Research on Foundation Models (CRFM)](https://hai.stanford.edu/news/introducing-center-research-foundation-models-crfm)
- [Foundation Models and the Future of Multi-Modal AI](https://lastweekin.ai/p/multi-modal-ai)
- [Foundation models: 2022’s AI paradigm shift](https://venturebeat.com/ai/foundation-models-2022s-ai-paradigm-shift/)
- [ChatGPT, LLMs, and Foundation models — a closer look into the hype and implications for startups](https://betterprogramming.pub/chatgpt-llms-and-foundation-models-a-closer-look-into-the-hype-and-implications-for-startups-b2f1d82f4d46)
- [Foundation Models: paradigm shift for AI or mere rebranding?](https://www.artificialintelligence.news/foundation-models-paradigm-shift-for-ai-or-mere-rebranding/)

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
	- [Typingmind](https://www.typingmind.com/) - A better UI for ChatGPT
	- [ChatGPT Cheat Sheet for Data Science](https://www.datacamp.com/cheat-sheet/chatgpt-cheat-sheet-data-science)
	- [How to Train an AI Chatbot With Custom Knowledge Base Using ChatGPT API](https://beebom.com/how-train-ai-chatbot-custom-knowledge-base-chatgpt-api/)
- #PAPER [LLaMA: Open and Efficient Foundation Language Models (Touvron 2023)](https://arxiv.org/pdf/2302.13971)
	- [Introducing LLaMA: A foundational, 65-billion-parameter large language model](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/)
	- [Paper explained](https://www.youtube.com/watch?v=E5OnoYF2oAk)
	- #CODE [Dalai](https://github.com/cocktailpeanut/dalai) - The simplest way to run LLaMA on your local machine
- #PAPER [GPT-4 Technical Report (OpenAI 2023)](https://cdn.openai.com/papers/gpt-4.pdf)
	- https://openai.com/product/gpt-4
	- [Paper explained](https://www.youtube.com/watch?v=2zW33LfffPc&t=8s)
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

