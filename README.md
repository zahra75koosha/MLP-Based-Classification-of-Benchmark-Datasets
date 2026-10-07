# MLP Classification Benchmark

A Multi-Layer Perceptron (MLP) implemented with TensorFlow/Keras for classifying three benchmark datasets: Spiral, Aggregation, and Banana.

## Overview

This project explores the use of a feed-forward neural network (MLP) for classification on three datasets with different class structures.

The same general classification approach is applied to:

- Spiral
- Aggregation
- Banana

For each dataset, the data is divided into training and test sets, class labels are converted into one-hot encoded vectors, and an MLP classifier is trained using the Adam optimizer and categorical cross-entropy loss.

## Methodology

The workflow for each dataset consists of:

1. Loading the dataset.
2. Splitting the data into training and test sets using a 70/30 split.
3. Separating input features and class labels.
4. Converting class labels to one-hot encoded vectors.
5. Training an MLP classifier using ReLU hidden layers and a Softmax output layer.
6. Evaluating the trained model on the test set.

## Datasets

### 1. Spiral

The Spiral dataset contains **312 samples**, with two input features (`A`, `B`) and three classes.

The MLP architecture consists of:

```text
Input (2 features)
    ↓
Dense (21, ReLU)
    ↓
Dense (21, ReLU)
    ↓
Dense (3, Softmax)
