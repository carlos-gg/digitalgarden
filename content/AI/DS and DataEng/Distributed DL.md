---
title: "Distributed Deep learning"
---

## Resources
- https://d2l.ai/chapter_computational-performance/multiple-gpus.html 
- https://jhui.github.io/2017/03/07/TensorFlow-GPU/ 
- https://www.logicalclocks.com/blog/goodbye-horovod-hello-collectiveallreduce 
- [Twelve ways to fool the masses when reporting performance of deep learning workloads](https://htor.inf.ethz.ch/blog/index.php/2018/11/08/twelve-ways-to-fool-the-masses-when-reporting-performance-of-deep-learning-workloads/)
- [Distributed Deep Learning 101: Introduction](https://towardsdatascience.com/distributed-deep-learning-101-introduction-ebfc1bcd59d9)

## Talks
- #TALK [ALCF Datascience frameworks: Tensorflow, PyTorch, Keras, and Horovod](https://www.alcf.anl.gov/files/Zheng_SDL_ML_Frameworks_1.pdf)
- #TALK [Scaling Deep Learning for Scientific Workloads on the #1 Summit Supercomputer](https://insidehpc.com/2019/04/scaling-deep-learning-for-scientific-workloads-on-the-1-summit-supercomputer/)
- #TALK [Scaling Neural Networks Training - Thorsten Kurth](https://www.youtube.com/watch?v=cRjiwIi_kuc)

## Code
See [[AI/DS and DataEng/Tensorflow, keras#Distributed training]]

- #CODE [Analytics Zoo](https://github.com/intel-analytics/analytics-zoo)
	- Distributed Tensorflow, Keras and PyTorch on Apache Spark/Flink & Ray
	- https://analytics-zoo.readthedocs.io/en/latest/index.html
- #CODE [Horovod](AI/DS%20and%20DataEng/Horovod.md)
- #CODE [Colossal-AI: A Unified Deep Learning System for Large-Scale Parallel Training](https://github.com/hpcaitech/colossalai)
	- See [[#^colossalai]]
	-  https://www.marktechpost.com/2021/10/31/researchers-introduce-colossal-ai-a-pytorch-based-deep-learning-system-for-large-scale-parallel-training/

## References
- #PAPER [Evaluation of Deep Learning Frameworks over Different HPC Architectures (Shams 2017)](https://www.ibm.com/university/power/images/EvaluationofDeepLearningFrameworksoverDifferentHPCArchitectures.pdf)
- #PAPER [Deep Learning at 15PF: Supervised and Semi-Supervised Classification for Scientific Data (Kurth 2017)](https://arxiv.org/abs/1708.05256)
- #PAPER [Demystifying Parallel and Distributed Deep Learning: An In-Depth Concurrency Analysis (Tal Ben-Nun and Torsten Hoefler 2018)](http://arxiv.org/abs/1802.09941) ^bennun18
	- #TALK [Hoefler 2018](https://www.youtube.com/watch?v=xtxxLWZznBI)
	- #TALK [Hoefler 2020](https://www.youtube.com/watch?v=uNzQ1vvJ82c)
	- #TALK [Ben-Nun 2020](https://www.youtube.com/watch?v=N5uIFSVR7jE)
- #PAPER [Mesh-TensorFlow: Deep Learning for Supercomputers (Shazeer 2018)](https://arxiv.org/abs/1811.02084v1) ^f86598
	- #TALK https://www.youtube.com/watch?v=HgGyWS40g-g
	- #CODE [Mesh-TensorFlow](https://github.com/tensorflow/mesh)
		- Go beyond data-parallel training
		- More sophisticated parallel computations (big models that do not fit on one device)
- #PAPER [GPipe: Efficient Training of Giant Neural Networks using Pipeline Parallelism (Huang 2019)](http://arxiv.org/abs/1811.06965)
- #PAPER [A Quantitative Study of Deep Learning Training on Heterogeneous Supercomputers (Han 2019)](https://ieeexplore.ieee.org/document/8890993)
	- http://people.cs.vt.edu/~butta/docs/cluster2019-DL.pdf
- #PAPER [Channel and filter parallelism for large-scale CNN training (Dryden 2019)](https://dl.acm.org/doi/10.1145/3295500.3356207)
	- https://ndryden.com/data/papers/sc2019-chanfilt.pdf
- #PAPER [Improving Strong-Scaling of CNN Training by Exploiting Finer-Grained Parallelism (Dryden 2019)](http://arxiv.org/abs/1903.06681)
- #PAPER [Pipe-SGD: A Decentralized Pipelined SGD Framework for Distributed Deep Net Training (Li 2019)](http://arxiv.org/abs/1811.03619)
- #PAPER [Scalable Deep Learning on Distributed Infrastructures: Challenges, Techniques and Tools (Mayer 2019)](http://arxiv.org/abs/1903.11314)
- #PAPER [Performance Analysis of Deep Learning Workloads on Leading-edge Systems (Ren 2019)](https://www.osti.gov/biblio/1571428-performance-analysis-deep-learning-workloads-leading-edge-systems)
- #PAPER [TensorFlow on State-of-the-Art HPC Clusters: A Machine Learning use Case (Ramirez-Gargallo 2019)](https://ieeexplore.ieee.org/document/8752892) ^ramirez19
	- https://core.ac.uk/download/pdf/196280993.pdf 
	- Compared MN4, Power9 and Dibona HPC clusters. Only CPUs compared (Power9 GPUs are not evaluated)
- #PAPER [Exascale Deep Learning for Scientific Inverse Problems (Laanait 2019)](http://arxiv.org/abs/1909.11150)
- #PAPER [TensorFlow Doing HPC (Chien 2019)](https://arxiv.org/abs/1903.04364)
- #PAPER [ZeRO: memory optimizations toward training trillion parameter models (Rajbhandari 2019)](https://arxiv.org/abs/1910.02054)
	- #CODE [DeepSpeed](https://github.com/microsoft/DeepSpeed)
		- DeepSpeed is a deep learning optimization library that makes distributed training easy, efficient, and effective. For pytorch
		- www.deepspeed.ai/
	- https://www.microsoft.com/en-us/research/blog/zero-deepspeed-new-system-optimizations-enable-training-models-with-over-100-billion-parameters/
- #PAPER [Towards a Scalable and Distributed Infrastructure for Deep Learning Applications (Hasheminezhad 2020)](https://arxiv.org/abs/2010.03012)
	- Phylanx Deep Learning Framework
	- Good comparison with respect to SOTA
	- [Phylanx provides a high-productivity debugable Python-based interactive interface, JetLag](https://github.com/STEllAR-GROUP/JetLag)
	- Tests only on CPU. Does it support GPUs?
- #PAPER [Distributed Training of Deep Learning Models: A Taxonomic Perspective (Langer 2020)](https://arxiv.org/abs/2007.03970)
- #PAPER [Colossal-AI: A Unified Deep Learning System For Large-Scale Parallel Training (Bian 2021)](https://arxiv.org/abs/2110.14883) 
- #PAPER [Pathways: Asynchronous Distributed Dataflow for ML (Barham 2022)](https://arxiv.org/pdf/2203.12533)            
- #PAPER [Scaling Laws vs Model Architectures: How does Inductive Bias Influence  Scaling? (Tay 2022)](https://arxiv.org/pdf/2207.10551v1)
