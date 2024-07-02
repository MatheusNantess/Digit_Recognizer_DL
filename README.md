# Handwritten Digit Recognition with Convolutional Neural Networks

## Overview

This project aims to recognize handwritten digits using Convolutional Neural Networks (CNNs). The model was trained on the well-known MNIST dataset and achieved a significant position of 570 in a Kaggle competition. The project involves data preprocessing, model building, training, and evaluation.

## Table of Contents

- [Installation](#installation)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

To get started with this project, clone the repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/handwritten-digit-recognition.git
cd handwritten-digit-recognition
pip install -r requirements.txt

Dataset
The dataset used for this project is the MNIST dataset, which contains 60,000 training images and 10,000 testing images of handwritten digits (0-9). Each image is 28x28 pixels.

Model Architecture
The model is built using PyTorch and consists of multiple convolutional layers followed by fully connected layers. Dropout layers are used to prevent overfitting.

- Conv Block 1: Conv2D -> ReLU -> MaxPool -> Dropout
- Conv Block 2: Conv2D -> ReLU -> MaxPool -> Dropout
- Conv Block 3: Conv2D -> ReLU -> Conv2D -> ReLU -> MaxPool
- Fully Connected: Flatten -> Linear -> ReLU -> Dropout -> Linear

Training
The training script trains the CNN model on the MNIST dataset. The model is trained for a specified number of epochs with Adam optimizer and Cross-Entropy Loss function.

Evaluation
After training, the model's performance is evaluated on the test set to calculate the accuracy and other metrics.

Results
The model achieved an accuracy of XX% on the test set and secured the 570th position in a Kaggle competition.

