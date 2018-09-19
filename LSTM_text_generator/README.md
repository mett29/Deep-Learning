## LSTM Text Generator

### About this notebook
I wrote this network following some tutorials to put in practice the theory behind the RNNs and LSTMs in particular.
I trained the network using [**Google Colab**](https://colab.research.google.com) for 40 epochs, so not too much, indeed the results are not the best, but at least the chars are combined in the right way.

### Recurrent Neural Network

![rnn](http://www.wildml.com/wp-content/uploads/2015/09/rnn.jpg)

A recurrent neural network (*RNN*) is a class of artificial neural network where connections between units form a directed graph along a sequence. This allows it to exhibit dynamic temporal behavior for a time sequence.

### When you should use a RNN
- NLP, like translation, sentiment analysis, summarization and more
- Sequential data, like stock prices, time series, music ecc.
- Get a caption of an image giving an image as input, and viceversa

### The problem of RNNs
Well, RNNs are one of the most powerful model out there, but of course, it has some limits. The biggest problem is the ***vanishing/exploding gradient***. In fact, if you want to run a RNN on long sequences, you have to run it over many time steps and this means a very deep network.
So the training time could be very very looong. But there's another problem: when the data goes through the network, they are transformated more and more, and as you can image, after a while there will be no trace of the first input.

### The solution: LSTM
Fortunately, in 1997, *Sepp Hochreiter and Jurgen Schmidhuber* proposed the ***Long Short-Term Memory***.

![lstm](https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/Long_Short-Term_Memory.svg/1594px-Long_Short-Term_Memory.svg.png)

I won't go into details (for now), but in short...
*"an LSTM can learn to recognize an important input (that's the role of the input gate), store it in the long-term state, learn to preserve it for as long as it is needed (that's the role of the forget state), and learn to extract it when it is needed."* **(from Hands-On Machine Learning with Scikit-Learn and TensorFlow, by Aurélien Géron)**. 

### References
- [Wikipedia](https://en.wikipedia.org/wiki/Recurrent_neural_network)
- [Hands-On Machine Learning with Scikit-Learn and TensorFlow book](http://shop.oreilly.com/product/0636920052289.do)
- [Understanding LSTMs](http://colah.github.io/posts/2015-08-Understanding-LSTMs/)