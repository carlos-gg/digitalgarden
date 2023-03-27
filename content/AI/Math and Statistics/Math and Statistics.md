---
title: "Math and Statistics"
---

## Resources
- https://en.wikipedia.org/wiki/Portal:Mathematics
- https://en.wikipedia.org/wiki/Mathematics
- [Statistics cheatsheet](https://stanford.edu/~shervine/teaching/cme-106/cheatsheet-statistics)
- [Mathematics for Machine Learning](https://github.com/dair-ai/Mathematics-for-ML)
- https://github.com/rouseguy/intro2stats
- [Stanford-cs-229 ML, probability and stats refresher](https://github.com/afshinea/stanford-cs-229-machine-learning/blob/master/en/refresher-probabilities-statistics.pdf)
- https://www.khanacademy.org/math/statistics-probability
- http://christopherroach.com/articles/statistics-for-hackers/
- [Trigonometry refresher](https://stanford.edu/~shervine/teaching/cme-102/trigonometry)

## Books
- #BOOK [Essential Mathematics and Statistics for Science (Currell 2009, WILEY)](https://www.wiley.com/en-us/Essential+Mathematics+and+Statistics+for+Science%2C+2nd+Edition-p-9780470694480)
	- http://www.stewartschultz.com/statistics/books/Essential%20Mathematics.pdf
- #BOOK [Think Stats - Exploratory Data Analysis in Python (Downey 2014)](https://greenteapress.com/wp/think-stats-2e/)
	- Think Stats is an introduction to Probability and Statistics for Python programmers
- #BOOK [An Introduction to Statistics with Python (Haslwanter, 2015 6 SPRINGER)](https://www.springer.com/fr/book/9783319283159)
	- Applications in the life sciences
	- https://es.scribd.com/document/338198132/An-Introduction-to-Statistics-With-Python-With-Applications-in-the-Life-Sciences
- #BOOK [Statistical Thinking for the 21st Century (Poldrack 2018)](http://statsthinking21.org/index.html)
	- R language
- #BOOK [Jupyter Guide to Linear Algebra](https://bvanderlei.github.io/jupyter-guide-to-linear-algebra/intro.html)

## Courses
- #COURSE [Statistical inference for data science](https://www.coursera.org/learn/statistical-inference)
	- https://leanpub.com/LittleInferenceBook
	- [Coursera Inference Version 3](https://www.youtube.com/playlist?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ)
- #COURSE [Probability and Statistics (Stanford online)](https://lagunita.stanford.edu/courses/course-v1:OLI+ProbStat+Open_Jan2017/about)
- #COURSE [Modern Applied Statistics: Elements of Statistical Learning (Statistics 315a, Stanford)](http://statweb.stanford.edu/~tibs/stat315a/)
- #COURSE [Calculus introductory courses (MIT)](https://ocw.mit.edu/high-school/mathematics/)
	- [Single Variable Calculus (18.01SC)](https://ocw.mit.edu/courses/mathematics/18-01sc-single-variable-calculus-fall-2010)
	- [Multivariable Calculus (18.02SC)](https://ocw.mit.edu/courses/mathematics/18-02sc-multivariable-calculus-fall-2010)
	- [Highlights of calculus (Strang)](https://ocw.mit.edu/resources/res-18-005-highlights-of-calculus-spring-2010)
- #TALK [Statistics in Python (Varoquaux 2015 Euroscipy)](https://www.youtube.com/watch?v=yaSgoGLXKOg)

## Code
- #CODE [Numpy](https://numpy.org/)
	- #PAPER [Array programming with NumPy (Harris 2020)](https://www.nature.com/articles/s41586-020-2649-2)
- #CODE [Scipy](https://www.scipy.org/)
- #CODE [Nums](https://github.com/nums-project/nums)
	- A library that translates Python and NumPy to optimized distributed systems code
- #CODE [Statsmodels](http://www.statsmodels.org/)
- #CODE [PyLops](https://github.com/PyLops/pylops)
	- https://pylops.readthedocs.io/en/latest/index.html
	- Python library is inspired by the MATLAB Spot – A Linear-Operator Toolbox project
- #CODE [Bayesian bootstrap](https://github.com/lmc2179/bayesian_bootstrap)


### A/B testing
- #CODE [Sixpack](https://github.com/sixpack/sixpack)
- #CODE [Expan (Zalando)](https://github.com/zalando/expan)
	- A Python library for statistical analysis of randomised control trials (A/B tests)
	- #TALK https://www.youtube.com/watch?v=furJxiZlo6w
- #CODE Proctor (Indeed): 
	- https://github.com/indeedeng/proctor
	- http://opensource.indeedeng.io/proctor/


## Subtopics
### Calculus
- [Calculus refresher](https://stanford.edu/~shervine/teaching/cme-102/calculus)
- Ordinary Differential Equations
	- https://stanford.edu/~shervine/teaching/cme-102/cheatsheet-first-ode
	- https://stanford.edu/~shervine/teaching/cme-102/cheatsheet-second-ode
	- https://stanford.edu/~shervine/teaching/cme-102/cheatsheet-applications
- [Stanford-cs-229 ML, algebra and calculus refresher](https://github.com/afshinea/stanford-cs-229-machine-learning/blob/master/en/refresher-algebra-calculus.pdf)
- https://scipy-latinamerica.github.io/revista.io/blog/2018/10/20/introduccion-al-calculo-con-python/
- https://www.khanacademy.org/math/multivariable-calculus

### Linear Algebra
See [[AI/Math and Statistics/Linear Algebra]]


### Distances
See [[AI/Math and Statistics/Distances]]


### Descriptive stats
- https://en.wikipedia.org/wiki/Descriptive_statistics
- http://debrouwere.org/2017/02/01/unlearning-descriptive-statistics/

#### Correlation and dependance
- https://www.datascience.com/blog/introduction-to-correlation-learn-data-science-tutorials
- https://en.wikipedia.org/wiki/Correlation_and_dependence
- Correlation is a statistical measure that describes the association between random variables. Why is correlation a useful metric?
	- Correlation can help in predicting one quantity from another
	- Correlation can (but often does not, as we will see in some examples below) indicate the presence of a causal relationship
	- Correlation is used as a basic quantity and foundation for many other modeling techniques
- Types:
	- Pearson’s Correlation: 
		- Pearson is the most widely used correlation coefficient. Pearson correlation measures the linear association between continuous variables. In other words, this coefficient quantifies the degree to which a relationship between two variables can be described by a line. Raw observations are centered by subtracting their means and re-scaled by a measure of standard deviations.
		- `Ro_X,Y = E[(X - mu_X)(Y - mu_Y)] / simga_X sigma_Y `
		- numerator  -> covariance
		- Dividing the covariance between two variables by the product of standard deviations ensures that correlation will always fall between -1 and 1 (much easier to interpret)
	- Spearman's Correlation:
		- Spearman's rank correlation coefficient can be defined as a special case of Pearson ρapplied to ranked (sorted) variables. Rather than comparing means and variances, Spearman's coefficient looks at the relative order of values for each variable. The formula for Spearman's coefficient looks very similar to that of Pearson, with the distinction of being computed on ranks instead of raw scores. 
	- Kendall's Tau:
		- Also based on variable ranks, however, unlike Spearman's coefficient, Kendall’s tau does not take into account the difference between ranks— only directional agreement.
- Covariance (matrix)
	- https://en.wikipedia.org/wiki/Covariance
	- In probability theory and statistics, covariance is a measure of the joint variability of two random variables. The sign of the covariance therefore shows the tendency in the linear relationship between the variables. The magnitude of the covariance is not easy to interpret. The normalized version of the covariance, the correlation coefficient, however, shows by its magnitude the strength of the linear relation. 
	- [In multidimensional case: covariance matrix](https://en.wikipedia.org/wiki/Covariance_matrix)
- Correlation & Causation 
	- https://en.wikipedia.org/wiki/Correlation_does_not_imply_causation
	- "Correlation does not imply causation" is a phrase used in statistics to emphasize that a correlation between two variables does not imply that one causes the other. Spurious statistical associations can be found in a multitude of quantities, simply due to chance.
	- Often, a relationship may appear to be causal through high correlation due to some unobserved variables. For example, the number of grocery stores in a city can be strongly correlated with the number of ice cream creameries. However, there is an obvious hidden variable here— the population size of the city.
	- https://medium.com/@akelleh/a-technical-primer-on-causality-181db2575e41#.4csn3na8j
	- https://www.khanacademy.org/math/probability/scatterplots-a1/creating-interpreting-scatterplots/v/correlation-and-causality
	- Also, weak or no correlation does not imply lack of association. Correlation is only one data summary statistic that by no means tells the complete story of relationships in the data.


### Experimental design
See [[AI/Active learning]]
- [Coursera - data scientist's toolbox](https://www.youtube.com/watch?v=vSXOJnGNtM4)
- Good experiment: replication, measure variability, generalise to the problem, transparent
- Confounding variable - strategies: randomization, stratifying 
- Prediction is not and inference. Both are important and depend on the problem. Prediction is more challenging that inference. For prediction there are key quantities (metrics): sensitivity, specificity, positive predictive value, negative predictive value, accuracy

#### A/B testing
- https://en.wikipedia.org/wiki/A/B_testing
- In marketing and business intelligence, A/B testing is a term for a randomized experiment with two variants, A and B, which are the control and variation in the controlled experiment. A/B testing is a form of statistical hypothesis testing with two variants leading to the technical term, two-sample hypothesis testing, used in the field of statistics. Other terms used for this method include bucket tests and split-run testing.
- https://www.optimizely.com/ab-testing/
- https://www.wired.com/2012/04/ff_abtesting/
- http://data36.com/ab-testing-5-rules/
- https://www.udacity.com/course/ab-testing--ud257
- https://tech.okcupid.com/the-pitfalls-of-a-b-testing-in-social-networks/
- https://www.quora.com/What-kind-of-A-B-testing-questions-should-I-expect-in-a-data-scientist-interview-and-how-should-I-prepare-for-such-questions
- http://www.kdnuggets.com/2017/05/must-know-key-issues-problems-ab-testing.html

#### Multi-armed bandit
- http://blog.actblue.com/2015/04/29/the-multi-armed-bandit-new-and-much-improved-ab-testing-tools-2/
- https://conversionxl.com/bandit-tests/
- https://support.google.com/analytics/answer/2844870?hl=en
- https://vwo.com/blog/multi-armed-bandit-algorithm/

### Statistical Inference
- https://en.wikipedia.org/wiki/Statistical_inference
- https://www.youtube.com/watch?v=WkOinijQmPU&feature=youtu.be&list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
- https://leanpub.com/LittleInferenceBook/
- Statistical inference : the process of generating conclusions about a population from a noisy sample. Without statistical inference we’re simply living within our data. With statistical inference, we’re trying to generate new knowledge. The use of probability models as the connection between our data and a populations represents the most effective way to obtain inference.
- Question to answer: Are the statistics calculated on a small sample representative of the ones of the whole population?
- http://www.datasciencecentral.com/profiles/blogs/the-death-of-the-statistical-test-of-hypothesis

#### Frequentist inference
- https://en.wikipedia.org/wiki/Frequentist_inference
- https://en.wikipedia.org/wiki/Nonparametric_statistics
- Statistical Hypothesis testing
	- http://youtu.be/Wqvx6_12ZMs?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-hypothesis-testing
	- Hypothesis testing is concerned with making decisions using data. 
	- To make decisions using data, we need to characterize the kinds of conclusions we can make. Classical hypothesis testing is concerned with deciding between two decisions (things get much harder if there’s more than two). The first, a null hypothesis is specified that represents the status quo. This hypothesis is usually labeled, H_0. This is what we assume by default. The alternative or research hypothesis is what we require evidence to conclude. This hypothesis is usually labeled H_a, or sometimes H_1 (or some other number other than 0). So to reiterate, the null hypothesis is assumed true and statistical evidence is required to reject it in favor of a research or alternative hypothesis	
	- [t-test](https://en.wikipedia.org/wiki/Student%27s_t-test)
		- http://www.cs.cornell.edu/~asampson/blog/statsmistakes.html
		- https://www.quora.com/What-is-an-intuitive-explanation-of-the-t-test-in-hypothesis-testing
		- https://medium.freecodecamp.org/the-t-distribution-a-key-statistical-concept-discovered-by-a-beer-brewery-dbfdc693184
		- Good for small samples? 
			- Historically, the very first demonstration of the t-test (in "Student"'s 1908 paper) was in an application to sample sizes of size four. Indeed, obtaining improved results for smallsamples is the test's claim to fame: once the sample size reaches 40 or so, the t-test is not substantially different from the z-tests researchers had been applying throughout the 19th century.  
			- There is no minimum sample size for the t test to be valid. Validity requires that the assumptions for the test statistic hold approximately. Those assumptions are in the one sample case that the data are iid normal (or approximately normal) with mean 0 under the null hypothesis and a variance that is unknown but estimated from the sample. In the two sample case it is that both samples are independent of each other and each sample consists of iid normal variables with the two samples having the same mean and a common unknown variance under the null hypothesis. A pooled estimate of variance is used for the statistic. 
			- The problem with low sample size is with regard to the power of the test. 
			- Using the Student’s t-test with extremely small sample sizes (Winter 2013). It is concluded that there are no principal objections to using a t-test with Ns as small as 2. This study showed that there are no objections to using a t-test with extremely small samples, as long as the effect size is large.  
	- [z-test](https://en.wikipedia.org/wiki/Z-test)
	- [f-test](https://en.wikipedia.org/wiki/F-test)
	- [Mann–Whitney U test](https://en.wikipedia.org/wiki/Mann%E2%80%93Whitney_U_test)
	- [Welch's t-test](https://en.wikipedia.org/wiki/Welch%27s_t-test)
	- [Anderson–Darling test](https://en.wikipedia.org/wiki/Anderson%E2%80%93Darling_test)
	- [Kolmogorov–Smirnov test](https://en.wikipedia.org/wiki/Kolmogorov%E2%80%93Smirnov_test)
		- In essence, the test answers the question "What is the probability that this collection of samples could have been drawn from that probability distribution?" or, in the second case, "What is the probability that these two sets of samples were drawn from the same (but unknown) probability distribution?"
		- https://asaip.psu.edu/Articles/beware-the-kolmogorov-smirnov-test/
- Confidence intervals
	- http://youtu.be/u85aQ0mtiZ8?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-confidence-intervals
	- Confidence intervals are methods for quantifying uncertainty in our estimates. The fact that the interval has width characterizes that there is randomness that prevents us from getting a perfect estimate.
	- t-confidence intervals
		- http://youtu.be/pHXrDMjzyYg?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
		- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-t-confidence-intervals
- Null hypothesis
	- https://en.wikipedia.org/wiki/Null_hypothesis
	- The term "null hypothesis" is a general statement or default position that there is no relationship between two measured phenomena, or no association among groups.
	- H_0 is generally assumed to be true until evidence indicates otherwise.
- P-value
	- https://en.wikipedia.org/wiki/P-value
	- A p-value is the probability that, using a given statistical model, the statistical summary (such as the sample mean difference between two compared groups) would be the same as or more extreme than the actual observed results, when the null hypothesis is true.
	- After choosing the models H_0, H_1 and a threshold value alpha for p (the significance level of the test, traditionally 5% or 1%), if the p-value is less than or equal to alpha, the test suggests that the observed data is inconsistent with the null hypothesis, so the null hypothesis must be rejected. However, that does not prove that the tested hypothesis is true. When the p-value is calculated correctly, this test guarantees that the Type I error rate is at most alpha. For typical analysis, using the standard alpha= 0.05 cutoff, the null hypothesis is rejected when p< .05 and not rejected when p> .05. 
	- The p-value does not, in itself, support reasoning about the probabilities of hypotheses but is only a tool for deciding whether to reject the null hypothesis (it can only provide evidence against a hypothesis).
	- http://youtu.be/Ky68x_7iK6c?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-p-values
	- P-values are the most common measure of statistical significance. Their ubiquity, along with concern over their interpretation and use makes them controversial among statisticians.
	- http://blog.minitab.com/blog/adventures-in-statistics-2/how-to-correctly-interpret-p-values
	- A P value is the probability of obtaining an effect at least as extreme as the one in your sample data, assuming the truth of the null hypothesis.
	- For example, suppose that a vaccine study produced a P value of 0.04. This P value indicates that if the vaccine had no effect, you’d obtain the observed difference or more in 4% of studies due to random sampling error. 
	- P values address only one question: how likely are your data, assuming a true null hypothesis? It does not measure support for the alternative hypothesis.
	- http://machinelearningmastery.com/use-statistical-significance-tests-interpret-machine-learning-results/
	- https://www.nature.com/news/big-names-in-statistics-want-to-shake-up-much-maligned-p-value-1.22375
- Statistical Power
	- https://en.wikipedia.org/wiki/Statistical_power
	- #TALK Statistical power:
		- http://youtu.be/-TsBOLiW4rQ?list=PLpl-gQkQivXiB1mGyzLrUjzsblmQsLtkzJ
		- http://youtu.be/GRS2b1aedmk?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
	- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-power
	- Power is the probability of rejecting the null hypothesis when it is false. Ergo, power (as its name would suggest) is a good thing; you want more power. A type II error (a bad thing, as its name would suggest) is failing to reject the null hypothesis when it’s false; the probability of a type II error is usually called Beta. Note Power = 1 - Beta.
- [Effect size](https://en.wikipedia.org/wiki/Effect_size)
- [Goodness of fit](https://en.wikipedia.org/wiki/Goodness_of_fit)
	- [Chi squared](https://en.wikipedia.org/wiki/Chi-squared_test)

### Bootstrap and permutation tests
- http://youtu.be/0hNQx9nagq4?list=PLpl-gQkQivXiBmGyzLrUjzsblmQsLtkzJ
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-the-bootstrap-and-resampling
- The bootstrap is a tremendously useful tool for constructing confidence intervals and calculating standard errors for difficult statistics. That’s the bootstrap principle: investigate the sampling distribution of a statistic by simulating repeated realizations from the observed distribution.
- https://leanpub.com/LittleInferenceBook/read#leanpub-auto-permutation-tests
- Consider comparing means between the group. However, let’s use the calculate the distribution of our statistic under a null hypothesis that the labels are irrelevant (exchangeable). This is a handy way to create a null distribution for our test statistic by simply permuting the labels over and over and seeing how extreme our data are with respect to this permuted distribution. 
- The procedure would be as follows: 
	- consider a data from with count and spray,
	- permute the spray (group) labels,
	- recalculate the statistic (such as the difference in means),
	- calculate the percentage of simulations where the simulated statistic was more extreme (toward the alternative) than the observed.

#### Bayesian bootstrap
- http://www.sumsar.net/blog/2015/04/the-non-parametric-bootstrap-as-a-bayesian-model/

### Probability theory
See [[AI/Math and Statistics/Probability Theory]]

### Bayesian modelling
See [[AI/Bayesian modelling]]

### Monte Carlo methods
See [[AI/Math and Statistics/Monte Carlo methods]]

### Mathematical Optimization
See [[AI/Math and Statistics/Mathematical Optimization]]

### Time series analysis
See [[AI/Time Series analysis]]

### Regression analysis
See [[AI/Supervised Learning/Regression]]
- https://en.wikipedia.org/wiki/Regression_analysis
- Regression analysis is widely used for prediction and forecasting, where its use has substantial overlap with the field of [[AI/ML]]

### Compressed sensing
See [[AI/Unsupervised learning/Sparse dictionary learning]]
- https://en.wikipedia.org/wiki/Compressed_sensing
- Compressed sensing(also known as compressive sensing, compressive sampling, or sparse sampling) is a signal processing technique for efficiently acquiring and reconstructing a signal, by finding solutions to underdetermined linear systems. This is based on the principle that, through optimization, the sparsity of a signal can be exploited to recover it from far fewer samples than required by the Shannon-Nyquist sampling theorem.
- There are two conditions under which recovery is possible: 
	- Sparsity, which requires the signal to be sparse in some domain. 
	- Incoherence, which is applied through the isometric property which is sufficient for sparse signals
- https://calculatedcontent.com/2012/12/28/foundations-theory-of-compressed-sensing/amp/

#### Nyquist theorem
- https://en.wikipedia.org/wiki/Nyquist%E2%80%93Shannon_sampling_theorem
- In the field of digital signal processing, the sampling theorem is a fundamental bridge between continuous-time signals(often called "analog signals") and discrete-time signals(often called "digital signals"). It establishes a sufficient condition for a sample rate that permits a discrete sequence of samples to capture all the information from a continuous-time signal of finite bandwidth.

#### Matching pursuit
- https://en.wikipedia.org/wiki/Matching_pursuit
- Matching pursuit (MP) is asparse approximation algorithm which involves finding the "best matching" projections of multidimensional data onto the span of an over-complete (i.e., redundant) dictionary D.
- Orthogonal Matching Pursuit
	- Extension of MP: after every step, all the coefficients extracted so far are updated, by computing the orthogonal projection of the signal onto the set of atoms selected so far. This can lead to better results than standard MP, but requires more computation.
	- http://scikit-learn.org/stable/auto_examples/linear_model/plot_omp.html
