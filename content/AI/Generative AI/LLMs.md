---
title: LLMs
---
> Large Language Models are artificial intelligence models that are trained on vast amounts of text data to generate, understand, and generate human-like language. These models are designed to process and analyze large volumes of text, allowing them to learn patterns, relationships, and nuances in language. The development of Large Language Models has revolutionized the field of NLP, enabling applications like chatbots, virtual assistants, and language translation tools. They have also sparked significant advancements in areas like research, education, and entertainment.

> See: 
> - [[AI/Generative AI/Foundation models|Foundation models]]
> - [[AI/Generative AI/Agents|Agents]]
> - [[AI/Generative AI/LLM Ops|LLM Ops]]
> - [[AI/Generative AI/RAG|RAG]]
> - [[AI/Generative AI/Prompt engineering|Prompt engineering]]
> - [[AI/Generative AI/Fine tuning LLMs|Fine tuning LLMs]]

## Resources
- [eugeneyan/open-llms: 📋 A list of open LLMs available for commercial use. (github.com)](https://github.com/eugeneyan/open-llms)
- [NiuTrans/ABigSurveyOfLLMs: A collection of 150+ surveys on LLMs (github.com)](https://github.com/NiuTrans/ABigSurveyOfLLMs)
- [Question answering using embeddings-based search | OpenAI Cookbook](https://cookbook.openai.com/examples/question_answering_using_embeddings)
- [Chat with your PDF: Using Langchain, F.A.I.S.S., and OpenAI to Query PDFs | by johnthuo | Medium](https://medium.com/@johnthuo/chat-with-your-pdf-using-langchain-f-a-i-s-s-and-openai-to-query-pdfs-e7bfde086155)
- [The Large Language Model (LLM) Index | Sapling](https://sapling.ai/llm/index)
- [Maxime Labonne - LLM Articles](https://mlabonne.github.io/blog/)
	- [Maxime Labonne - Merge Large Language Models with MergeKit](https://mlabonne.github.io/blog/posts/2024-01-08_Merge_LLMs_with_mergekit.html)
	- [Decoding strategies in LLMs](https://mlabonne.github.io/blog/posts/2023-06-07-Decoding_strategies.html) - understanding temperature, topk, topp, numbeams
- Pricing calculators:
	- [Free OpenAI & every-LLM API Pricing Calculator | Updated Nov 2024](https://docsbot.ai/tools/gpt-openai-api-pricing-calculator?utm_source=pocket_shared)
	- [LLM Cost Calculator: Compare OpenAI, Claude2, PaLM, Cohere & More](https://yourgpt.ai/tools/openai-and-other-llm-api-pricing-calculator?utm_source=pocket_saves)
	- [OpenAI API Pricing Calculator](https://gptforwork.com/tools/openai-chatgpt-api-pricing-calculator?utm_source=pocket_shared)
	- [OpenAI API Pricing Calculator | 100% Free](https://www.launchnow.pro/openai-chatgpt-api-pricing-calculator?utm_source=pocket_saves)
### APIs
 - OpenAI
	- [OpenAI Platform - Models](https://platform.openai.com/docs/models/models)
	- [OpenAI Platform - Assistants](https://platform.openai.com/docs/assistants/overview)
	- [Vision - OpenAI API](https://platform.openai.com/docs/guides/vision)
	- [GPT-4](https://openai.com/product/gpt-4)
		- [OpenAI GPT-4 - The Future Is Here!](https://www.youtube.com/watch?v=7VSWyghVZIg)
	- [ChatGPT (OpenAI)](https://openai.com/blog/chatgpt)
		- [ChatGPT Gets Its “Wolfram Superpowers”!](https://writings.stephenwolfram.com/2023/03/chatgpt-gets-its-wolfram-superpowers/)
		- [ChatGPT Cheat Sheet for Data Science](https://www.datacamp.com/cheat-sheet/chatgpt-cheat-sheet-data-science)
		- [How to Train an AI Chatbot With Custom Knowledge Base Using ChatGPT API](https://beebom.com/how-train-ai-chatbot-custom-knowledge-base-chatgpt-api/)
- https://openrouter.ai/  - A unified interface for LLMs
- [Groq is Fast AI Inference](https://groq.com/)
	- [GitHub - groq/groq-python: The official Python Library for the Groq API](https://github.com/groq/groq-python)
- HuggingFace [Serverless Inference API](https://huggingface.co/docs/api-inference/index)
### Benchmarks
- [Chat with Open Large Language Models (lmsys.org)](https://chat.lmsys.org/)
- [MMLU Benchmark (Multi-task Language Understanding) | Papers With Code](https://paperswithcode.com/sota/multi-task-language-understanding-on-mmlu)
- [Open LLM Leaderboard 2 - a Hugging Face Space by open-llm-leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard)
- [Chat bot arena](https://lmarena.ai/)
#### Metrics and evaluation
* First 3 could be the primary and the last 3 as secondary.
	- MixEval: A dynamic benchmark evaluating LLMs using real-world user queries and benchmarks, achieving a 0.96 model ranking correlation with Chatbot Arena. [https://mixeval.github.io/](https://mixeval.github.io/)  
	- IFEval: Assess the ability to follow detailed, verifiable instructions. For example, a prompt might instruct, "Write an article with more than 800 words" or "Wrap your response in double quotation marks". [https://lnkd.in/eq9PCFCT](https://lnkd.in/eq9PCFCT)  
	- Arena-Hard: Evaluating LLMs using challenging user queries, reflecting real-world preferences. Successor to MT-Bench and is similar to AlpacaEval 2.0, focusing on multi-turn conversations and instruction-following tasks. [https://lnkd.in/eV7pavKT](https://lnkd.in/eV7pavKT)  
	- MMLU (Pro/Redux): Testing on diverse subjects, evaluating zero-shot and few-shot settings. [https://lnkd.in/epgM393X](https://lnkd.in/epgM393X)  
	- GSM8K: Diverse grade school math problems for testing multi-step arithmetic reasoning. [https://lnkd.in/eiJUS-Uv](https://lnkd.in/eiJUS-Uv)  
	- HumanEval: Evaluating code generation models using hand-crafted programming problems and unit tests. [https://lnkd.in/eNcTCanG](https://lnkd.in/eNcTCanG)

### Tuning LLMs
- Tuning your LLM (prompt vs rag vs fine tuinig): [Full Fine-Tuning, PEFT, Prompt Engineering, or RAG? (deci.ai)](https://deci.ai/blog/fine-tuning-peft-prompt-engineering-and-rag-which-one-is-right-for-you/)
- [Domain specific generative AI: pre-training, fine-tuning & RAG — Elastic Search Labs](https://www.elastic.co/search-labs/blog/domain-specific-generative-ai-pre-training-fine-tuning-rag)
- Methods:
    - [[Prompt engineering]]
    - [[RAG]]
    - [[Fine tuning LLMs]]
    - RLHF: [Illustrating Reinforcement Learning from Human Feedback (RLHF) (huggingface.co)](https://huggingface.co/blog/rlhf)
        - [¿Qué es el RLHF? | IBM](https://www.ibm.com/mx-es/topics/rlhf)
### Quantization
- [Maxime Labonne - Quantize Llama models with GGUF and llama.cpp](https://mlabonne.github.io/blog/posts/Quantize_Llama_2_models_using_ggml.html)
- [LLM Quantization | GPTQ | QAT | AWQ | GGUF | GGML | PTQ](https://medium.com/@siddharth.vij10/llm-quantization-gptq-qat-awq-gguf-ggml-ptq-2e172cd1b3b5)
- [Quantization of LLMs with llama.cpp | by Ingrid Stevens | Medium](https://medium.com/@ingridwickstevens/quantization-of-llms-with-llama-cpp-9bbf59deda35#:~:text=cpp%2C%20Q4_K_M%20refers%20to%20a,means%20clustering%20in%20the%20quantization.)
### Interfaces, model hubs and UIs
- [Ollama](https://ollama.com/)
	- https://www.markhneedham.com/blog/2023/10/18/ollama-hugging-face-gguf-models/
- [GoLlama](https://github.com/sammcj/gollama) - Gollama is a macOS / Linux tool for managing Ollama models
- [Open-WebUI](https://github.com/open-webui/open-webui) - User-friendly WebUI for LLMs (Formerly Ollama WebUI)
- [Jan](https://jan.ai/)
	- https://github.com/janhq/jan
- [LM studio](https://lmstudio.ai/)
- [LLM farm](https://llmfarm.site/)
	- https://github.com/guinmoon/LLMFarm
- [Sanctum](https://sanctum.ai/)
- [Msty](https://msty.app/)
- [jasonacox/TinyLLM: Setup and run a local LLM and Chatbot using consumer grade hardware. (github.com)](https://github.com/jasonacox/TinyLLM)
    - Builds a local OpenAI API web service via ollama, vllm
    - Serves up a Chatbot web interface with customizable prompts, accessing external websites (URLs), vector databases and other sources (e.g. news, stocks, weather)
### Services and aplications
#### Tabular data
- [dreamquark-ai/tabnet: PyTorch implementation of TabNet paper : https://arxiv.org/pdf/1908.07442.pdf (github.com)](https://github.com/dreamquark-ai/tabnet)
    - #PAPER [[1908.07442] TabNet: Attentive Interpretable Tabular Learning (arxiv.org)](https://arxiv.org/abs/1908.07442?utm_source=pocket_reader)
    - [Tabular Deep Leaning: TabNet deep-dive - (francescopochetti.com)](https://francescopochetti.com/tabular-deep-leaning-tabnet-deep-dive/?utm_source=pocket_reader)
    - [OKUA1/tabnet-keras (github.com)](https://github.com/OKUA1/tabnet-keras)
- [automl/TabPFN: Official implementation of the TabPFN paper (https://arxiv.org/abs/2207.01848) and the tabpfn package. (github.com)](https://github.com/automl/TabPFN)
    - #PAPER [[2207.01848] TabPFN: A Transformer That Solves Small Tabular Classification Problems in a Second (arxiv.org)](https://arxiv.org/abs/2207.01848)
#### Time series data
See [[AI/Time Series analysis|Time Series analysis]]
- TimeGPT
	- #PAPER [[2310.03589] TimeGPT-1 (arxiv.org)](https://arxiv.org/abs/2310.03589)
    - [Nixtla/nixtla: TimeGPT-1: production ready pre-trained Time Series Foundation Model for forecasting and anomaly detection. Generative pretrained transformer for time series trained on over 100B data points. It's capable of accurately predicting various domains such as retail, electricity, finance, and IoT with just a few lines of code 🚀. (github.com)](https://github.com/Nixtla/nixtla)
    - [TimeGPT: The First Foundation Model for Time Series Forecasting | by Marco Peixeiro | Towards Data Science](https://towardsdatascience.com/timegpt-the-first-foundation-model-for-time-series-forecasting-bf0a75e63b3a)
- Chronos
	- [amazon-science/chronos-forecasting: Chronos: Pretrained (Language) Models for Probabilistic Time Series Forecasting (github.com)](https://github.com/amazon-science/chronos-forecasting)
    - #PAPER [\[2403.07815\] Chronos: Learning the Language of Time Series](https://arxiv.org/abs/2403.07815)
    - [Forecasting with Chronos - AutoGluon 1.1.0 documentation](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-chronos.html)
- TimesFM
	- #PAPER [[2310.10688] A decoder-only foundation model for time-series forecasting (arxiv.org)](https://arxiv.org/abs/2310.10688)
    - [google/timesfm-1.0-200m · Hugging Face](https://huggingface.co/google/timesfm-1.0-200m?utm_source=pocket_reader)
- TimesNet
	- #PAPER [[2210.02186] TimesNet: Temporal 2D-Variation Modeling for General Time Series Analysis (arxiv.org)](https://arxiv.org/abs/2210.02186)
    - [thuml/Time-Series-Library: A Library for Advanced Deep Time Series Models. (github.com)](https://github.com/thuml/Time-Series-Library)
    - [TimesNet: The Latest Advance in Time Series Forecasting | by Marco Peixeiro | Towards Data Science](https://towardsdatascience.com/timesnet-the-latest-advance-in-time-series-forecasting-745b69068c9c)
- MOMENT
	- #PAPER [[2402.03885] MOMENT: A Family of Open Time-series Foundation Models (arxiv.org)](https://arxiv.org/abs/2402.03885)
    - [AutonLab/MOMENT-1-large · Hugging Face](https://huggingface.co/AutonLab/MOMENT-1-large)
#### Search engines
- [Copilot](https://copilot.microsoft.com/)
- [You chat](https://you.com/search?q=who+are+you&tbm=youchat&cfr=chat)
- [Perplexity.ai](https://www.perplexity.ai/)
#### Chatbots
- [Chatbots | 🦜️🔗 Langchain](https://python.langchain.com/docs/use_cases/chatbots/)
- [Custom Chat Model | 🦜️🔗 Langchain](https://python.langchain.com/docs/modules/model_io/chat/custom_chat_model)
- Evaluación rendimiento:
    - [Métricas que te ayudarán a medir el éxito de tu chatbot - Gus](https://gus.chat/blog/metricas-para-medir-el-exito-de-tu-chatbot/)
    - [12 métricas para analizar el rendimiento de un chatbot - Planeta Chatbot](https://planetachatbot.com/metricas-para-analizar-el-rendimiento-de-un-chatbot/#:~:text=Aqu%C3%AD%20est%C3%A1n%20las%2012%20m%C3%A9tricas%20principales%2C%20en%20nuestra,de%20c%C3%B3mo%20se%20puede%20mejorar.%20...%20M%C3%A1s%20elementos)
    - [Evaluación de modelos de lenguaje grandes: una guía técnica - Unite.AI](https://www.unite.ai/es/evaluaci%C3%B3n-de-modelos-de-lenguaje-grandes-una-gu%C3%ADa-t%C3%A9cnica/)
#### NER
- [Named Entity Recognition to Enrich Text | OpenAI Cookbook](https://cookbook.openai.com/examples/named_entity_recognition_to_enrich_text)
#### Text-to-sql, dynamic reports and analysis
- #CODE [microsoft/lida: Automatic Generation of Visualizations and Infographics using Large Language Models (github.com)](https://github.com/microsoft/lida)
    - [LIDA | Automatically Generate Visualization with LLMs | The Future of Data Visualization | by Sunny Bhaveen Chandra | Medium](https://medium.com/@c17hawke/lida-automatically-generate-visualization-and-with-llms-the-future-of-data-visualization-6bc556876b46)
- [Graphext](https://www.graphext.com/) (paid service - startup)
- [Goodbye, Text2SQL: Why Table-Augmented Generation (TAG) is the Future of AI-Driven Data Queries! | by Pavan Emani | Sep, 2024 | Artificial Intelligence in Plain English](https://ai.plainenglish.io/goodbye-text2sql-why-table-augmented-generation-tag-is-the-future-of-ai-driven-data-queries-892e24e06922)
- [Text2SQL is Not Enough: Unifying AI and Databases with TAG](https://arxiv.org/html/2408.14717v1)
- [BIRD-bench](https://bird-bench.github.io/)
- [The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models](https://arxiv.org/html/2408.07702v2)
- LOTUS 
	- #PAPER [[2407.11418] LOTUS: Enabling Semantic Queries with LLMs Over Tables of Unstructured and Structured Data](https://arxiv.org/abs/2407.11418)
	- [TAG-Research/lotus: LOTUS: The semantic query engine - process data with LLMs as easily as writing pandas code](https://github.com/TAG-Research/lotus)
#### Medicine
- [Inteligencia Artificial en la Medicina | IBM](https://www.ibm.com/mx-es/topics/artificial-intelligence-medicine)
- [Elevating Healthcare Documentation With Generative AI (opendatascience.com)](https://opendatascience.com/elevating-healthcare-documentation-the-significance-of-soap-birp-and-the-promise-of-generative-ai/?utm_campaign=Newsletters&utm_medium=email&_hsenc=p2ANqtz-8eiEqdD2RmUZeW_8gBTEfT66SkjB32BLvRsvUrbMLcV1JIJfiJvzMpLn3EH5M-C0EAr4xwdOdTFvhWeZh_ENTx_6G_OUynAscJP8X5JGPJ3UBDQlo&_hsmi=305226791&utm_content=305211788&utm_source=hs_email)
- #PAPER [[2309.00087] Large language models in medicine: the potentials and pitfalls (arxiv.org)](https://arxiv.org/abs/2309.00087)
- #PAPER [[2403.03640] Apollo: An Lightweight Multilingual Medical LLM towards Democratizing Medical AI to 6B People (arxiv.org)](https://arxiv.org/abs/2403.03640)
    - [FreedomIntelligence/Apollo: Multilingual Medicine: Model, Dataset, Benchmark, Code (github.com)](https://github.com/FreedomIntelligence/Apollo)
- #PAPER [[2405.00715] Towards Adapting Open-Source Large Language Models for Expert-Level Clinical Note Generation (arxiv.org)](https://arxiv.org/abs/2405.00715)
- #PAPER [[2404.18416] Capabilities of Gemini Models in Medicine (arxiv.org)](https://arxiv.org/abs/2404.18416)
    - [Med-Gemini and Meditron: Google and Meta present new LLMs for medicine (the-decoder.com)](https://the-decoder.com/med-gemini-and-meditron-google-and-meta-present-new-llms-for-medicine/)
- #PAPER [[2402.12749] Me LLaMA: Foundation Large Language Models for Medical Applications (arxiv.org)](https://arxiv.org/abs/2402.12749)
- #PAPER [Paper page - ChatDoctor: A Medical Chat Model Fine-tuned on LLaMA Model using Medical Domain Knowledge (huggingface.co)](https://huggingface.co/papers/2303.14070)
- #PAPER [PMC-LLaMA: toward building open-source language models for medicine | Journal of the American Medical Informatics Association | Oxford Academic (oup.com)](https://academic.oup.com/jamia/advance-article-abstract/doi/10.1093/jamia/ocae045/7645318?redirectedFrom=fulltext)
- #PAPER [\[2311.16079\] MEDITRON-70B: Scaling Medical Pretraining for Large Language Models](https://arxiv.org/abs/2311.16079)
	- [epfLLM/meditron: Meditron is a suite of open-source medical Large Language Models (LLMs). (github.com)](https://github.com/epfLLM/meditron)
- #PAPER [[2311.16588v2] Ascle: A Python Natural Language Processing Toolkit for Medical Text Generation (arxiv.org)](https://arxiv.org/abs/2311.16588v2)
- Datasets:
    - [abachaa/Existing-Medical-QA-Datasets: Multimodal Question Answering in the Medical Domain: A summary of Existing Datasets and Systems (github.com)](https://github.com/abachaa/Existing-Medical-QA-Datasets)
    - [Andy-jqa/biomedical-qa-datasets: Biomedical Question Answering Datasets. (github.com)](https://github.com/Andy-jqa/biomedical-qa-datasets)
        - Español: [HEAD-QA | A Healthcare Dataset for Complex Reasoning (aghie.github.io)](https://aghie.github.io/head-qa/)

### LLMs in production
- [Creación de aplicaciones de IA generativa con modelos de base – Amazon Bedrock – AWS](https://aws.amazon.com/es/bedrock/?trk=68f42e87-3ae0-43b3-8101-9bc153ae3b39&sc_channel=ps&s_kwcid=AL!4422!10!71468517518479!71469056518657&ef_id=47853f94ebef1464e6be5a6e07726a57:G:s)
#### Servir LLMs
- [vllm-project/vllm: A high-throughput and memory-efficient inference and serving engine for LLMs (github.com)](https://github.com/vllm-project/vllm)
    - [Quickstart — vLLM](https://docs.vllm.ai/en/latest/getting_started/quickstart.html#openai-compatible-server)
- [https://docs.bentoml.org/en/v1.1.11/quickstarts/deploy-a-transformer-model-with-bentoml.html](https://docs.bentoml.org/en/v1.1.11/quickstarts/deploy-a-transformer-model-with-bentoml.html)
- [How to deploy Meta Llama models with Azure Machine Learning studio - Azure Machine Learning | Microsoft Learn](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-deploy-models-llama?view=azureml-api-2&tabs=llama-three)

## Courses
- #COURSE [LLM-twin-course](https://github.com/decodingml/llm-twin-course)
	- [The LLM-Twin Free Course on Production-Ready RAG applications | Decoding ML](https://medium.com/decodingml/the-llm-twin-free-course-on-production-ready-rag-pipelines-c96472f4e8c8)
- #COURSE [Prompt Engineering with Llama 2 & 3 - DeepLearning.AI](https://www.deeplearning.ai/short-courses/prompt-engineering-with-llama-2/?utm_campaign=meta-launch&utm_medium=featured-card&utm_source=dlai-homepage)
- #COURSE Get into LLMs with roadmaps and colab notebooks
    - [mlabonne/llm-course: Course to get into Large Language Models (LLMs) with roadmaps and Colab notebooks. (github.com)](https://github.com/mlabonne/llm-course?tab=readme-ov-file)
    - [machinelearnear/curso-ia-generativa-y-llms: Un curso para meterse en todo lo que es Generative AI y modelos grandes de lenguaje (LLMs) con roadmaps y notebooks para Colab. (github.com)](https://github.com/machinelearnear/curso-ia-generativa-y-llms)

## Code
- #CODE [openai/tiktoken: tiktoken is a fast BPE tokeniser for use with OpenAI's models. (github.com)](https://github.com/openai/tiktoken)
- #CODE [GitHub - BerriAI/litellm](https://github.com/BerriAI/litellm) - Python SDK, Proxy Server (LLM Gateway) to call 100+ LLM APIs in OpenAI format
	- [LiteLLM - Getting Started | liteLLM](https://docs.litellm.ai/docs/)
- #CODE [Exllamav2](https://github.com/turboderp/exllamav2) - A fast inference library for running LLMs locally on modern consumer-class GPUs
	- [Maxime Labonne - ExLlamaV2: The Fastest Library to Run LLMs](https://mlabonne.github.io/blog/posts/ExLlamaV2_The_Fastest_Library_to_Run%C2%A0LLMs.html)
### Lifecycle and deployment
- #CODE Langsmith [langchain-ai/langsmith-cookbook (github.com)](https://github.com/langchain-ai/langsmith-cookbook)
    - [LangSmith (langchain.com)](https://www.langchain.com/langsmith)
    - [Get started with LangSmith | 🦜️🛠️ LangSmith (langchain.com)](https://docs.smith.langchain.com/)
    - [Evaluate your LLM application | 🦜️🛠️ LangSmith (langchain.com)](https://docs.smith.langchain.com/tutorials/Developers/evaluation)
### Frameworks
- Framework comparisons:
	- [Choosing a RAG Framework: Haystack, LangChain, LlamaIndex (gettingstarted.ai)](https://www.gettingstarted.ai/introduction-to-rag-ai-apps-and-frameworks-haystack-langchain-llamaindex/)
	- [A comparative overview of LangChain, Semantic Kernel, AutoGen and more | by Jane Huang | Data Science at Microsoft | Medium](https://medium.com/data-science-at-microsoft/harnessing-the-power-of-large-language-models-a-comparative-overview-of-langchain-semantic-c21f5c19f93e)
	- [Microsoft Semantic Kernel and AutoGen: Open Source Frameworks for AI Solutions](https://techcommunity.microsoft.com/t5/educator-developer-blog/microsoft-semantic-kernel-and-autogen-open-source-frameworks-for/ba-p/4051305)
- #CODE [huggingface/transformers: 🤗 Transformers: State-of-the-art Machine Learning for Pytorch, TensorFlow, and JAX. (github.com)](https://github.com/huggingface/transformers)
    - [🤗 Transformers (huggingface.co)](https://huggingface.co/docs/transformers/index)
    - Transformers-agents: [License to Call: Introducing Transformers Agents 2.0 (huggingface.co)](https://huggingface.co/blog/agents)
- #CODE [LangChain](https://www.langchain.com/?ref=gettingstarted.ai)
    - [How to build a tool-using agent with LangChain | OpenAI Cookbook](https://cookbook.openai.com/examples/how_to_build_a_tool-using_agent_with_langchain)
    - [Unleashing the Power of LangChain Expression Language (LCEL): from proof of concept to production | by Tom Darmon | Artefact Engineering and Data Science | Jan, 2024 | Medium](https://medium.com/artefact-engineering-and-data-science/unleashing-the-power-of-langchain-expression-language-lcel-from-proof-of-concept-to-production-8ad8eebdcb1d)
    - [Chains | 🦜️🔗 LangChain](https://python.langchain.com/docs/modules/chains/)
    - LangGraph: [langchain-ai/langgraph: Build resilient language agents as graphs. (github.com)](https://github.com/langchain-ai/langgraph)
- #CODE [microsoft/semantic-kernel: Integrate cutting-edge LLM technology quickly and easily into your apps (github.com)](https://github.com/microsoft/semantic-kernel)
    - [Introduction to Semantic Kernel | Microsoft Learn](https://learn.microsoft.com/en-us/semantic-kernel/overview/)
    - [microsoft/SemanticKernelCookBook: This is a Semantic Kernel's book for beginners (github.com)](https://github.com/microsoft/SemanticKernelCookBook?WT.mc_id=academic-120325-leestott)
- #CODE [microsoft/graphrag: A modular graph-based Retrieval-Augmented Generation (RAG) system (github.com)](https://github.com/microsoft/graphrag)
    - [GraphRAG: Unlocking LLM discovery on narrative private data - Microsoft Research](https://www.microsoft.com/en-us/research/blog/graphrag-unlocking-llm-discovery-on-narrative-private-data/)
    - [Introducing GraphRAG with LangChain and Neo4j | by Valentina Alto | Microsoft Azure | Medium](https://medium.com/microsoftazure/introducing-graphrag-with-langchain-and-neo4j-90446df17c1e)
- #CODE [microsoft/autogen: A programming framework for agentic AI. Discord: https://aka.ms/autogen-dc. Roadmap: https://aka.ms/autogen-roadmap (github.com)](https://github.com/microsoft/autogen)
    - [AutoGen | AutoGen (microsoft.github.io)](https://microsoft.github.io/autogen/)
    - [[2308.08155] AutoGen: Enabling Next-Gen LLM Applications via Multi-Agent Conversation (arxiv.org)](https://arxiv.org/abs/2308.08155)
    - [Agent AutoBuild - Automatically Building Multi-agent Systems | AutoGen (microsoft.github.io)](https://microsoft.github.io/autogen/blog/2023/11/26/Agent-AutoBuild/)
    - [vLLM | AutoGen (microsoft.github.io)](https://microsoft.github.io/autogen/docs/topics/non-openai-models/local-vllm/)
- #CODE [microsoft/TaskWeaver: A code-first agent framework for seamlessly planning and executing data analytics tasks. (github.com)](https://github.com/microsoft/TaskWeaver?tab=readme-ov-file)
    - A code-first agent framework for seamlessly planning and executing data analytics tasks (autonomous agent)
    - It translates user requests into executable code and treats user-defined plugins as callable functions. TaskWeaver supports rich data structures, flexible plugin usage, dynamic plugin selection, and harnesses LLM coding capabilities for complex logic. It also incorporates domain-specific knowledge through examples and ensures the secure execution of generated code
    - [[2311.17541] TaskWeaver: A Code-First Agent Framework (arxiv.org)](https://arxiv.org/abs/2311.17541)
    - [The Future of Agent Frameworks: TaskWeaver and Microsoft Autogen and Microsoft Semantic Kernel](https://techcommunity.microsoft.com/t5/ai-azure-ai-services-blog/uncover-the-future-microsoft-autonomous-ai-agents-analyzing-sap/ba-p/4005307)
    - [TaskWeaver beats AutoGen! 🚀 Microsoft's Code-First Agent Framework 🤯 ( LIVE DEMO Full Tutorial ) - YouTube](https://www.youtube.com/watch?v=1CdU4n-Obsw&ab_channel=MervinPraison)
- #CODE [Haystack | Haystack (deepset.ai)](https://haystack.deepset.ai/?ref=gettingstarted.ai)
    - [deepset-ai/haystack: :mag: LLM orchestration framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data. With advanced retrieval methods, it's best suited for building RAG, question answering, semantic search or conversational agent chatbots. (github.com)](https://github.com/deepset-ai/haystack)
    - [What is Haystack? | Haystack (deepset.ai)](https://haystack.deepset.ai/overview/intro)
    - [Haystack: An Alternative to Langchain carrying LLMs | by Amanatullah | 𝐀𝐈 𝐦𝐨𝐧𝐤𝐬.𝐢𝐨 | Medium](https://medium.com/aimonks/haystack-an-alternative-to-langchain-carrying-llms-bf7c515c9a7e)
    - [Customizing Agent to Chat with Your Documents | Haystack (deepset.ai)](https://haystack.deepset.ai/tutorials/25_customizing_agent)
    - [LM Format Enforcer | Haystack (deepset.ai)](https://haystack.deepset.ai/integrations/lmformatenforcer)
    - [Generating Structured Output with Loop-Based Auto-Correction | Haystack (deepset.ai)](https://haystack.deepset.ai/tutorials/28_structured_output_with_loop)
- #CODE [LlamaIndex, Data Framework for LLM Applications](https://www.llamaindex.ai/?ref=gettingstarted.ai)
    - Llama-agents: [run-llama/llama-agents (github.com)](https://github.com/run-llama/llama-agents)
    - Llama-cloud, llama-parse: [Introducing LlamaCloud and LlamaParse — LlamaIndex, Data Framework for LLM Applications](https://www.llamaindex.ai/blog/introducing-llamacloud-and-llamaparse-af8cedf9006b)
- #CODE [stanfordnlp/dspy: DSPy: The framework for programming—not prompting—foundation models (github.com)](https://github.com/stanfordnlp/dspy)
    - [Building an AI Assistant with DSPy | by Lak Lakshmanan | Mar, 2024 | Towards Data Science](https://towardsdatascience.com/building-an-ai-assistant-with-dspy-2e1e749a1a95)
- #CODE [embedchain/embedchain: The Open Source RAG framework (github.com)](https://github.com/embedchain/embedchain)
    - [What is the difference between Embedchain and LangChain (gettingstarted.ai)](https://www.gettingstarted.ai/what-is-the-difference-between-embedchain-and-langchain/)
- #CODE [sgl-project/sglang: SGLang is a structured generation language designed for large language models (LLMs). It makes your interaction with models faster and more controllable. (github.com)](https://github.com/sgl-project/sglang)
- #CODE [lm-sys/FastChat: An open platform for training, serving, and evaluating large language models. Release repo for Vicuna and Chatbot Arena. (github.com)](https://github.com/lm-sys/FastChat)
    - An open platform for training, serving, and evaluating large language models (chatbot arena)

## References
- #PAPER [Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond (2023)](https://arxiv.org/abs/2304.13712)
- #PAPER [Reflexion: an autonomous agent with dynamic memory and self-reflection (2023)](https://arxiv.org/pdf/2303.11366)
	- [Paper explained - GPT 4 Can Improve Itself](https://www.youtube.com/watch?v=5SgJKZLBrmg)
- #PAPER [GSM-Symbolic: Understanding the Limitations of Mathematical Reasoning in  Large Language Models (2024)](https://arxiv.org/pdf/2410.05229)
	- #CODE https://github.com/zhaoolee/garss
	- [Apple drops AI bombshell: LLMs cannot Reason - YouTube](https://www.youtube.com/watch?v=tTG_a0KPJAc)
- #PAPER #REVIEW [Parameter-Efficient Fine-Tuning for Large Models: A Comprehensive Survey (2024)](https://arxiv.org/abs/2403.14608)

### Causality and LLMs
See [[AI/Causality/Causality|Causality]]
- #PAPER [[2305.00050] Causal Reasoning and Large Language Models: Opening a New Frontier for Causality (arxiv.org)](https://arxiv.org/abs/2305.00050)
    - LLM-based methods establish new state-of-the-art accuracies on multiple causal benchmarks
    - [Metaculus Presents — Causal Inference and LLMs: A New Frontier - YouTube](https://www.youtube.com/watch?v=PT1NoaeYwDs&ab_channel=Metaculus)
- #PAPER [[2304.05524] Understanding Causality with Large Language Models: Feasibility and Opportunities (arxiv.org)](https://arxiv.org/abs/2304.05524)
    - LLMs are not yet able to provide satisfactory answers for discovering new knowledge or for high-stakes decision-making tasks with high precision
    - Current LLMs can answer causal questions with existing causal knowledge as combined domain experts
- #PAPER [[2112.03753] Tell me why! Explanations support learning relational and causal structure (arxiv.org)](https://arxiv.org/abs/2112.03753)
    - [google-deepmind/tell_me_why_explanations_rl (github.com)](https://github.com/google-deepmind/tell_me_why_explanations_rl)
- #PAPER [[2305.16183] Passive learning of active causal strategies in agents and language models (arxiv.org)](https://arxiv.org/abs/2305.16183)