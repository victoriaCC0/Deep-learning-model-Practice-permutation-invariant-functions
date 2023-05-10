# Deep-learning-model-Practice-permutation-invariant-functions
Deep learning model Practice of permutation invariant functions
## permutation invariant functions
Consider the problem of learning a permutation-invariant function  by using a neural network according to the -sum-decomposition neural network architecture defined in the lectures and slides you find in this repository.

For function , use a feedforward neural network with one hidden layer with 100 neurons and ReLU activation function, and the output layer with lat_dim output units. lat_dim is a hyperparameter which you will need to set to values specified below.

For function , use a feedforward neural network with one hidden layer with 100 neurons and ReLU activation function.

For training, use the stochastic gradient descent algorithm with learning rate 1e-4. Use MSE for the loss function. Use a validation dataset by taking 0.1 portion of the training dataset (validation split). Use batch size of value 128.

## permutation equivariant functions
Consider the problem of learning a permutation-equivariant function  by using a feedforward neural network with equivariant layers - see lectures for definition. The function we are going to consider corresponds to a choice function that for each set of input items outputs the choice of one of these items (using one-hot encoding).

We consider a feedforward neural network with L equivariant layers. Each of the first L-1 layers consists of an equivariant affine transformation followed by ReLU activation units with output dimension . The output layer is an equivariant affine transformation with output dimension .

For training, use Adam optimizer with learning rate of value 1e-4 and epsilon set to value 1e-3. For the loss function, use MSE. Use validation split of value 0.1. Use batch size of value 300. Use the number of epochs of value 100.
