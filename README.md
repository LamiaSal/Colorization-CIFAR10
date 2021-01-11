# Colorization-CIFAR10

This github presents the MALIS project made by Weiheng Xia and Lamia Salhi at Eurecom. This project is about image colorization by implementing Multilayer Perceptron and an Autoencoder based on MLP.

The database used is CIFAR10 and the code is implemented in python on jupyther Notebook. We used PyTorch framework. Thus to run this code you'll have to import CIFAR10 database yourself and change the path to the your imported database at the beginning of each jupyternotebook.

You can find a more detailed report on the tests we ran. Here is a small summary to what you'll find in this repository:

## Summary

- CIFAR10-AE-MLP: in this directory you'll find different kind of tests made on Auto encoder based on MLP. In particular, you'll find:
  - a sanity check on a one hidden layer AE MLP (ie: the model is trained on one batch (16 images only) with learning rate= 0.0005
  - one hidden layer AE MLP trained on 5000 images with learning rate= 0.0005
  - one hidden layer AE MLP trained on the whole training dataset with learning rate= 0.0005
  - one hidden layer AE MLP trained on 5000 images with learning rate= 0.0002
  - and finally differrent version of the previousof this last document with more layers


You'll find the results of some tests:
- Regularization_tests (test on one hidden layer MLP with L2 normalization and Batch Normalization)
- Activation_Functions_tests (test on one hidden layer MLP with sigmoid, tanh, ReLU functions)
