---
title: "Gated Recurrent Units (GRUs)"
---

## Resources
- GRUs are a gating mechanism in recurrent neural networks
- https://en.wikipedia.org/wiki/Gated_recurrent_unit 
- https://towardsdatascience.com/understanding-gru-networks-2ef37df6c9be
- GRU (Gated Recurrent Unit) aims to solve the vanishing gradient problem which comes with a standard recurrent neural network. GRU can also be considered as a variation on the LSTM. GRU’s got rid of the cell state and used the hidden state to transfer information. It also only has two gates, a reset gate and update gate. 
- The update gate acts similar to the forget and input gate of an LSTM. It decides what information to throw away and what new information to add.
- The reset gate is another gate is used to decide how much past information to forget.

## References
- #PAPER [Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation (Cho 2014)](https://arxiv.org/abs/1406.1078v3)
- #PAPER [On the Properties of Neural Machine Translation: Encoder-Decoder Approaches (Cho 2014)](https://arxiv.org/abs/1409.1259)


