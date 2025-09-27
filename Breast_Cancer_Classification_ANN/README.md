Project Overview:

This project implements an Artificial Neural Network (ANN) to predict whether a breast tumor is malignant or benign using the Breast Cancer Wisconsin dataset. The goal is to demonstrate how ANN can be applied to real-world medical data for classification tasks.


Dataset:

Source: sklearn.datasets.load_breast_cancer()

Samples: 569 tumor records

Features: 30 numeric attributes (e.g radius, texture, smoothness)

Target: Binary classification

0 → Malignant

1 → Benign


Preprocessing:

Train Test Split: 80% training, 20% testing

Feature Scaling: StandardScaler to normalize feature values

Labels: Kept as 0/1 (no scaling)

| Layer          | Neurons | Activation |
| -------------- | ------- | ---------- |
| Input          | 30      | -          |
| Hidden Layer 1 | 16      | ReLU       |
| Hidden Layer 2 | 8       | ReLU       |
| Output Layer   | 1       | Sigmoid    |

Optimizer: Adam

Loss Function: Binary Crossentropy

Metrics: Accuracy


Training:

Epochs: 20

Batch Size: 16

Validation Split: 10% of training data

The model typically achieves ~97–99% test accuracy.
