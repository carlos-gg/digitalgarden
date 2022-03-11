---
title: "Reinforcement learning"
disableToc: false 
---

## Resources
- Reinforcement learning is the task of learning what actions to take, given a certain situation/environment, so as to maximize a reward signal. The interesting difference between supervised and reinforcement learning is that this reward signal simply tells you whether the action (or input) that the agent takes is good or bad. It doesn’t tell you anything about what the best action is. Contrast this to CNNs where the corresponding label for each image input is a definite instruction of what the output should be for each input.  Another unique component of RL is that an agent’s actions will affect the subsequent data it receives. For example, an agent’s action of moving left instead of right means that the agent will receive different input from the environment at the next time step.
- https://en.wikipedia.org/wiki/Reinforcement_learning
- [Curriculum for Reinforcement Learning](https://lilianweng.github.io/lil-log/2020/01/29/curriculum-for-reinforcement-learning.html)
- [Andrej Karpathy's introduction to RL](http://karpathy.github.io/2016/05/31/rl/)
- [Evolution strategies vs RL](https://blog.openai.com/evolution-strategies/)
	- https://github.com/openai/evolution-strategies-starter
- [Reinforcement learning derivations (math)](http://www.alexirpan.com/rl-derivations/)
- [Introduction to various RL algos](https://towardsdatascience.com/introduction-to-various-reinforcement-learning-algorithms-i-q-learning-sarsa-dqn-ddpg-72a5e0cb6287)
- [Q-learning](https://en.wikipedia.org/wiki/Q-learning)
- Temporal differencing (TD) learning  is a prediction-based machine learning method. 
	- It has primarily been used for the reinforcement learning problem, and is said to be "a combination ofMonte Carlo ideas and dynamic programming (DP) ideas." 
	- TD resembles a Monte Carlo method because it learns by sampling the environment according to some policy, and is related to dynamic programming techniques as it approximates its current estimate based on previously learned estimates (a process known as bootstrapping). The TD learning algorithm is related to the temporal difference model of animal learning. As a prediction method, TD learning considers that subsequent predictions are often correlated in some sense.
	- TD-Lambda: This algorithm was famously applied by Gerald Tesauro to createTD-Gammon, a program that learned to play the game of backgammon at the level of expert human players. The lambda parameter refers to the trace decay parameter, with 0<= lambda <=1. Higher settings lead to longer lasting traces; that is, a larger proportion of credit from a reward can be given to more distant states and actions when lambda is higher, with lambda=1 producing parallel learning to Monte Carlo RL algorithms.
- [SARSA](https://en.wikipedia.org/wiki/State%E2%80%93action%E2%80%93reward%E2%80%93state%E2%80%93action)


## Courses, talks and books
- #COURSE [Reinforcement Learning (UCL)](https://www.davidsilver.uk/teaching/)
	- [Videos](https://www.youtube.com/watch?v=2pWv7GOvuf0&list=PLzuuYNsE1EZAXYR4FJ75jcJseBmo4KQ9-)
- #COURSE [CS294-112 Deep Reinforcement Learning Sp17](https://www.youtube.com/playlist?list=PLkFD6_40KJIwTmSbCv9OVJB3YaO4sFwkX)
- #COURSE [Practical Reinforcement Learning (Yandex)](https://github.com/yandexdataschool/Practical_RL)
- #COURSE [Tutorial: Introduction to Reinforcement Learning](https://colab.research.google.com/github/NeuromatchAcademy/course-content-dl/blob/main/tutorials/W3D2_BasicReinforcementLearning/student/W3D2_Tutorial1.ipynb)
- #TALK [Deep Learning and Reinforcement Learning Summer School, Toronto 2018](http://videolectures.net/DLRLsummerschool2018_toronto/)
- #TALK [Deep RL Bootcamp](https://sites.google.com/view/deep-rl-bootcamp/lectures	  )
- #BOOK [Deep Reinforcement Learning (2020 SPRINGER)](https://www.springer.com/gp/book/9789811540943)
	- https://deepreinforcementlearningbook.org/


## Code
- #CODE [Acme: a research framework for reinforcement learning](https://github.com/deepmind/acme)
- #CODE [Deep Reinforcement Learning Model ZOO](https://github.com/tensorlayer/tensorlayer/tree/master/examples/reinforcement_learning)
- #CODE [Open.ai Gym - A toolkit for developing and comparing reinforcement learning algorithms](https://github.com/openai/gym)
	- https://gym.openai.com/
	- #PAPER http://arxiv.org/abs/1606.01540
- #CODE [Horizon (Facebook) - The first open source reinforcement learning platform for large-scale products and services](https://github.com/facebookresearch/Horizon)
- #CODE [Keras-rl - Deep Reinforcement Learning for Keras](https://github.com/keras-rl/keras-rl)
- #CODE [TRFL (pronounced "truffle") is a library built on top of TensorFlow that exposes several useful building blocks for implementing Reinforcement Learning agents](https://github.com/deepmind/trfl/)
- #CODE [Surreal - Open-Source Distributed Reinforcement Learning Framework by Stanford Vision and Learning Lab](https://github.com/SurrealAI/surreal)
	- https://surreal.stanford.edu
- #CODE Tensorforce - Tensorforce is an open-source deep reinforcement learning framework, with an emphasis on modularized flexible library design and straightforward usability for applications in research and practice. 
	- https://github.com/tensorforce/tensorforce
	- https://reinforce.io/blog/introduction-to-tensorforce/
- #CODE [Tensorlayer](https://github.com/tensorlayer/tensorlayer)
	- Deep Learning and Reinforcement Learning Library for Scientists and Engineers
	- https://tensorlayer.readthedocs.io/en/latest/index.html


## References
### Deep RL
- [Spinning Up as a Deep RL Researcher](https://spinningup.openai.com/en/latest/spinningup/spinningup.html)

Review papers:
- #PAPER [A Brief Survey of Deep Reinforcement Learning (Arulkumaran 2017)](https://arxiv.org/abs/1708.05866)
	- Many of the successes in DRL have been based on scaling up prior work in RL to high-dimensional problems. This is due to the learning of low-dimensional feature representations and the powerful function approximation properties of neural networks. By means of representation learning, DRL can deal efficiently with the curse of dimensionality, unlike tabular and traditional non-parametric methods.
	- https://adeshpande3.github.io/adeshpande3.github.io/Deep-Learning-Research-Review-Week-2-Reinforcement-Learning
- #PAPER [An Introduction to Deep Reinforcement Learning (Fancois-Lavet 2018)](https://arxiv.org/abs/1811.12560)
- #PAPER [Offline Reinforcement Learning: Tutorial, Review, and Perspectives on Open Problems (Levine 2020)](https://arxiv.org/abs/2005.01643)

- #PAPER [DQN: Human-level control through Deep Reinforcement Learning (Mnih 2015)](https://deepmind.com/research/dqn/)
	- https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf
- #PAPER [Learning to Optimize (Li 2016)](https://arxiv.org/abs/1606.01885)
	- [Learning to Optimize with Reinforcement Learning](https://bair.berkeley.edu/blog/2017/09/12/learning-to-optimize-with-rl/)
- #PAPER [Deep Recurrent Q-Learning for Partially Observable MDPs (Hausknecht 2017)](https://arxiv.org/abs/1507.06527)
- #PAPER [Neural Episodic Control (Pritzel 2017)](https://arxiv.org/abs/1703.01988)
	- Deep reinforcement learning methods attain super-human performance in a wide range of environments. Such methods are grossly inefficient, often taking orders of magnitudes more data than humans to achieve reasonable performance
	- Neural Episodic Control: a deep reinforcement learning agent that is able to rapidly assimilate new experiences and act upon them. 
	- The agent uses a semi-tabular representation of the value function: a buffer of past experience containing slowly changing state representations and rapidly updated estimates of the value function
	- https://www.technologyreview.es/s/6656/olvidese-del-aprendizaje-profundo-el-nuevo-enfoque-de-google-funciona-mucho-mejor
	- [Explanation of Neural Episodic Control](https://rylanschaeffer.github.io/content/research/neural_episodic_control/main.html)
- #PAPER [Supervising strong learners by amplifying weak experts (Christiano 2018)](https://arxiv.org/abs/1810.08575)
	- [Learning Complex Goals with Iterated Amplification](https://blog.openai.com/amplifying-ai-training/)
- #PAPER [MuZero - Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model (Schrittwieser 2019)](https://deepmind.com/research/publications/MasterinModel)
	- https://medium.com/dataseries/deepminds-muzero-is-one-of-the-most-important-deep-learning-systems-ever-created-347442a6793g-Atari-Go-Chess-and-Shogi-by-Planning-with-a-Learned-
- #PAPER [Decision Transformer: Reinforcement Learning via Sequence Modeling (Chen 2021)](https://arxiv.org/abs/2106.01345v1) ^decisiontransformer
	- #CODE https://paperswithcode.com/paper/decision-transformer-reinforcement-learning
	- [Paper explained](https://www.youtube.com/watch?v=-buULmf7dec)
- #PAPER [Reward is enough (Silver 2021)](https://www.sciencedirect.com/science/article/pii/S0004370221000862)
	- https://towardsdatascience.com/reward-is-enough-ml-paper-review-e448ee0a6092
	- From the authors of “Attention is all you need”, this paper proposes an intriguing hypothesis that incentivizing AI agents with reward is enough to achieve General Artificial Intelligence
	- "General intelligence, of the sort possessed by humans and perhaps also other animals, may be defined as the ability to flexibly achieve a variety of goals in different contexts. According to our hypothesis, general intelligence can instead be understood as, and implemented by, maximising a singular reward in a single, complex environment4"