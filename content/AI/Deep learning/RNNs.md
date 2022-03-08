---
title: "Recurrent Neural Networks (RNNs)"
disableToc: false 
---

## Resources
- https://en.wikipedia.org/wiki/Recurrent_neural_network
- https://github.com/kjw0612/awesome-rnn
- Recurrent Neural Networks cheatsheet: https://stanford.edu/~shervine/teaching/cs-230/cheatsheet-recurrent-neural-networks
- Tensorflow, DL and RNNs without a PhD: https://docs.google.com/presentation/d/e/2PACX-1vRouwj_3cYsmLrNNI3Uq5gv5-hYp_QFdeoan2GlxKgIZRSejozruAbVV0IMXBoPsINB7Jw92vJo2EAM/pub?slide=id.p
- http://www.wildml.com/2015/09/recurrent-neural-networks-tutorial-part-1-introduction-to-rnns/
- http://www.abigailsee.com/2017/04/16/taming-rnns-for-better-summarization.html
- http://karpathy.github.io/2015/05/21/rnn-effectiveness/
- http://www.kdnuggets.com/2017/04/build-recurrent-neural-network-tensorflow.html
- https://towardsdatascience.com/the-fall-of-rnn-lstm-2d1594c74ce0
- https://www.kaggle.com/thebrownviking20/intro-to-recurrent-neural-networks-lstm-gru
- https://towardsdatascience.com/illustrated-guide-to-lstms-and-gru-s-a-step-by-step-explanation-44e9eb85bf21
- 4 Sequence Encoding Blocks You Must Know Besides RNN/LSTM in Tensorflow: https://hanxiao.github.io/2018/06/24/4-Encoding-Blocks-You-Need-to-Know-Besides-LSTM-RNN-in-Tensorflow/
- When Recurrent Models Don't Need to be Recurrent (recurrent vs feed-forward models): http://www.offconvex.org/2018/07/27/approximating-recurrent/


## References
- #PAPER Neural Turing Machines (Graves 2014): http://arxiv.org/abs/1410.5401
- #PAPER Attention and Augmented Recurrent Neural Networks (Olah 2016): http://distill.pub/2016/augmented-rnns/
- #PAPER Engineering Extreme Event Forecasting at Uber with Recurrent Neural Networks (Laptev 2017): https://eng.uber.com/neural-networks/
- #PAPER Deep and Confident Prediction for Time Series at Uber (Zhu 2017): https://arxiv.org/abs/1709.01907
	- https://eng.uber.com/neural-networks-uncertainty-estimation/ 
	- introduced a new end-to-end Bayesian neural network (BNN) architecture that more accurately forecasts time series predictions and uncertainty estimations at scale
- #PAPER Neural Machine Translation by Jointly Learning to Align and Translate (Bahdanau 2016): https://arxiv.org/abs/1409.0473
	- https://medium.com/datadriveninvestor/attention-in-rnns-321fbcd64f05
	

### Long Short-Term Memory (LSTM)
- https://en.wikipedia.org/wiki/Long_short-term_memory
- One of the most innovative works in the NLP space is LSTMs and their variations e.g. GRU 
- With a basic RNN cell, we see a massive drop in performance when it comes to long sequences and the network needs to remember patterns which have occurred way at the beginning to infer things correctly at a current time step. And this is because of exploding and vanishing gradients.
- Then came Sepp Hochreiter and Jürgen Schmidhuber and invented LSTMs, which can remember information from the way past and also selectively forget stuff that is not required.
- There are several architectures of LSTM units. A common architecture is composed of a cell (the memory part of the LSTM unit) and three "regulators", usually called gates, of the flow of information inside the LSTM unit: an input gate, an output gate and a forget gate. Some variations of the LSTM unit do not have one or more of these gates or maybe have other gates (for instance, GRUs do not have an output gate).
- The Forget gate decides what is relevant to keep from prior steps. The input gate decides what information is relevant to add from the current step. The output gate determines what the next hidden state should be.
- http://colah.github.io/posts/2015-08-Understanding-LSTMs/
- http://machinelearningmastery.com/tune-lstm-hyperparameters-keras-time-series-forecasting/
- http://machinelearningmastery.com/use-features-lstm-networks-time-series-forecasting/
- http://blog.echen.me/2017/05/30/exploring-lstms/
- https://hackernoon.com/understanding-architecture-of-lstm-cell-from-scratch-with-code-8da40f0b71f4
- https://rubikscode.net/2018/03/19/understanding-long-short-term-memory-networks-lstms/
- https://eli.thegreenplace.net/2018/minimal-character-based-lstm-implementation/

