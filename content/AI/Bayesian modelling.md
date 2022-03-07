---
title: "Bayesian modelling"
disableToc: false 
---

See [Bayesian neural networks](Bayesian%20neural%20networks.md)

# Resources
- https://en.wikipedia.org/wiki/Bayesian_statistics
- https://en.wikipedia.org/wiki/Bayesian_inference
- http://brohrer.github.io/how_bayesian_inference_works.html
- http://willwolf.io/en/2017/02/07/bayesian-inference-via-simulated-annealing/
- #TALK Bayesian Inference, Shakir Mohamed, MLSS 2020:
	- Part I:  https://www.youtube.com/watch?v=x4Y90zPjbq0
	- Part II: https://www.youtube.com/watch?v=x4Y90zPjbq0&feature=youtu.be

## Bayesian vs frequentist discussion
- http://jakevdp.github.io/blog/2014/03/11/frequentism-and-bayesianism-a-practical-intro/
- http://www.fharrell.com/2017/02/my-journey-from-frequentist-to-bayesian.html
- https://mchankins.wordpress.com/2013/04/21/still-not-significant-2/
- https://aeon.co/essays/it-s-time-for-science-to-abandon-the-term-statistically-significant
- http://www.fharrell.com/2017/02/a-litany-of-problems-with-p-values.html?m=1

## Bayes theorem
- http://blogs.scientificamerican.com/cross-check/bayes-s-theorem-what-s-the-big-deal/
- http://www.analyticsvidhya.com/blog/2016/06/bayesian-statistics-beginners-simple-english/

## MAP
- https://en.wikipedia.org/wiki/Maximum_a_posteriori_estimation
- In Bayesian statistics, a maximum a posteriori probability(MAP) estimate is an estimate of an unknown quantity, that equals the mode of the posterior distribution. The MAP can be used to obtain a point estimate of an unobserved quantity on the basis of empirical data.It is closely related toFisher's method of maximum likelihood(ML) estimation, but employs an augmented optimization objective which incorporates a prior distribution(that quantifies the additional information available through prior knowledge of a related event) over the quantity one wants to estimate. MAP estimation can therefore be seen as a regularization of ML estimation.

## MLE
- https://en.wikipedia.org/wiki/Maximum_likelihood_estimation
- Maximum likelihood estimation (MLE) is a method of estimating the parameters of a statistical model given observations, by finding the parameter values that maximize the likelihood of making the observations given the parameters. MLE can be seen as a special case of the maximum a posteriori estimation (MAP) that assumes a uniform prior distribution of the parameters, or as a variant of the MAP that ignores the prior and which therefore is unregularized.

## Bayesian network
- https://en.wikipedia.org/wiki/Bayesian_network

## Variational Bayesian methods
- See [Normalizing flows](Normalizing%20flows.md)
- Variational Bayesian inference with normalizing flows: a simple example: https://towardsdatascience.com/variational-bayesian-inference-with-normalizing-flows-a-simple-example-1db109d91062
	- #CODE https://github.com/fraseriainlewis/towardsdatascience

# Code
- A list of Python-based MCMC packages. Also here’s a nice list of MCMC algorithms: https://gabriel-p.github.io/pythonMCMC/
- #CODE Stan: https://github.com/stan-dev/stan
	- http://mc-stan.org
- #CODE Pymc3 - Probabilistic Programming in Python: http://pymc-devs.github.io/pymc3/
- #CODE emcee: http://dan.iel.fm/emcee/current/
- #CODE Arviz - Exploratory analysis of Bayesian models with Python: https://arviz-devs.github.io/arviz/
- #CODE Sampyl - MCMC samplers for Bayesian estimation in Python, including Metropolis-Hastings, NUTS, and Slice: http://mcleonard.github.io/sampyl/
- #CODE BayesicFitting - A package for model fitting and bayesian evidence calculation: https://github.com/dokester/BayesicFitting
- #CODE UltraNest - A Pythonic implementation of the Nested Sampling integration algorithm for Bayesian model comparison and parameter estimation
	- https://johannesbuchner.github.io/UltraNest/
	- https://johannesbuchner.github.io/UltraNest/testsuite/

# Books
- #BOOK Think Bayes - Bayesian Statistics Made Simple (Downey 2012): http://greenteapress.com/wp/think-bayes/
	- Think Bayes is an introduction to Bayesian statistics using computational methods
- #BOOK Probabilistic programming and bayesian methods for hackers: http://camdavidsonpilon.github.io/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/
	- https://github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers
- #BOOK Bayesian Modeling and Computation in Python (Martin 2021, CRC): https://bayesiancomputationbook.com/welcome.html


# References
- #PAPER Bayesian model selection for complex dynamic systems (Mark 2018): https://www.nature.com/articles/s41467-018-04241-5 ^1ef748
