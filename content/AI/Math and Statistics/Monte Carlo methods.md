---
title: "Monte Carlo methods"
disableToc: false 
---


## Resources
- https://en.wikipedia.org/wiki/Monte_Carlo_method

### Sequential Monte Carlo (SMC or particle filter)
- Particle filters or Sequential Monte Carlo (SMC) methods are a set of Monte Carlo algorithms used to solve filtering problems arising in signal processing and Bayesian statistical inference. The filtering problem consists of estimating the internal states in dynamical systems when partial observations are made, and random perturbations are present in the sensors as well as in the dynamical system. The objective is to compute the posterior distributions of the states of some Markov process, given some noisy and partial observations.

### Markov Process
- https://en.wikipedia.org/wiki/Markov_chain
- https://en.wikipedia.org/wiki/Markov_property
- A stochastic process has the Markov property if the conditional probability distribution of future states of the process (conditional on both past and present states) depends only upon the present state, not on the sequence of events that preceded it. A process with this property is called a Markov process.
- [Markov Chains Explained Visually](http://setosa.io/ev/markov-chains/)

#### Hidden Markov Model (HMM)
- https://en.wikipedia.org/wiki/Hidden_Markov_model
- Hidden Markov Model (HMM) is a statistical Markov model in which the system being modeled is assumed to be a Markov process with unobserved (i.e. hidden) states.
- HMM is a Markov chain for which the state is only partially observable. In other words, observations are related to the state of the system, but they are typically insufficient to precisely determine the state. Several well-known algorithms for hidden Markov models exist. 
- https://www.quora.com/What-is-a-hidden-Markov-Model-HMM-and-how-can-it-be-used-in-speech-recognition
- https://www.quora.com/Why-do-we-use-Hidden-Markov-Models-for-speech-recognition
- http://scikit-learn.sourceforge.net/stable/modules/hmm.html
- https://github.com/hmmlearn/hmmlearn
- http://hmmlearn.readthedocs.io/en/latest/tutorial.html#available-models

### MCMC
- MCMC methods comprise a class of algorithms for sampling from a probability distribution. By constructing a Markov chain that has the desired distribution as its equilibrium distribution, one can obtain a sample of the desired distribution by recording states from the chain
- https://en.wikipedia.org/wiki/Markov_chain_Monte_Carlo

### Nested Sampling
- https://en.wikipedia.org/wiki/Nested_sampling_algorithm
- The nested sampling algorithm is a computational approach to the problem of comparing models in Bayesian statistics. 


## Code
- [A list of Python-based MCMC packages. Also here’s a nice list of MCMC algorithms](https://gabriel-p.github.io/pythonMCMC/)
- #CODE [Sampyl - MCMC samplers for Bayesian estimation in Python, including Metropolis-Hastings, NUTS, and Slice](http://mcleonard.github.io/sampyl/)
- #CODE [emcee](http://dan.iel.fm/emcee/current/)
- #CODE UltraNest - A Pythonic implementation of the Nested Sampling integration algorithm for Bayesian model comparison and parameter estimation
	- https://johannesbuchner.github.io/UltraNest/
	- https://johannesbuchner.github.io/UltraNest/testsuite/