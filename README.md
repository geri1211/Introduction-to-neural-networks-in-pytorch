
# Introduction to Neural Networks in PyTorch

This repository contains the hands-on lab notebooks and final project I completed during my course on the fundamentals of neural networks with PyTorch.



## About the Course

The course builds up from the basics of PyTorch to training real models. Each lab is a Jupyter notebook where I wrote and ran the code myself. The notebooks are numbered by module and lesson, so they can be followed in order.

## What I Did

**Module 1: PyTorch basics.** I started with tensors, the core data structure in PyTorch, working with one-dimensional and two-dimensional tensors and the operations on them. I learned how PyTorch computes derivatives automatically and how it represents computations as graphs. I also built simple custom datasets, applied transformations to them, and used PyTorch's pre-built datasets.

**Module 2: Linear regression.** I made predictions with a one-dimensional linear regression model and learned how to train its slope and bias by minimizing a loss function.

**Module 3: Gradient descent.** I trained models with stochastic gradient descent and mini-batch gradient descent and compared how they behave. I then rebuilt the same models "the PyTorch way" using the built-in `nn.Module`, loss functions and optimizers. I also used training and validation data to choose a good learning rate.

**Module 4: Multiple linear regression.** I extended linear regression to several inputs and several outputs, first making predictions and then training the models.

**Module 5: Logistic regression.** I moved from regression to classification. I made predictions with logistic regression, saw how a bad choice of initial values can hurt a model when using the wrong loss function, and then trained with cross-entropy loss, which works much better.

**Final project: League of Legends Match Predictor.** I applied everything to a real-world problem: building a logistic regression model in PyTorch to predict the outcome of League of Legends matches. The project covered loading and preparing the data, defining and training the model, adding L2 regularization (weight decay) to reduce overfitting, and evaluating the results with a confusion matrix and ROC curve.

## What I Learned

- How tensors work and how to manipulate them in PyTorch
- How automatic differentiation and gradients drive the training of a model
- How to build custom datasets and apply transformations
- How gradient descent works, and the differences between stochastic, mini-batch and batch training
- How to build models with `nn.Module` and train them with PyTorch's built-in loss functions and optimizers
- How to use validation data to choose hyperparameters such as the learning rate
- How to extend linear regression to multiple inputs and multiple outputs
- How logistic regression works for classification, and why cross-entropy is a better loss than mean squared error here
- How to reduce overfitting with regularization and evaluate a classifier with a confusion matrix and ROC curve

## Tech Stack

Python, PyTorch, NumPy, pandas, scikit-learn, Matplotlib and Jupyter Notebook.

## Using This Repository

The notebooks are named with their module and lesson numbers (for example, `3_2_Mini-Batch_Gradient_Descent`), so they appear in course order. Each one is self-contained and can be opened and run in Jupyter. A few notebooks, mainly the gradient descent labs, contain many saved plots and may be slow to load on GitHub.

## Acknowledgments

These notebooks are lab exercises from a course on the IBM Skills Network platform. The lab content, datasets and original instructions belong to their respective authors and to IBM. I'm sharing this repository as a record of my own learning and progress.
