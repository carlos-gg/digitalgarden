---
title: "Neural Ordinary Differential Equations"
disableToc: false 
---

# Resources
- https://github.com/Zymrael/awesome-neural-ode
- Understanding Neural ODE's: https://jontysinai.github.io/jekyll/update/2019/01/18/understanding-neural-odes.html
- Neural Ordinary Differential Equations and Dynamics Models: https://medium.com/@ml.at.berkeley/neural-ordinary-differential-equations-and-dynamics-models-1a4277fbb80
	- ODEs are often used to describe the time derivatives of a physical situation, referred to as the dynamics. Knowing the dynamics allows us to model the change of an environment, like a physics simulation, unlocking the ability to take any starting condition and model how it will change. With Neural ODEs, we don’t define explicit ODEs to document the dynamics, but learn them via ML.
	- Strong connection with [[Residual and dense neural networks]]. Why do residual layers help networks achieve higher accuracies and grow deeper? Firstly, skip connections help information flow through the network by sending the hidden state, h(t), along with the transformation by the layer, f(h(t)), to layer t+1, preventing important information from being discarded by f. Secondly, residual layers can be stacked, forming very deep networks.
	- However, ResNets still employ many layers of weights and biases requiring much time and data to train. On top of this, the backpropagation algorithm on such a deep network incurs a high memory cost to store intermediate values.
	- Continuous depth ODENets are evaluated using black box ODE solvers, but first the parameters of the model must be optimized via gradient descent. To do this, we need to know the gradient of the loss with respect to the parameters, or how the loss function depends on the parameters in the ODENet.
	- In deep learning, backpropagation is the workhorse for finding this gradient, but this algorithm incurs a high memory costs to store the intermediate values of the network. On top of this, the sheer number of chain rule applications produces numerical error. Since an ODENet models a differential equation, these issues can be circumvented using sensitivity analysis methods developed for calculating gradients of a loss function with respect to the parameters of the system producing its input.


# References
- #PAPER Neural Ordinary Differential Equations (TQ Chen 2018): https://arxiv.org/abs/1806.07366
	- #CODE https://github.com/JSeam2/Neural-Ordinary-Differential-Equations
	- #CODE https://github.com/jason71995/Keras_ODENet
	- Neural Ordinary Differential Equations - Best Paper Awards NeurIPS 2018: https://www.youtube.com/watch?v=V6nGT0Gakyg
	- https://towardsdatascience.com/paper-summary-neural-ordinary-differential-equations-37c4e52df128
	- https://braindump.jethro.dev/posts/neural_ode/
	- https://msurtsukov.github.io/Neural-ODE/
	- https://github.com/msurtsukov/neural-ode/blob/master/Neural%20ODEs.ipynb
	- https://www.youtube.com/watch?v=jltgNGt8Lpg
- #PAPER Augmented Neural ODEs (Dupont 2019): https://arxiv.org/abs/1904.01681
- #PAPER Differential Bayesian Neural Nets (Look 2020): https://arxiv.org/abs/1912.00796
	- Neural Ordinary Differential Equations (N-ODEs) are a powerful building block for learning systems, which extend residual networks to a continuous-time dynamical system. Propose a Bayesian version of N-ODEs that enables well-calibrated quantification of prediction uncertainty, while maintaining the expressive power of their deterministic counterpart.
- #THESIS/MSC Generative Modeling with Neural Ordinary Differential Equations (2019): https://uwspace.uwaterloo.ca/bitstream/handle/10012/15354/Dockhorn_Tim.pdf
- #PAPER Universal Differential Equations for Scientific Machine Learning (Rackauckas 2020): https://arxiv.org/abs/2001.04385
	- https://www.stochasticlifestyle.com/how-to-train-interpretable-neural-networks-that-accurately-extrapolate-from-small-data/
- #PAPER Neural Differential Equations for Single Image Super-Resolution (Le Scao 2020): https://arxiv.org/pdf/2005.00865
- #PAPER Liquid Time-constant Networks (Hasani 2020): https://arxiv.org/abs/2006.04439
	- #TALK https://www.youtube.com/watch?v=IlliqYiRhMU
	- #CODE https://github.com/raminmh/liquid_time_constant_networks
	- https://news.mit.edu/2021/machine-learning-adapts-0128
