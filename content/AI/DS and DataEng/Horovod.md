---
title: "Horovod"
---


## References
- #PAPER [Horovod: fast and easy distributed deep learning in TensorFlow (Sergeev 2018)](http://arxiv.org/abs/1802.05799 )
	- #CODE https://github.com/horovod/horovod 
	- https://horovod.readthedocs.io/en/latest/keras.html 
	- https://horovod.readthedocs.io/en/stable/tensorflow.html
	- https://eng.uber.com/horovod/
	- Horovod is a distributed training framework for TensorFlow, Keras, PyTorch, and MXNet. The goal of Horovod is to make distributed Deep Learning fast and easy to use. Horovod is hosted by the LF AI Foundation (Linux Foundation AI). Horovod implements all-reduce operations into the back-propagation computation to average the computed gradients and allow the distributed scaling among multiple GPUs. Based on Baidu ring allreduce (http://andrew.gibiansky.com/blog/machine-learning/baidu-allreduce/)
	- [Not straightforward from Jupyterlab](https://github.com/horovod/horovod/issues/622. Possible solution - Ipyparallel:)
		- [Interactive Distributed Deep Learning with Jupyter Notebooks](https://sc18.supercomputing.org/proceedings/tech_poster/poster_files/post206s2-file3.pdf)
		- https://github.com/sparticlesteve/cori-intml-examples 

## Examples
- https://github.com/horovod/horovod/tree/master/examples
- https://horovod.readthedocs.io/en/stable/running_include.html
- https://github.com/horovod/tutorials/blob/master/fashion_mnist/README.md 
- [Distributed Deep Learning with Horovod (Jordi Torres)](https://towardsdatascience.com/distributed-deep-learning-with-horovod-2d1eea004cb2)
- https://towardsdatascience.com/a-quick-guide-to-distributed-training-with-tensorflow-and-horovod-on-amazon-sagemaker-dae18371ef6e 
- [with SLURM on the BSC-P9 cluster](https://towardsdatascience.com/distributed-deep-learning-with-horovod-2d1eea004cb2)
- With SLURM workload manager. See paper Ramirez-Gargallo 2019 in [[AI/DS and DataEng/Distributed DL]]
- [Example with SLURM](http://www.idris.fr/eng/jean-zay/gpu/jean-zay-gpu-hvd-tf-multi-eng.html)

