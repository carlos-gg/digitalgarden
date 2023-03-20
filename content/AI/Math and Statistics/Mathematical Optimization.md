---
title: "Mathematical Optimization"
---


## Resources
- https://en.wikipedia.org/wiki/Mathematical_optimization
- [A birds-eye view of optimization algorithms (Pedregosa)](http://fa.bianp.net/teaching/2018/eecs227at/)
- http://people.duke.edu/~ccc14/sta-663/BlackBoxOptimization.html
- http://www.benfrederickson.com/numerical-optimization/ (notebook kind of post with python, d3)
- http://www.kdnuggets.com/2016/12/hard-thing-about-deep-learning.html
- https://www.neuraldesigner.com/blog/5_algorithms_to_train_a_neural_network
- [Why Momentum works](http://distill.pub/2017/momentum/)

### Heuristics
- See "Genetic algorithms" in [[AI/Evolutionary computation]]
- A heuristic is any algorithm which is not guaranteed (mathematically) to find the solution, but which is nevertheless useful in certain practical situations.
- [Nelder–Mead method](https://en.wikipedia.org/wiki/Nelder%E2%80%93Mead_method)
	- The Nelder–Mead method or downhill simplex method or amoeba method is a commonly applied numerical method used to find the minimum or maximum of an objective function in a multidimensional space. It is applied to nonlinear optimization problems for which derivatives may not be known. However, the Nelder–Mead technique is a heuristic search method that can converge to non-stationary points on problems that can be solved by alternative methods.
	- The method uses the concept of a simplex, which is a special polytope of n+ 1 vertices in n dimensions. Examples of simplices include a line segment on a line, a triangle on a plane, a tetrahedron in three-dimensional space and so forth. The method approximates a local optimum of a problem with n variables when the objective function varies smoothly and is unimodal.
	- Nelder–Mead in n dimensions maintains a set of n+1test points arranged as a simplex. It then extrapolates the behavior of the objective function measured at each test point, in order to find a new test point and to replace one of the old test points with the new one, and so the technique progresses. The simplest approach is to replace the worst point with a point reflected through the centroid of the remaining n points. If this point is better than the best current point, then we can try stretching exponentially out along this line. On the other hand, if this new point isn't much better than the previous value, then we are stepping across a valley, so we shrink the simplex towards a better point.
	- [The Nelder–Mead algorithm](https://pyfssa.readthedocs.io/en/stable/nelder-mead.html)
	- https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.fmin.html

### Iterative methods
- Iterative methods used to solve problems of nonlinear programming differ according to whether they evaluate Hessians, gradients, or only function values.
- Gradient descent
	- https://en.wikipedia.org/wiki/Gradient_descent
	- Gradient descent is a first-order iterative optimization algorithm. To find a local minimum of a function using gradient descent, one takes steps proportional to the negative of the gradient (or of the approximate gradient) of the function at the current point. Gradient descent is also known as steepest descent, or the method of steepest descent.
	- [An overview of gradient descent optimization algorithms](http://ruder.io/optimizing-gradient-descent/index.html)
	- https://towardsdatascience.com/gradient-descent-demystified-bc30b26e432a
	- https://www.jeremyjordan.me/gradient-descent/
- [Conjugate gradient method](https://en.wikipedia.org/wiki/Conjugate_gradient_method)
- [Interior point method](https://en.wikipedia.org/wiki/Interior_point_method)


## Code
- #CODE [Nevergrad (Facebook)](https://code.fb.com/ai-research/nevergrad/)
	- A Python toolbox for performing gradient-free optimization
- #CODE [Theseus (Facebook)](https://github.com/facebookresearch/theseus)
	- A library for differentiable nonlinear optimization
	- https://sites.google.com/view/theseus-ai
- #CODE [scikit-optimize](https://scikit-optimize.github.io/)
- #CODE [GPflowOpt - library for Bayesian Optimization with GPflow](https://gpflowopt.readthedocs.io/en/latest/index.html )
- #CODE [PyBrain - Black-box Optimization Algorithms](http://pybrain.org/docs/api/optimization/optimization.html)
- #CODE [JAX](https://github.com/google/jax) ^jax
	- JAX is Autograd and XLA, brought together for high-performance machine learning research. It can automatically differentiate native Python and NumPy functions
	- #TALK [JAX: Accelerated Machine Learning Research | SciPy 2020 | VanderPlas](https://www.youtube.com/watch?v=z-WSrQDXkuM)
	- https://towardsdatascience.com/deep-learning-with-jax-and-elegy-c0765e3ec31a
	- #TALK [Machine Learning with JAX - From Zero to Hero](https://www.youtube.com/watch?v=SstuvS-tVc0)