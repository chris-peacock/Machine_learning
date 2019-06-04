# Machine learning scripts
Here is a directory for the scripts Ive written to explore various concepts in machine learning

## activations

A few activation function, to be called when constructing individual layers of the neural network, in nn_test

## nn_test

Within, a <b>layer</b> class which can be created with a certain number of neurons with randomly initialized weights and constant bias

<b>backprop</b> performs simple regression back-propagation (no momentum; 1st order in taylor expansion) on a many-layered network of arbitrary size and series of activation functions

<b>comp</b> compiles a list of layers as a tuple of layer objects, which can be fed into backprop

I've yet to incorporate a layer-specific bias which gets updated along with the weights in the backprop step.  Because of this, all neurons in the network essentially converge to the same set of weights, and so the output label is simply the average label of the input dataset.  problematic, but solvable with a bit of tweaking to the layer class
