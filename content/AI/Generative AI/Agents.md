---
title: Agents
---

> See: 
> - [[AI/Generative AI/Foundation models]] 
> - [[AI/Deep learning/Multimodal learning]] 

## Resources
- [ChatGPT’s next level is Agent AI: Auto-GPT, BabyAGI, AgentGPT, Microsoft Jarvis & friends](https://medium.com/the-generator/chatgpts-next-level-is-agent-ai-auto-gpt-babyagi-agentgpt-microsoft-jarvis-friends-d354aa18f21)
- [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT) - An experimental open-source attempt to make GPT-4 fully autonomous
	- https://significant-gravitas.github.io/Auto-GPT/
	- https://autogpt.net/
- [AgentGPT](https://agentgpt.reworkd.ai/es)
- [BabyAGI](https://babyagi.org/)
- [JARVIS / HuggingGPT](https://github.com/microsoft/JARVIS)
- [Agents in AutoGen | AutoGen (microsoft.github.io)](https://microsoft.github.io/autogen/blog/2024/05/24/Agent/)
    - Agent - an entity that can act on behalf of human intent
    - we can incorporate both very simple agents that can solve simple tasks with a single backend, but also we can have agents that are composed of multiple simpler agents
    - When we use the word 'multi-agent' and 'single-agent', I think there are at least two different dimensions:
        - Interface
            - From the user's point of view, do they interact with the system in a single interaction point or do they see explicitly multiple agents working and need to interact with multiple of them?
            - A single interaction point can make many applications' user experience more straightforward
        - Architecture
            - Are there multiple agents underneath running at the backend?
            - The multi-agent design of the architecture is easier to maintain, understand and extend than a single agent system
            - It's very important to recognize that the multi-agent architecture is a good way to build a single agent
    - A particular system can have a single-agent interface and a multi-agent architecture
    - Ways of combining models and agents:
        - Different conversation patterns or chats: sequential, group, constrained group, customized group, nested
        - Different prompting and reasoning techniques such as reflection, ReAct
        - Tool use and code execution
        - Planning and task decomposition
        - Retrieve augmentation
        - Integrating multiple models, APIs, modalities and memories
- Stateflow - enhancing LLM task-solving through state-driven workflows
    - #PAPER [StateFlow: Enhancing LLM Task-Solving through State-Driven Workflows](https://arxiv.org/abs/2403.11322)
    - [yiranwu0/StateFlow](https://github.com/yiranwu0/StateFlow)
    - [StateFlow - Build State-Driven Workflows with Customized Speaker Selection in GroupChat | AutoGen](https://microsoft.github.io/autogen/0.2/blog/2024/02/29/StateFlow/)
    - [Customize Speaker Selection | AutoGen](https://microsoft.github.io/autogen/0.2/docs/topics/groupchat/customized_speaker_selection/)
    - [FSM - User can input speaker transition constraints | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_groupchat_finite_state_machine/)
    - [StateFlow: Build Workflows through State-Oriented Actions | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_groupchat_stateflow/)
- [EcoAssistant - Using LLM Assistants More Accurately and Affordably | AutoGen (microsoft.github.io)](https://microsoft.github.io/autogen/blog/2023/11/09/EcoAssistant/)
    - Built on top of Autogen
    - #PAPER [EcoAssistant: Using LLM Assistant More Affordably and Accurately (arxiv.org)](https://arxiv.org/abs/2310.03046)
    - [JieyuZ2/EcoAssistant: EcoAssistant: using LLM assistant more affordably and accurately (github.com)](https://github.com/JieyuZ2/EcoAssistant)
- [Agent for text-to-SQL with automatic error correction - Hugging Face Open-Source AI Cookbook](https://huggingface.co/learn/cookbook/agent_text_to_sql?utm_source=pocket_shared)
    - Agent for text-to-SQL with automatic error correction
    - Uses ReactCodeAgent in transformers.agents
- [Natural Language Queries Across Databases with LLMs, AutoGen, and Langchain (PostgreSQL) | by Manojpn | Medium](https://medium.com/@manojpn/natural-language-queries-across-databases-with-llms-autogen-and-langchain-postgresql-5bab04684361)
    - Autogen for SQL queries
- [Step by Step guide to develop AI Multi-Agent system using Microsoft Semantic Kernel and GPT-4o | by Akshay Kokane | Jun, 2024 | Medium](https://medium.com/@akshaykokane09/step-by-step-guide-to-develop-ai-multi-agent-system-using-microsoft-semantic-kernel-and-gpt-4o-f5991af40ea6)
    - Multi-agent system with semantic kernel and openai assistant. Using .NET
- [https://numbersstation.ai/text-to-sql-that-isnt/](https://numbersstation.ai/text-to-sql-that-isnt/)
    - [https://www.youtube.com/watch?v=xmzda44hUgk](https://www.youtube.com/watch?v=xmzda44hUgk)
- [Agent for text-to-SQL with automatic error correction - Hugging Face Open-Source AI Cookbook](https://huggingface.co/learn/cookbook/agent_text_to_sql?utm_source=pocket_shared)
- [Natural Language Queries Across Databases with LLMs, AutoGen, and Langchain (PostgreSQL) | by Manojpn | Medium](https://medium.com/@manojpn/natural-language-queries-across-databases-with-llms-autogen-and-langchain-postgresql-5bab04684361)

## Courses
- #COURSE [AI Agentic Design Patterns with AutoGen](https://www.deeplearning.ai/short-courses/ai-agentic-design-patterns-with-autogen/)
	- https://github.com/ksm26/AI-Agentic-Design-Patterns-with-AutoGen?tab=readme-ov-file
- #COURSE [DLAI - AI Agentic Design Patterns with AutoGen (deeplearning.ai)](https://learn.deeplearning.ai/courses/ai-agentic-design-patterns-with-autogen/lesson/1/introduction)
    - [GitHub - ksm26/AI-Agentic-Design-Patterns-with-AutoGen: Learn to build and customize multi-agent systems using the AutoGen. The course teaches you to implement complex AI applications through agent collaboration and advanced design patterns.](https://github.com/ksm26/AI-Agentic-Design-Patterns-with-AutoGen/tree/main)
- #COURSE [AI Agents in LangGraph - DeepLearning.AI](https://www.deeplearning.ai/short-courses/ai-agents-in-langgraph/)
- #COURSE [Multi AI Agent Systems with crewAI - DeepLearning.AI](https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/)

## Code
- #CODE Autogen
    - [GitHub - autogen-ai/autogen: A programming framework for agentic AI. Discord: https://discord.gg/pAbnFJrkgZ](https://github.com/autogen-ai/autogen)
    - [GitHub - microsoft/autogen: A programming framework for agentic AI 🤖](https://github.com/microsoft/autogen)
    - [Resuming a GroupChat | AutoGen](https://microsoft.github.io/autogen/0.2/docs/topics/groupchat/resuming_groupchat/)
    - [Group Chat with Coder and Visualization Critic | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_groupchat_vis/)
    - [https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_logging](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_logging)
    - [FSM Group Chat -- User-specified agent transitions | AutoGen](https://microsoft.github.io/autogen/0.2/blog/2024/02/11/FSM-GroupChat/)
    - [FSM - User can input speaker transition constraints | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_groupchat_finite_state_machine/)
    - [agentchat_groupchat_customized.ipynb - Colab](https://colab.research.google.com/github/autogen-ai/autogen/blob/main/notebook/agentchat_groupchat_customized.ipynb#scrollTo=PbnYdSWYC8jx)
    - [Group Chat with Retrieval Augmented Generation | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_groupchat_RAG/)
    - Chatbots:
        - [Creating a Streamlit User Interface for AutoGen Agents | by Dr. Ernesto Lee | Medium](https://drlee.io/creating-a-streamlit-user-interface-for-autogen-agents-e053649c74d0)
        - [How to Create APIs for AutoGen - by Yeyu Huang - Lab For AI](https://yeyu.substack.com/p/how-to-create-apis-for-autogen)
        - [How to Create APIs for AutoGen](https://www.youtube.com/watch?v=4mO2TmDervU&ab_channel=YeyuLab)
        - [Integrating AutoGen Agents into Your Web Application (FastApi + Websockets + Queues)](https://newsletter.victordibia.com/p/integrating-autogen-agents-into-your)
- #CODE [AgentOps](https://app.agentops.ai/)
    - [Agent Tracking with AgentOps | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_agentops/)
    - [AgentOps, the Best Tool for AutoGen Agent Observability | AutoGen](https://autogenhub.github.io/autogen/blog/2024/07/25/AgentOps/)
- #CODE Letta (MemGPT)
    - [cpacker/MemGPT: Letta (fka MemGPT) is a framework for creating stateful LLM services.](https://github.com/cpacker/MemGPT)
    - [MemGPT](https://memgpt.ai/)
    - [MemGPT + AutoGen](https://memgpt.readme.io/docs/autogen)
- #CODE Mem0
    - [mem0ai/mem0: The Memory layer for your AI apps](https://github.com/mem0ai/mem0)
    - [Agent with memory using Mem0 | AutoGen](https://microsoft.github.io/autogen/0.2/docs/notebooks/agentchat_memory_using_mem0/)
    - [Mem0: Long-Term Memory and Personalization for Agents | AutoGen](https://autogenhub.github.io/autogen/docs/ecosystem/mem0/)
- #CODE [GitHub - crewAIInc/crewAI: Framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks.](https://github.com/crewAIInc/crewAI)
	- [CrewAI](https://www.crewai.com/open-source?utm_source=pocket_shared)
- #CODE [LangGraph](https://www.langchain.com/langgraph)

## References
- #PAPER  [HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in HuggingFace (Shen 2023)](https://arxiv.org/pdf/2303.17580)
- #PAPER [MLE-bench: Evaluating Machine Learning Agents on Machine Learning  Engineering](https://arxiv.org/pdf/2410.07095)
	- #CODE https://github.com/openai/mle-bench
	- MLE-bench is a benchmark for measuring how well AI agents perform at machine learning engineering
- #PAPER [MLAgentBench: Evaluating Language Agents on Machine Learning Experimentation](https://arxiv.org/pdf/2310.03302)
	- #CODE [GitHub - snap-stanford/MLAgentBench](https://github.com/snap-stanford/mlagentbench)
- #WHITEPAPER [AIDE: Human-Level Performance in Data Science Competitions](https://www.weco.ai/blog/technical-report)
	- #CODE https://github.com/WecoAI/aideml
- #PAPER [OpenHands: An Open Platform for AI Software Developers as Generalist  Agents](https://arxiv.org/pdf/2407.16741)
	- #CODE https://github.com/opendevin/opendevin


