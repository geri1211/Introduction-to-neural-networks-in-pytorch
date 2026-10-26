[README (1).md](https://github.com/user-attachments/files/33966794/README.1.md)

# Introduction to Neural Networks in PyTorch

A collection of the hands-on lab notebooks and projects I completed during my course on neural networks with PyTorch. The course starts with tensors and linear regression and builds up step by step to deep neural networks and convolutional neural networks (CNNs), ending with two projects.

> **Course:** _[Add your course name and provider here]_
> **Platform:** IBM Skills Network labs

---

## Table of Contents

1. [Course Overview](#course-overview)
2. [What I Covered](#what-i-covered)
3. [Projects](#projects)
4. [Skills I Gained](#skills-i-gained)
5. [Tech Stack](#tech-stack)
6. [Repository Structure](#repository-structure)
7. [Running the Notebooks](#running-the-notebooks)
8. [Acknowledgments](#acknowledgments)

---

## Course Overview

Each lab is a Jupyter notebook that I worked through and ran myself. The notebooks are numbered by module and lesson (for example, `3_2_Mini-Batch_Gradient_Descent`), so they appear in course order and build on each other. Later labs reuse ideas from earlier ones, so it helps to go through them in sequence.

---

## What I Covered

| Module | Topic | What I did |
|---|---|---|
| 1 | PyTorch basics | Worked with 1D and 2D tensors, computed derivatives with automatic differentiation, and built and transformed datasets |
| 2 | Linear regression | Made predictions with a linear model and trained its slope and bias |
| 3 | Gradient descent | Trained with stochastic and mini-batch gradient descent, built models the PyTorch way, and used validation data to pick a learning rate |
| 4 | Multiple linear regression | Extended regression to multiple inputs and multiple outputs, for both prediction and training |
| 5 | Logistic regression | Moved to classification, saw how bad initialization affects training, and trained with cross-entropy loss |
| 6 | Softmax classification | Classified handwritten digits from the MNIST dataset with a softmax classifier |
| 7 | Neural networks | Built networks with hidden layers, compared activation functions, and solved the XOR problem |
| 8 | Deep neural networks | Trained deeper networks and improved them with dropout, weight initialization, momentum and batch normalization |
| 9 | Convolutional neural networks | Learned convolution, activation and max pooling, multiple channels, and built CNNs on small images and Fashion-MNIST |

### Module details

**Module 1: PyTorch basics.** I started with tensors, the core data structure in PyTorch, and learned how to create and manipulate one-dimensional and two-dimensional tensors. I then looked at how PyTorch calculates derivatives automatically and represents computations as graphs, which is what makes training neural networks possible. I finished by building simple custom datasets, applying transformations to them, and using PyTorch's pre-built datasets.

**Module 2: Linear regression.** I made predictions with a one-dimensional linear regression model and trained it by finding the slope and bias that minimize the loss.

**Module 3: Gradient descent.** I trained models with stochastic gradient descent and mini-batch gradient descent and compared how each one behaves. I then rebuilt the same models "the PyTorch way" using `nn.Module`, built-in loss functions and optimizers, and used training and validation data to select a good learning rate.

**Module 4: Multiple linear regression.** I extended linear regression to handle several inputs and several outputs, working through both making predictions and training the models.

**Module 5: Logistic regression.** I moved from predicting numbers to classifying. I made predictions with logistic regression, saw how a bad starting point can break training when the wrong loss is used, and trained with cross-entropy loss. I also started on softmax for classifying into more than two classes.

**Module 6: Softmax classification.** I used a softmax classifier to recognize handwritten digits in the MNIST dataset.

**Module 7: Neural networks.** I built my first networks with a hidden layer, then added more hidden neurons to see how this improves what the network can learn. I solved the XOR problem, which a single linear model can't, and trained a one-hidden-layer network on MNIST. I also compared the sigmoid, tanh and ReLU activation functions.

**Module 8: Deep neural networks.** I built deeper networks, including multi-class models using `nn.ModuleList`, and learned several techniques to make them train better:
- **Dropout** to reduce overfitting, for both classification and regression
- **Weight initialization**, comparing default, Xavier and He initialization, and seeing why starting every weight at the same value fails
- **Momentum** to speed up and stabilize gradient descent
- **Batch normalization** to make training faster and more stable

**Module 9: Convolutional neural networks.** I learned how convolution works, then added activation functions and max pooling, and worked with multiple input and output channels. I built CNNs step by step: a simple example, then a CNN for small images, then one with batch normalization.

---

## Projects

**Fashion-MNIST Project.** I built and trained a convolutional neural network to classify images of clothing from the Fashion-MNIST dataset, applying the CNN techniques from Module 9.

**Final Project: League of Legends Match Predictor.** I built a logistic regression model in PyTorch to predict the outcome of League of Legends matches from game data. The project covered preparing the data, defining and training the model, adding L2 regularization (weight decay) to reduce overfitting, and evaluating the results with a confusion matrix and ROC curve.

---

## Skills I Gained

- Creating, manipulating and differentiating tensors in PyTorch
- Building custom datasets and applying transformations
- Understanding gradient descent and training models with PyTorch's loss functions and optimizers
- Building models with `nn.Module` and `nn.ModuleList`
- Using validation data to tune hyperparameters
- Regression and classification: linear, logistic and softmax
- Designing neural networks with hidden layers and choosing activation functions
- Improving deep networks with dropout, initialization, momentum and batch normalization
- Building and training convolutional neural networks for image classification
- Evaluating models with accuracy, a confusion matrix and an ROC curve

---

## Tech Stack

Python, PyTorch, torchvision, NumPy, pandas, scikit-learn, Matplotlib and Jupyter Notebook.

---

## Repository Structure

```
.
├── README.md
├── 1_x   PyTorch basics: tensors, derivatives, datasets
├── 2_x   Linear regression
├── 3_x   Gradient descent and training
├── 4_x   Multiple linear regression
├── 5_x   Logistic regression and softmax
├── 6_x   Softmax on MNIST
├── 7_x   Neural networks and activation functions
├── 8_x   Deep networks: dropout, initialization, momentum, batch normalization
├── 9_x   Convolutional neural networks
├── Fashion-MNIST_Project.ipynb
└── Final_Project_League_of_Legends_Match_Predictor.ipynb
```

The prefix of each notebook is its module and lesson number.

---

## Running the Notebooks

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Install the dependencies:
   ```bash
   pip install torch torchvision numpy pandas scikit-learn matplotlib jupyter
   ```
3. Launch Jupyter and open any notebook:
   ```bash
   jupyter notebook
   ```

Some notebooks download datasets such as MNIST the first time they run, so an internet connection is needed. A GPU isn't required for these labs. A few of the gradient descent notebooks contain many saved plots and may be slow to open on GitHub.

---

## Acknowledgments

These notebooks are lab exercises from a course on the IBM Skills Network platform. The lab content, datasets and original instructions belong to their respective authors and to IBM. I'm sharing this repository as a record of my own learning and progress.
