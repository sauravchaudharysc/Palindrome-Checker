# Palindrome-Checker
This architecture is designed to process binary inputs through the network, with the hidden layer applying Sigmoid activation to introduce non-linearity, and the output layer using Sigmoid activation to produce a binary classification or prediction.

## Introduction
This repository contains a simple implementation of a Neural Network trained to recognize palindromic binary strings. The model is built using NumPy and includes functionalities for training, evaluation, and testing.

## Architecture
Our neural network architecture consists of: 

- [**Input layer:**](#Input-layer) 10 neurons, each representing a 1-bit binary number. 
- [**Hidden layer:**](#hidden-layer) 2 neurons, utilizing the Sigmoid activation function. 
- [**Output layer:**](#output-layer) 1 neuron, utilizing the Sigmoid activation function. 

## Contents

- [**Model Initialization**](#model-initialization): Describes how the neural network model is initialized.
- [**Model Instantiation**](#model-instantiation): Provides an example of how to instantiate the neural network.
- [**Loading Data**](#loading-data): Demonstrates how the data is loaded and prepared for training.
- [**Training and Evaluation**](#training-and-evaluation): Illustrates how the model is trained and evaluated using k-fold cross-validation.
- [**Loading Saved Model**](#loading-saved-model): Shows how to load a pre-trained model.
- [**Testing**](#testing): Includes a testing section with a confusion matrix and sample predictions.
- [**Evaluation**](#evaluation): Allows users to input a 10-bit binary number and checks if it's a palindrome.

## Requirements

- NumPy
- scikit-learn
- imbalanced-learn
- seaborn
- matplotlib

## Usage

1. Install the required libraries: `pip install numpy scikit-learn imbalanced-learn seaborn matplotlib`.
2. Run the notebook `Palindrome-Assignment1.ipynb` in a Jupyter environment.

## Model Saving and Loading

- The model can be saved using the `save_model` method and loaded using the `load_model` method.

```python
neural_network.save_model("model.pkl")
neural_network.load_model("model.pkl")
```

## Testing Palindromes

- After running the notebook, you can test whether a given 10-bit binary number is a palindrome using the provided evaluation section.
