---
tags: python,numpy,neural-network,activation-functions,loss-functions,optimizer,optimizer-algorithms,derivatives,convolution,pooling,relu,leakyrelu,softmax
---
# A NumPy based Neural Network Package Implementation

## Objective

Years ago I studied Microelectronics and Computer Science and had the opportunity to join some Machine Learning lectures.
From this point on, I always followed this topic up to now where Neural Networks and Machine Learning gain a lot of momentum.
My interest in all the things surrounding this field of research and the ever growing amount of available material took me to the decision to - once again - dive deeper into it. To understand all these things down to their details, I think a very good way is to implement all components of a neural network using a nice language called Python and the NumPy library.
The idea was to use the knowledge about neural networks as they were when I studied and combine it with the latest research outcomes regarding new activation functions, new optimizer algorithms and new structures, better suited to solve several problems.
As a side effect I got a better knowledge of Python and NumPy ...

## What is a Neural Network made off ?

>Connected Layers of Neurons

These layers of neurons are coupled by weighted connections which are adjusted during the learning process in a way to minimize the prediction error of the network normally using some sort of error gradient backpropagation.

An easy way to build up a neural network is to define the following types of layers:

- **Connect layer** *(to implement sums of weighted connections)*
  - Fully connected layer
  - Convolutional layer
  - MaxPooling layer

- **Function layer** *(to implement neuron activation functions)*
  - [Linear](https://nbviewer.jupyter.org/github/m-a-h-e/numpy-neural-network/blob/master/Linear.ipynb)
  - [ReLU](https://nbviewer.jupyter.org/github/m-a-h-e/numpy-neural-network/blob/master/ReLU.ipynb)
  - [LeakyReLU](https://nbviewer.jupyter.org/github/m-a-h-e/numpy-neural-network/blob/master/LeakyReLU.ipynb)
  - [Tanh](https://nbviewer.jupyter.org/github/m-a-h-e/numpy-neural-network/blob/master/Tanh.ipynb)
  - [Sigmoid](https://nbviewer.jupyter.org/github/m-a-h-e/numpy-neural-network/blob/master/Sigmoid.ipynb)
  - [Softmax](softmax.md)

- **Loss layer** *(to implement network error loss functions)*
  - RMS loss *(= L2 Norm loss)*
  - L1 Norm loss
  - Cross Entropy loss

To adjust the weights *(parameters)* of the network, an optimization algorithm is needed:

- **Optimizer**
  - [An excellent overview by Sebastian Ruder](http://ruder.io/optimizing-gradient-descent/)
  - Stochastic gradient descent
  - RMSprop
  - Adagrad
  - Adadelta
  - Adam

The Python package - implementing all the above Neural Network components - can be found [here ...](https://github.com/m-a-h-e/numpy-neural-network)