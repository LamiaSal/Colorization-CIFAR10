# Colorization-CIFAR10

This github presents the MALIS project made by Weiheng Xia and Lamia Salhi at Eurecom. This project is about image colorization by implementing Multilayer Perceptron and an Autoencoder based on MLP.

The database used is CIFAR10 and the code is implemented in python on jupyther Notebook. We used PyTorch framework. Thus to run this code you'll have to import CIFAR10 database yourself and change the path to the your imported database at the beginning of each jupyternotebook.

You can find a more detailed report on the tests we ran. Here is a small summary to what you'll find in this repository:

## Summary
- MLP_v1v2v3: in this directory you'll find 3 versions MLP:
  - version 1: MLP with one hidden layer
  - version 2: MLP with 2 hidden layers
  - version 3: MLP with 3 hidden layers
 
- CIFAR10-AE-MLP: in this directory you'll find different kind of tests made on Autoencoder based on MLP. In particular, you'll find:
  - a sanity check on a one hidden layer AE MLP (ie: the model is trained on one batch (16 images only) with learning rate= 0.0005
  - one hidden layer AE MLP trained on 5000 images with learning rate= 0.0005
  - one hidden layer AE MLP trained on the whole training dataset with learning rate= 0.0005
  - one hidden layer AE MLP trained on 5000 images with learning rate= 0.0002
  - and finally differrent version of the previous of this last document with more layer

You'll find the results of some tests:
- BatchNormalization_tests (test on one hidden layer MLP with L2 normalization and Batch Normalization)
- Activation_Functions_tests (test on one hidden layer MLP with sigmoid, tanh, ReLU functions)
- Last_layer_activation_func ( test on one hidden layer MLP with sigmoid for the hidden layer and sigmoid, tanh and ReLU functions after the output layer)
- no_activation_funcitons( test on one hidden layer MLP with no activation function)


- First_attempt_mlp: in this directory you'll find our first implementation of MLP but without activation function you'll also find some draft of our first attempts
- Self_implemented_MLP: in this directory you'll find a self implemented MLP with a backpropagation function and a feedforward function without Pytorch)


NB: Except for "First_attempt_mlp" and "Self_implemented_MLP" directories, you'll always find 3 elements in each subdirectory:
 - the Jupyter notebook with a checkpoint
 - a directory inference in which you'll find some exmamples of test, validation and training images outputs
 - a Loss_curve.png file where you'll find the graph of the training and validation loss per epoch.
