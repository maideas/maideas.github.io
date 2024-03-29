---
tags: neural-network,activation-functions,loss-functions,optimizer,optimizer-algorithms,derivatives,convolution,pooling,relu,leakyrelu,softmax
---

# Neural Network Components

>Neural networks are made of connected layers of [Artificial Neurons](artificial_neuron.md).

These layers of neurons are coupled by weighted connections which are adjusted during the learning process in a way to minimize the prediction error of the network, using error gradient [Backpropagation](https://en.wikipedia.org/wiki/Backpropagation), an optimization method, that has been published in 1986 by [Geoffrey Hinton](https://en.wikipedia.org/wiki/Geoffrey_Hinton) et. al.

A good way to build neural networks is to define the following basic elements, which make it easy to create neural networks of different structure and arbitrary complexity:

## Connect layer 

>Implement sums of weighted connections.

- [Dense connected layer](dense_connected_layer.md)
- [Convolution layer](convolutional_networks.md)
- [UpConvolution layer](autoencoder.md)
- Pooling layer

## Function layer

>Implement neuron activation functions.

- [Linear](https://github.com/maideas/numpy-neural-network/blob/master/Linear.ipynb)
- [ReLU](https://github.com/maideas/numpy-neural-network/blob/master/ReLU.ipynb)
- [LeakyReLU](https://github.com/maideas/numpy-neural-network/blob/master/LeakyReLU.ipynb)
- [Tanh](https://github.com/maideas/numpy-neural-network/blob/master/Tanh.ipynb)
- [Sigmoid](https://github.com/maideas/numpy-neural-network/blob/master/Sigmoid.ipynb)
- [Swish](https://github.com/maideas/numpy-neural-network/blob/master/Swish.ipynb)
- [Softplus](https://github.com/maideas/numpy-neural-network/blob/master/Softplus.ipynb)
- [Softmax](classification_basics.md)

## Loss layer

>Implement error loss functions.

- [RMS loss](single_layer_regression.md) (= L2 Norm loss)
- L1 Norm loss
- [Cross Entropy loss](classification_basics.md)
- [Binary Cross Entropy loss](classification_basics.md)
- [Kullback-Leibler loss](variational_autoencoder.md)

## Complex layer

- Sequential layer
- [Inception layer](inception_classification.md)
- Latent and Sample layer
- [LSTM layer](long_short_term_memory.md)
- GRU layer

## Optimizer

>Adjust the network parameters during learning.

- [An excellent overview by Sebastian Ruder](http://ruder.io/optimizing-gradient-descent/)
- Stochastic gradient descent
- RMSprop
- Adagrad
- Adadelta
- Adam

