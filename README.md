# Neural Network for Digit Recognition

This project is a simple implementation of a neural network for digit recognition. The neural network has three hidden layers and uses the ReLU and softmax activation functions.

## Overview

The neural network consists of an input layer, three hidden layers, and an output layer. The input layer takes in a 28x28 pixel image (784 neurons), and the output layer produces a prediction of the digit (10 neurons). The three hidden layers each contain 10 neurons.

The neural network uses the ReLU activation function for the hidden layers and the softmax activation function for the output layer. The parameters of the neural network are initialized randomly and are then updated using gradient descent.

The neural network is trained using a dataset of handwritten digits, and its performance is evaluated based on its accuracy in predicting the correct digit.ˇ

## Code Overview

The code is divided into several functions, each responsible for a specific task in the neural network:

1. `init_params()`: Initializes the weights and biases for the hidden layers of the neural network.

2. `ReLU(Z)`: Computes the ReLU activation function on a given input Z.

3. `softmax(Z)`: Computes the softmax activation function on a given input Z.

4. `forward_prop(W1, b1, W2, b2, W3, b3, X)`: Performs forward propagation through the neural network.

5. `ReLU_deriv(Z)`: Computes the derivative of the ReLU activation function on a given input Z.

6. `one_hot(Y)`: Converts a vector of labels into a one-hot encoding.

7. `backward_prop(Z1, A1, Z2, A2, Z3, A3, W1, W2, W3, X, Y)`: Performs backward propagation through the neural network.

8. `update_params(W1, b1, W2, b2, W3, b3, dW1, db1, dW2, db2, dW3, db3, alpha)`: Updates the parameters of the neural network using gradient descent.

9. `get_predictions(A2)`: Returns the predictions of the neural network.

10. `get_accuracy(predictions, Y)`: Computes the accuracy of a set of predictions.

11. `gradient_descent(X, Y, alpha, iterations)`: Trains the neural network using gradient descent.

## Merits of this Project

1. The code is written from scratch, providing a deep understanding of the inner workings of neural networks.
2. The code is heavily commented, making it easy for beginners to understand.

## Notes

1. This project is an adaptation of the Kaggle tutorial by Samson Zhang. The original tutorial can be found [here](https://www.kaggle.com/code/wwsalmon/simple-mnist-nn-from-scratch-numpy-no-tf-keras/notebook). I followed this tutorial and then further expanded on it by adding an additional hidden layer in the neural network.

2. The code contains extensive comments to explain each step of the process. This is intentional to further my own understanding of the processes while also making it easy for any beginner to follow.

