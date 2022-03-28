---
title: "Long Short-Term Memory networks (LSTMs)"
disableToc: false 
---

## Resources
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


## References
- #PAPER [Long Short-Term Memory (Hochreiter 1997)](https://dl.acm.org/doi/10.1162/neco.1997.9.8.1735)
- #PAPER [IndyLSTMs: Independently Recurrent LSTMs (Gonnet 2019)](https://arxiv.org/abs/1903.08023)
	- Independently Recurrent Long Short-term Memory cells (IndyLSTMs) differ from regular LSTM cells in that the recurrent weights are not modeled as a full matrix, but as a diagonal matrix, i.e.\ the output and state of each LSTM cell depends on the inputs and its own output/state, as opposed to the input and the outputs/states of all the cells in the layer. The number of parameters per IndyLSTM layer, and thus the number of FLOPS per evaluation, is linear in the number of nodes in the layer, as opposed to quadratic for regular LSTM layers, resulting in potentially both smaller and faster models. IndyLSTMs, despite their smaller size, consistently outperform regular LSTMs both in terms of accuracy per parameter, and in best accuracy overall. We attribute this improved performance to the IndyLSTMs being less prone to overfitting.
- #PAPER [Understanding LSTM -- a tutorial into Long Short-Term Memory Recurrent Neural Networks (Staudemeyer 2019)](https://arxiv.org/abs/1909.09586)

