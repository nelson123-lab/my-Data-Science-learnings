## GRU Cell

A GRU (Gated Recurrent Unit) is a type of recurrent neural network (RNN) architecture that is designed to address some of the limitations of traditional RNNs, such as the vanishing gradient problem and the difficulty of learning long-term dependencies.

- Simplified version of an LSTM Cell
- No Separate output, the whole state is output at every timstep
- The gate controller r decides which part of the previous state will be shown to the main layer.

The key components of a GRU include:

1. Update Gate: Controls how much of the past information needs to be passed along to the future. It decides how much of the previous state should be kept and how much of the new state should be added.
2. Reset Gate: Determines how much of the past information should be forgotten or ignored.
3. Candidate State: The new candidate state that will be added to the memory.
4. Hidden State: The output of the GRU cell, which is a combination of the previous hidden state and the new candidate state.

By using these gates, GRUs are able to learn to selectively update the hidden state based on the input sequence, allowing them to capture long-range dependencies more effectively than traditional RNNs. They have become popular in various sequence modeling tasks, including natural language processing, speech recognition, and time series prediction.

References:
[Fool-proof RNN explanation](https://youtu.be/y9PLF2GsD-c)
