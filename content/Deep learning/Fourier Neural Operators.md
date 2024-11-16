---
title: "Fourier Neural Operator (FNO)"
---

## Resources
- [Neural Operator - Machine learning for scientific computing](https://zongyi-li.github.io/neural-operator/)
	- The classical development of neural networks has primarily focused on learning mappings between finite dimensional Euclidean spaces or finite sets. To better approximate the solution operators raised in PDEs, a generalization of neural networks to learn operators mapping between infinite dimensional function spaces is proposed
	- Formulate the approximation of operators by composition of a class of linear integral operators and nonlinear activation functions, so that the composed operator can approximate complex nonlinear operators
	- Such neural operators are resolution-invariant, and consequently more efficient compared to traditional neural networks
	- The FNO model has shown state-of-the-art performance with 1000x speedup in learning turbulent Navier-Stokes equation


## Talks
- #TALK [A crash course on Neural Operators (Kamyar Azizzadenesheli)](https://www.youtube.com/watch?v=KIGG-IA9awU)
- #TALK [Zongyi Li's talk on solving PDEs from data](https://www.youtube.com/watch?v=0Ve9xwNJO2o&t=1197s)
- #TALK [Neural operator: A new paradigm for learning PDEs (Anima Anandkumar)](https://www.youtube.com/watch?v=Bd4KvlmGbY4&t=0s)

## References
- #PAPER [Fourier Neural Operator for Parametric Partial Differential Equations (Li 2020)](https://arxiv.org/abs/2010.08895)
	- #CODE https://github.com/zongyi-li/fourier_neural_operator
	- #CODE https://github.com/astanziola/fourier-neural-operator-flax
	- https://zongyi-li.github.io/blog/2020/fourier-pde/
	- https://www.technologyreview.com/2020/10/30/1011435/ai-fourier-neural-network-cracks-navier-stokes-and-partial-differential-equations/
	- [Paper explained](https://www.youtube.com/watch?v=IaS72aHrJKE)
	- Function approximation in Fourier space instead of a the Euclidian (with conventional convolutions)
	- Fourier representation is more efficient than CNN, it's global and continuous
	- Convolution -> pointwise multiplication (by matrix R, that is learned) in Fourier domain
	- Fourier layer. 
		- Fourier transform. Filtering/truncating low frequency modes
		- Non-linearity (as in other DL models)
		- Linear transform/layer to track location information (just like a residual connection)
	- FNO captures energy spectrum
	- It can do zero-shot super-resolution: trained on a lower resolution directly evaluated on a higher resolution
- #PAPER [MeshfreeFlowNet: A Physics-Constrained Deep Continuous Space-Time Super-Resolution Framework (Jiang 2020)](https://arxiv.org/abs/2005.01463)
	- #TALK [ML Cluster: Karthik Kashinath, Physics-informed Machine learning for weather and climate science](https://www.youtube.com/watch?v=B_4TONeY75U)
	- [[AI/Computer Vision/Super-resolution]]
- #PAPER [Neural Operator: Learning Maps Between Function Spaces (Kovachki 2021)](https://arxiv.org/pdf/2108.08481)
- #PAPER [Adaptive Fourier Neural Operators: Efficient Token Mixers for Transformers (Guibas 2022)](https://arxiv.org/pdf/2111.13587)            
	- #CODE https://github.com/NVlabs/AFNO-transformer
	- #CODE https://github.com/DarshanDeshpande/research-paper-implementations/tree/main/tensorflow/afno (not official)
	- Adaptive FNO (AFNO) - connection between transformers and FNOs
	- Transformers are a special case of neural operators
	- AFNO is efficient for that it splits the grid (efficient token mixing) 
- #PAPER [FourCastNet: A Global Data-driven High-resolution Weather Model using  Adaptive Fourier Neural Operators (2022)](https://arxiv.org/pdf/2202.11214)
	- [FourCastNet - NVIDIA Docs](https://docs.nvidia.com/deeplearning/modulus/modulus-sym/user_guide/neural_operators/fourcastnet.html)
	- #CODE [GitHub - NVlabs/FourCastNet: Initial public release of code, data, and model weights for FourCastNet](https://github.com/NVlabs/FourCastNet)