- #PAPER Long Short-Term Memory (Hochreiter 1997): https://dl.acm.org/doi/10.1162/neco.1997.9.8.1735
- #PAPER IndyLSTMs: Independently Recurrent LSTMs (Gonnet 2019): https://arxiv.org/abs/1903.08023
	- Independently Recurrent Long Short-term Memory cells (IndyLSTMs) differ from regular LSTM cells in that the recurrent weights are not modeled as a full matrix, but as a diagonal matrix, i.e.\ the output and state of each LSTM cell depends on the inputs and its own output/state, as opposed to the input and the outputs/states of all the cells in the layer. The number of parameters per IndyLSTM layer, and thus the number of FLOPS per evaluation, is linear in the number of nodes in the layer, as opposed to quadratic for regular LSTM layers, resulting in potentially both smaller and faster models. IndyLSTMs, despite their smaller size, consistently outperform regular LSTMs both in terms of accuracy per parameter, and in best accuracy overall. We attribute this improved performance to the IndyLSTMs being less prone to overfitting.
- #PAPER Understanding LSTM -- a tutorial into Long Short-Term Memory Recurrent Neural Networks (Staudemeyer 2019): https://arxiv.org/abs/1909.09586


### Gated recurrent units (GRU): 
- https://en.wikipedia.org/wiki/Gated_recurrent_unit 
- https://towardsdatascience.com/understanding-gru-networks-2ef37df6c9be
- GRU (Gated Recurrent Unit) aims to solve the vanishing gradient problem which comes with a standard recurrent neural network. GRU can also be considered as a variation on the LSTM. GRU’s got rid of the cell state and used the hidden state to transfer information. It also only has two gates, a reset gate and update gate. 
- The update gate acts similar to the forget and input gate of an LSTM. It decides what information to throw away and what new information to add.
- The reset gate is another gate is used to decide how much past information to forget.
	

### Reservoir computing
- https://en.wikipedia.org/wiki/Reservoir_computing
- Reservoir computing is a framework for computation derived from recurrent neural network theory that maps input signals into higher dimensional computational spaces through the dynamics of a fixed, non-linear system called a reservoir. After the input signal is fed into the reservoir, which is treated as a "black box," a simple readout mechanism is trained to read the state of the reservoir and map it to the desired output.

#### Echo state networks (ESN)
- https://en.wikipedia.org/wiki/Echo_state_network
- The ESN is a recurrent neural network with a sparsely connected hidden layer (with typically 1% connectivity)

- #PAPER Harnessing nonlinearity: predicting chaotic systems and saving energy in wireless communication (Jaeger 2004): https://pubmed.ncbi.nlm.nih.gov/15064413/
	- #CODE https://github.com/cknd/pyESN
- #PAPER Design of deep echo state networks (Gallicchio 2018): https://www.sciencedirect.com/science/article/pii/S0893608018302223
	- #CODE https://github.com/lucapedrelli/DeepESN
- #PAPER Using Machine Learning to Replicate Chaotic Attractors and Calculate Lyapunov Exponents from Data (Pathak 2017): https://arxiv.org/abs/1710.07313
- #PAPER Model-Free Prediction of Large Spatiotemporally Chaotic Systems from Data: A Reservoir Computing Approach (Pathak 2018): https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.120.024102
- #PAPER Wind Power Forecasting Based on Echo State Networks and Long Short-Term Memory (Lopez 2018): https://www.mdpi.com/1996-1073/11/3/526/htm
	- ESN + LSTM
- #PAPER Comparison between DeepESNs and gatedRNNs on multivariate time-series prediction (Gallicchio 2019): https://arxiv.org/abs/1812.11527
- #PAPER Deep Echo State Network (DeepESN): A Brief Survey (Gallicchio 2020): https://arxiv.org/abs/1812.11527	
- #PAPER Comparison of Recurrent Neural Networks for Wind Power Forecasting (Lopez 2020): https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7297597/#CR12
	- ESN + LSTM







