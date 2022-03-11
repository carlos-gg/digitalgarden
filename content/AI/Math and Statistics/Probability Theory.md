---
title: "Probability Theory"
disableToc: false 
---


## Resources
- https://en.wikipedia.org/wiki/Probability_theory
- https://stanford.edu/~shervine/teaching/cme-106/key-concepts
- [A visual introduction to probability and statistics](http://students.brown.edu/seeing-theory/)
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-probability
- Probability forms the foundation for almost all treatments of statistical inference. Probability is a law that assigns numbers to the long run occurrence of random phenomena after repeated unrelated realizations
- http://nbviewer.jupyter.org/url/norvig.com/ipython/Probability.ipynb
- https://en.wikipedia.org/wiki/Probability_interpretations
- https://en.wikipedia.org/wiki/Bayesian_probability
- [The Coursera Statistical Inference class](http://youtu.be/oTERv_vrmJM?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ)
- [Monty Hall problem](https://en.wikipedia.org/wiki/Monty_Hall_problem)
- [Coded in Python](https://github.com/cs109/2015lab1/blob/master/hw0.ipynb)
- Cheatsheets:
	- https://stanford.edu/~shervine/teaching/cme-106/cheatsheet-probability
	- Probability Cheatsheet (Chen): 
		- http://www.wzchen.com/probability-cheatsheet/
		- This is an 10-page probability cheatsheet compiled from Harvard's Introduction to Probability course, taught by Joe Blitzstein (@stat110). The probability formula sheet summarizes important probability probability concepts, formulas, and distributions, with figures, examples, and stories.
	- Review of Probability Theory (CS229 Stanford)
		- http://cs229.stanford.edu/section/cs229-prob.pdf	
		- http://cs229.stanford.edu/section/cs229-prob-slide.pdf

#### Random variables
- http://youtu.be/Shzt9uZ8BII?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-random-variables
- Random variable is a numerical outcome of an experiment. The random variables that we study will come in two varieties, discrete or continuous. Discrete random variables are random variables that take on only a countable number of possibilities. Mass functions will assign probabilities that they take specific values. Continuous random variable can conceptually take any value on the real line or some subset of the real line and we talk about the probability that they lie within some range. Densities will characterize these probabilities.
- For all of these kinds of random variables, we need convenient mathematical functions to model the probabilities of collections of realizations. These functions, called mass functions and densities, take possible values of the random variables, and assign the associated probabilities. These entities describe the population of interest.
- PDF - probability density function
	- https://en.wikipedia.org/wiki/Probability_density_function
	- http://youtu.be/mPe0Us4VYDM?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-probability-density-functions
	- A probability density function (pdf), is a function associated with a continuous random variable. Because of the peculiarities of treating measurements as having been recorded to infinite decimal expansions, we need a different set of rules. This leads us to the central dogma of probability density functions: Areas under PDFs correspond to probabilities for that random variable. 
	- A PDF, or density of a continuous random variable, is a function, whose value at any given sample (or point) in the sample space(the set of possible values taken by the random variable) can be interpreted as providing a relative likelihood that the value of the random variable would equal that sample.
	- The PDF is used to specify the probability of the random variable falling within a particular range of values, as opposed to taking on any one value.

#### Conditional probability
- http://youtu.be/u6AH6qsSVA4?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-conditional-probability
- Conditioning is a central subject in statistics. If we are given information about a random variable, it changes the probabilities associated with it. For example, the probability of getting a one when rolling a (standard) die is usually assumed to be one sixth. If you were given the extra information that the die roll was an odd number (hence 1, 3 or 5) then conditional on this new information, the probability of a one is now one third.
- http://setosa.io/ev/conditional-probability/

#### Independance
- https://en.wikipedia.org/wiki/Independence_(probability_theory)
- http://youtu.be/MY1EfrR1ZUs?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-independence
- Statistical independence of events is the idea that the events are unrelated. Consider successive coin flips. Knowledge of the result of the first coin flip tells us nothing about the second.
- The important principle is that probabilities of independent things multiply! This has numerous consequences, including the idea that we shouldn’t multiply non-independent probabilities.
- [IID samples ](https://en.wikipedia.org/wiki/Independent_and_identically_distributed_random_variables)
	- IID - Independent and identically distributed 
	- In probability theory and statistics, a sequence or other collection of random variables is independent and identically distributed(i.i.d.) if each random variable has the same probability distribution as the others and all are mutually independent.
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-iid-random-variables
	- Random variables are said to be independent and identically distributed (iid) if they are independent and all are drawn from the same population. The reason iid samples are so important is that they are a model for random samples. This is a default starting point for most statistical inferences.
  
#### Common distributions
- https://stanford.edu/~shervine/teaching/cme-106/distribution-tables
- https://blog.cloudera.com/blog/2015/12/common-probability-distributions-the-data-scientists-crib-sheet/
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-some-common-distributions
- [Normal distribution](http://efavdb.com/normal-distributions/)
- Bernoulli
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-the-bernoulli-distribution
	- TheBernoulli distribution arises as the result of a binary outcome, such as a coin flip.
- Normal
	- http://youtu.be/dUTWvKa0Leo?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-the-normal-distribution
	- The normal distribution is easily the handiest distribution in all of statistics. It can be used in an endless variety of settings. Moreover, as we’ll see later on in the course, sample means follow normal distributions for large sample sizes.
	- The normal distribution only requires two numbers to characterize it, mean and variance.
- Poisson
	- http://youtu.be/ZPLZg7qz4xE?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-the-poisson-distribution
	- The Poisson distribution is used to model counts. It is perhaps only second to the normal distribution usefulness. In fact, the Bernoulli, binomial and multinomial distributions can all be modeled by clever uses of the Poisson.
	- The Poisson distribution is especially useful for modeling unbounded counts or counts per unit of time (rates). Like the number of clicks on advertisements, or the number of people who show up at a bus stop. There is also a deep connection between the Poisson distribution and popular models for so-called event-time data.

#### Expected value
- https://en.wikipedia.org/wiki/Expected_value
- In probability theory, the expected value of a random variable, intuitively, is the long-run average value of repetitions of the experiment it represents.
- Less roughly, the law of large numbers states that the arithmetic mean of the values almost surely converges to the expected value as the number of repetitions approaches infinity. The expected value is also known as the expectation, mathematical expectation, EV, average, mean value, mean, or first moment.
- [Expected values](http://youtu.be/zljxRbu6jyc?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ)
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-expected-values
- Expected values characterize a distribution. The most useful expected value, the mean, characterizes the center of a density or mass function. Another expected value summary, the variance, characterizes how spread out a density is. Yet another expected value calculation is the skewness, which considers how much a density is pulled toward high or low values.

#### Central limit theorem
- https://en.wikipedia.org/wiki/Central_limit_theorem
- http://youtu.be/FAIyVHmniK0?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-the-central-limit-theorem
- CLT is one of the most important theorems in statistics. For our purposes, the CLT states that the distribution of averages of iid variables becomes that of a standard normal as the sample size increases.

#### Kullback-Leibler Divergence
- https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence
- https://www.countbayesie.com/blog/2017/5/9/kullback-leibler-divergence-explained


## Books
- #COURSE [Introduction to Probability and Statistics (MIT)](https://ocw.mit.edu/courses/mathematics/18-05-introduction-to-probability-and-statistics-spring-2014/)