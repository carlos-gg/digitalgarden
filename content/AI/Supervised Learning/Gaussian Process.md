# Gaussian Process

- https://en.wikipedia.org/wiki/Gaussian_process
- In probability theory and statistics, a Gaussian process is a stochastic process (a collection of random variables indexed by time or space), such that every finite collection of those random variables has a multivariate normal distribution, i.e. every finite linear combination of them is normally distributed. The distribution of a Gaussian process is the joint distribution of all those (infinitely many) random variables, and as such, it is a distribution over functions with a continuous domain, e.g. time or space.
- A machine-learning algorithm that involves a Gaussian process uses lazy learning and a measure of the similarity between points (the kernel function) to predict the value for an unseen point from training data. The prediction is not just an estimate for that point, but also has uncertainty information—it is a one-dimensional Gaussian distribution (which is the marginal distribution at that point).
- http://scikit-learn.org/stable/modules/gaussian_process.html
- A Practical Guide to Gaussian Processes: https://drafts.distill.pub/gp/ 
- A Visual Exploration of Gaussian Processes
	- https://www.jgoertler.com/visual-exploration-gaussian-processes/
	- https://blog.dominodatalab.com/fitting-gaussian-process-models-python/
- Gaussian processes: http://krasserm.github.io/2018/03/19/gaussian-processes/

## Code
- #CODE GPy: https://github.com/SheffieldML/GPy
- #CODE GPyTorch: https://github.com/cornellius-gp/gpytorch
	- https://gpytorch.ai/
- #CODE GPFlow: https://github.com/GPflow/GPflow
	- https://gpflow.readthedocs.io/en/master/intro.html
- #CODE GPflux: https://github.com/secondmind-labs/GPflux
	- GPflux uses the mathematical building blocks from GPflow and marries these with the powerful layered deep learning API provided by Keras. 
	- https://secondmind-labs.github.io/GPflux/tutorials.html


## Books and review papers
- #BOOK Bayesian Optimization Book (Garnett 2021): https://bayesoptbook.com/
- #PAPER An Intuitive Tutorial to Gaussian Processes Regression (Wang 2021): https://arxiv.org/abs/2009.10862
- #PAPER Deep Gaussian Processes: A Survey (Jakkala 2021): https://arxiv.org/abs/2106.12135


## References
- #PAPER Gaussian Processes for Machine Learning (Rasmussen and Williams 2006): http://www.gaussianprocess.org/gpml/
	- http://www.gaussianprocess.org/gpml/chapters/RW.pdf
- #PAPER Convolutional Gaussian Processes (van der Wilk 2017): https://arxiv.org/abs/1709.01894
	- #CODE https://gpflow.readthedocs.io/en/master/notebooks/advanced/convolutional.html
- #PAPER Deep convolutional Gaussian processes (Blomqvist 2018): https://arxiv.org/abs/1810.03052
	- #CODE https://github.com/kekeblom/DeepCGP
	- https://github.com/kekeblom/DeepCGP/blob/master/notebooks/Inspect.ipynb
- #PAPER Gaussian processes meet NeuralODEs: A Bayesian framework for learning the dynamics of partially observed systems from scarce and noisy data (Aziz Bhouri 2021): https://arxiv.org/abs/2103.03385
	- #CODE https://github.com/PredictiveIntelligenceLab/GP-NODEs
