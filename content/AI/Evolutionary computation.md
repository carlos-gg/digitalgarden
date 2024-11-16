---
title: "Evolutionary computation"
---

> In computer science, evolutionary computation is a family of algorithms for global optimization inspired by biological evolution, and the subfield of artificial intelligence and soft computing studying these algorithms. In technical terms, they are a family of population-based trial and error problem solvers with a metaheuristic or stochastic optimization character.

## Resources
- https://en.wikipedia.org/wiki/Evolutionary_algorithm
- https://en.wikipedia.org/wiki/Evolutionary_computation
- [Evolutionary Computation (FULL COURSE) Overview](https://towardsdatascience.com/evolutionary-computation-full-course-overview-f4e421e945d9)

### Genetic algorithms
- https://en.wikipedia.org/wiki/Genetic_algorithm
- Metaheuristic inspired by the process of natural selection that belongs to the larger class of evolutionary algorithms. Genetic algorithms are commonly used to generate high-quality solutions to optimization and search problems by relying on bio-inspired operators such as mutation, crossover and selection
- [What Is the Genetic Algorithm?](https://www.mathworks.com/help/gads/what-is-the-genetic-algorithm.html)
- [Introduction to Genetic Algorithms — Including Example Code](https://towardsdatascience.com/introduction-to-genetic-algorithms-including-example-code-e396e98d8bf3)

## Code
- #CODE [Evotorch](https://github.com/nnaisense/evotorch) - Advanced evolutionary computation library built directly on top of PyTorch
	- https://evotorch.ai/
	- Various evolutionary computation algorithms are available in EvoTorch. 
		- Distribution-based search algorithms: PGPE - Policy Gradients with Parameter-based Exploration, XNES - Exponential Natural Evolution Strategies, CMA-ES - Covariance Matrix Adaptation Evolution Strategies, SNES - Separable Natural Evolution Strategies, CEM - Cross Entropy Method
		- Population-based search algorithms: GeneticAlgorithm - A genetic algorithm implementation. Also supports multiple objectives, in which case it behaves like NSGA-II, CoSyNE - Cooperative Synapse Neuroevolution, MAPElites - Multi-dimensional Archive of Phenotypic Elites
- #CODE [DEAP](https://github.com/DEAP/deap) - Distributed Evolutionary Algorithms in Python
	- http://deap.readthedocs.org/
- #CODE [geneticalgorithm](https://github.com/rmsolgi/geneticalgorithm)