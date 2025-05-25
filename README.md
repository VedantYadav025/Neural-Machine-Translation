This is a project taken from Stanford course, Deep Learning with NLP.

### We do a seq2seq machine translation from Mandarin (Chinese) to English.

### We use a Bi-directional LSTM encoder, and a Uni-directional LSTM decoder. We use attention scores, calculated using multiplicative attention b/w the hidden states of the LSTMs. The attention scores are then passes through a softmax layer, which is then project to calculate the weighted average of the hidden states of encoder. This is then used (along with decoder hidden state) to calculate the final output vector (using a linear layer and dropout for regularization). The output is then passed through a softmax layer to calculate the probability distribution of the target words.

### The BLEU score is 19.84
