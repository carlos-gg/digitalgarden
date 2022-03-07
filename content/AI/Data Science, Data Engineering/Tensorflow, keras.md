---
title: "Tensorflow, Keras"
disableToc: false 
---

# Code
- #CODE Tensorflow (Google): https://github.com/tensorflow/tensorflow
	- http://playground.tensorflow.org/
	- https://cloud.google.com/blog/big-data/2016/07/understanding-neural-networks-with-tensorflow-playground
	- https://blog.metaflow.fr/tensorflow-how-to-freeze-a-model-and-serve-it-with-a-python-api-d4f3596b3adc#.dg41ldof5
	- https://codelabs.developers.google.com/codelabs/cloud-tensorflow-mnist/#0
	- Tensorflow 2.0: models migration and new design: https://pgaleone.eu/tensorflow/gan/2018/11/04/tensorflow-2-models-migration-and-new-design/
	- http://planspace.org/20170404-how_not_to_program_the_tensorflow_graph/
- #CODE TF Similarity: https://github.com/tensorflow/similarity
	- https://blog.tensorflow.org/2021/09/introducing-tensorflow-similarity.html
	- Metric learning is different from traditional classification as it's objective is different. The model learns to minimize the distance between similar examples and maximize the distance between dissimilar examples, in a supervised or self-supervised fashion
- #CODE TF Probability: https://github.com/tensorflow/probability
	- Probabilistic reasoning and statistical analysis in TensorFlow
	- https://www.tensorflow.org/probability
- #CODE TF Decision Forests: https://github.com/tensorflow/decision-forests
	- A collection of state-of-the-art algorithms for the training, serving and interpretation of Decision Forest models in Keras
	- https://blog.tensorflow.org/2021/05/introducing-tensorflow-decision-forests.html
	- https://towardsdatascience.com/tensorflow-decision-forests-train-your-favorite-tree-based-models-using-keras-875d05a441f
	- Decision forests in TF: https://www.youtube.com/watch?v=5qgk9QJ4rdQ
- #CODE TF Datasets: https://github.com/tensorflow/datasets
- #CODE TF Agents: https://github.com/tensorflow/agents
	- A reliable, scalable and easy to use TensorFlow library for Contextual Bandits and Reinforcement Learning
- #CODE TF Recommenders: https://github.com/tensorflow/recommenders 
	- Library for building recommender system models using TensorFlow.
- #CODE TF Graphics: https://github.com/tensorflow/graphics
	- Differentiable Graphics Layers for TensorFlow
- #CODE TF Ranking: https://github.com/tensorflow/ranking
	- Learning to Rank in TensorFlow
- #CODE Tensorboard: https://github.com/tensorflow/tensorboard
	- https://tensorboard.dev/
	- https://www.tensorflow.org/tensorboard/get_started (use as a jupyterlab magic)
- #CODE Tensorflow.js: https://www.tensorflow.org/js/
- #CODE TF On Spark: https://github.com/yahoo/TensorFlowOnSpark
- #CODE Sonnet: https://github.com/deepmind/sonnet
	- https://deepmind.com/blog/open-sourcing-sonnet/
- #CODE seq2seq: https://github.com/google/seq2seq
- #CODE Tensor2Tensor: https://github.com/tensorflow/tensor2tensor
	- https://research.googleblog.com/2017/06/accelerating-deep-learning-research.html
- #CODE Graph Nets - Build Graph Nets in Tensorflow: https://github.com/deepmind/graph_nets
	- https://arxiv.org/abs/1806.01261
- TF Graph Visualizer: http://idl.cs.washington.edu/papers/tfgraph/
- #CODE Tensorpack - It's Yet Another TF high-level API, with speed, and flexibility built together. https://github.com/tensorpack/tensorpack
- #CODE Cleverhans - A library for benchmarking vulnerability to adversarial examples: https://github.com/tensorflow/cleverhans
	- http://karpathy.github.io/2015/03/30/breaking-convnets/
	- https://blog.openai.com/adversarial-example-research/


# Keras
- #CODE Keras: https://github.com/keras-team/keras 
	- Keras is a deep learning API written in Python, running on top of the machine learning platform Tensorflow
	- http://keras.io/
	- https://keras.io/getting_started/intro_to_keras_for_researchers/
	- Modern Keras design patterns: https://www.youtube.com/watch?v=FCz9m4T0DI0
- #CODE AutoKeras - Auto-Keras is an open source software library for automated machine learning (AutoML): https://github.com/keras-team/autokeras
	- http://autokeras.com/
	- #PAPER Auto-Keras: An Efficient Neural Architecture Search System (Jin 2019): https://arxiv.org/abs/1806.10282
	- https://towardsdatascience.com/autokeras-the-killer-of-googles-automl-9e84c552a319


# Distributed training
- https://missinglink.ai/guides/tensorflow/tensorflow-distributed-training-introduction-tutorials/ 
- TF.Distribute
	- https://www.tensorflow.org/guide/distributed_training 
	- https://www.tensorflow.org/guide/gpu
	- https://keras.io/guides/distributed_training/
	- #TALK Inside TensorFlow: tf.data + tf.distribute: https://www.youtube.com/watch?v=ZnukSLKEw34
- Numpy to tf.record: https://gist.github.com/swyoon/8185b3dcf08ec728fb22b99016dd533f
- https://www.tensorflow.org/tutorials/distribute/keras 
- https://www.tensorflow.org/tutorials/distribute/custom_training 
- https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/tutorials/distribute/custom_training.ipynb#scrollTo=9iagoTBfijUz 
- Train a Neural Network on multi-GPU with TensorFlow (Jordi Torres): https://towardsdatascience.com/train-a-neural-network-on-multi-gpu-with-tensorflow-42fa5f51b8af
- Multinode example: https://github.com/tensorflow/examples/blob/master/community/en/docs/deploy/distributed.md
- MultiWorkerMirroredStrategy:
	- https://www.tensorflow.org/api_docs/python/tf/distribute/MultiWorkerMirroredStrategy (after TF v2)
	- https://www.tensorflow.org/api_docs/python/tf/distribute/experimental/MultiWorkerMirroredStrategy
	- https://blog.tensorflow.org/2020/12/whats-new-in-tensorflow-24.html (TF v2.4)
	- https://www.tensorflow.org/tutorials/distribute/multi_worker_with_keras 
	- https://github.com/tensorflow/tensorflow/issues/36094
- https://www.tensorflow.org/api_docs/python/tf/distribute/cluster_resolver/SlurmClusterResolver 
- https://lambdalabs.com/blog/tensorflow-2-0-tutorial-05-distributed-training-multi-node/ 

Data lazy loading: 
- Tf.data:
	- https://www.tensorflow.org/api_docs/python/tf/data/Dataset 
	- https://www.tensorflow.org/api_docs/python/tf/data/Dataset#from_generator
	- https://www.tensorflow.org/tutorials/distribute/input
- Tensorflow data netcdf, MATEX tensorflow (seems to be abandoned) :https://github.com/matex-org/matex/wiki/DataSet-Reader 
