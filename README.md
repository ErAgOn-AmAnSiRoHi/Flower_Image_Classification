﻿# Flower Image Classification

## Overview

This project explores various advanced approaches to flower image classification, comparing traditional Convolutional Neural Networks (CNNs) with Bayesian methods and Dynamic Mode Decomposition (DMD) based features. The goal is to demonstrate the strengths and unique characteristics of each approach in the context of image classification tasks.

## Approaches Implemented

1. Standard CNN
2. Bayesian CNN
3. DMD-based Feature Classification
4. Bayesian Neural Network (BNN)
5. Edge Detection using Bayesian CNN

## Dataset

The project uses a flowers dataset containing images of five different types of flowers:
- Daisy
- Dandelion
- Rose
- Sunflower
- Tulip

The dataset consists of 4242 images, with approximately 800 images per flower type.

## Implementation Details

### 1. Standard CNN

- Architecture: 4 convolutional layers followed by flatten and dense layers
- Optimizer: Adam
- Loss Function: Categorical Cross-Entropy
- Metrics: Accuracy

### 2. Bayesian CNN

- Uses TensorFlow Probability library
- First layer: Convolutional2DReparameterization (for aleatoric uncertainty)
- Last layer: DenseReparameterization (for epistemic uncertainty)
- Loss Function: Negative Log-Likelihood
- Incorporates Kullback-Leibler (KL) divergence for regularization

### 3. DMD-based Feature Classification

- Applies Dynamic Mode Decomposition to extract temporal structures from static images
- Features extracted using DMD are used as inputs for classification algorithms

### 4. Bayesian Neural Network (BNN)

- Treats network weights as probability distributions
- Outputs probability distributions over classes instead of single values
- Incorporates prior and posterior distributions over weights
- Loss function includes both classification loss and KL divergence

### 5. Edge Detection using Bayesian CNN

- Integrates Bayesian principles into CNN for edge detection
- Provides uncertainty estimation along with edge detection results

## Results and Observations

- The project demonstrates the ability of Bayesian approaches to quantify uncertainty in predictions
- Bayesian methods show improved performance in scenarios with limited labeled data
- DMD-based features offer a novel approach to capturing temporal structures in static images

## Future Work

- Further exploration of model compression techniques for Bayesian CNNs
- Investigation of computational efficiency and scalability challenges in Bayesian approaches
- Application of these methods to other image classification tasks and datasets

## Dependencies

- TensorFlow
- TensorFlow Probability
- NumPy
- Matplotlib
- split-folders (for dataset preparation)

## Contributors

- Aman Sirohi
- R Sriviswa
- Rakhil ML
- Vikhyat Bansal

## References

[You may refer the last slides of the misprojectppt.pptx]
