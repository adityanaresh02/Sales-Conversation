# MNIST Digit Classifier

This repository contains a PyTorch implementation of a neural network model for classifying handwritten digits from the MNIST dataset. The model is trained on the MNIST training set and evaluated on the MNIST test set. Additionally, a Gradio interface is provided to visualize the model's weights and make predictions on user-uploaded images.

The neural network model consists of two fully connected (dense) layers:

The first layer takes the **28x28** MNIST image as input, flattens it into a **784-dimensional vector**, and applies a **ReLU** activation function.

The second layer takes the output of the first layer and produces a 10-dimensional output vector, representing the probabilities of each digit class(0-9).

The model is trained using the Adam optimizer and cross-entropy loss function. The training loop iterates over the MNIST training set in batches of **100 images**, and the model is updated using backpropagation. The training process is repeated for **5 epochs**.
