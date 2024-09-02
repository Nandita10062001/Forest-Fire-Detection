# Forest Fire Detection for Carbon Offset Evaluation

## Overview

This project aims to detect forest fires using image classification techniques, which can play a crucial role in evaluating carbon offset projects and supporting sustainability causes. By accurately detecting and preventing forest fires, we can better manage forest ecosystems, which are vital carbon sinks, and ensure the integrity of carbon offset projects. The project leverages a dataset containing images labeled as either "fire" or "nofire" and implements two neural network architectures: a simple Convolutional Neural Network (CNN) with an accuracy of 93%, and a fully connected neural network (FCNN) that achieved an accuracy of 95%.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architectures](#model-architectures)
  - [Convolutional Neural Network (CNN)](#convolutional-neural-network-cnn)
  - [Fully Connected Neural Network (FCNN)](#fully-connected-neural-network-fcnn)
- [Results](#results)
- [Impact on Carbon Offset and Sustainability](#impact-on-carbon-offset-and-sustainability)
- [Installation](#installation)

## Introduction

Forest fires not only threaten wildlife and human lives but also significantly impact the environment by releasing stored carbon into the atmosphere. Effective detection and management of forest fires are essential for protecting forest ecosystems, which are vital for carbon sequestration. In this project, we developed machine learning models to detect the presence of fire in images, helping to maintain the health of forests and support sustainability initiatives.

## Dataset

The dataset used in this project consists of images categorized into two classes:
- **Fire**: Images containing visible fire.
- **Nofire**: Images without any visible fire.

These images were preprocessed and resized to a consistent format suitable for input into the neural networks.

## Model Architectures

### Convolutional Neural Network (CNN)

The CNN model was designed with the following architecture:
- **Input Layer**: Accepts images of size 256x256x3.
- **Convolutional Layers**: Multiple layers with `ReLU` activation and `MaxPooling`.
- **Fully Connected Layer**: Flattened output of convolutional layers connected to dense layers.
- **Output Layer**: A softmax layer with 2 neurons for binary classification (fire/nofire).

**Accuracy**: 93%

### Fully Connected Neural Network (FCNN)

The FCNN model was built with a deeper architecture:
- **Input Layer**: Accepts flattened image vectors.
- **Hidden Layers**: Multiple dense layers with `ReLU` activation and dropout for regularization.
- **Output Layer**: A softmax layer with 2 neurons for binary classification (fire/nofire).

**Accuracy**: 95%

## Results

- **CNN Model**: Achieved an accuracy of 93% on the test set.
- **FCNN Model**: Achieved an accuracy of 95% on the test set.

Both models were evaluated using various performance metrics, including accuracy, precision, recall, and F1-score.
![Fire [0]](output1.png) 
![NoFire [1]](output2.png)

*Figure 1: Fire example image from the dataset.*      
*Figure 2: NoFire example image from the dataset.*

## Impact on Carbon Offset and Sustainability

### Evaluating Carbon Offset Projects

Accurate forest fire detection is essential for evaluating the effectiveness of carbon offset projects, which often rely on preserving forest areas to absorb CO2 from the atmosphere. By detecting and mitigating fires early, we can protect these critical carbon sinks, ensuring that carbon offset goals are met and that carbon credits remain valid.

### Supporting Sustainability Causes

Forest ecosystems are crucial for biodiversity and climate regulation. Early fire detection helps maintain the ecological balance and supports sustainability efforts by reducing the risk of large-scale forest degradation. This project contributes to sustainability by providing a tool that can be integrated into broader environmental monitoring systems, aiding in the protection of natural resources.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/forest-fire-detection.git
