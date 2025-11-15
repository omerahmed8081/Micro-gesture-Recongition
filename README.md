# Micro-gesture-Recongition
## Project Overview

This project demonstrates an Enhanced ResNet50 architecture for gesture recognition using PyTorch. It applies transfer learning with additional convolutional layers to classify 32 gesture classes, improving feature extraction and overall accuracy.

## Dataset

The dataset consists of 32 gesture classes organized into subdirectories within the training folder. Each subfolder represents one gesture class. The data is split into training and validation sets with an 80/20 ratio.

## Model Architecture

The model builds upon a pre-trained ResNet50 backbone trained on ImageNet. The final fully connected layer is replaced with an additional convolutional block, batch normalization, ReLU activation, and a global average pooling layer, followed by a custom linear classifier.

## Training

The model is trained using the Adam optimizer and cross-entropy loss. Early stopping is implemented to prevent overfitting. Training and validation accuracy and loss are displayed for each epoch to track progress and convergence.

## Evaluation

Model performance is evaluated using Top-1 and Top-5 accuracy metrics. The model achieves approximately 85% Top-1 and 95% Top-5 accuracy, indicating strong generalization across gesture classes.

## Key Features

Enhanced ResNet50 with improved spatial feature extraction

Full training and validation workflow with early stopping

Top-1 and Top-5 accuracy evaluation

Modular, reproducible structure for easy experimentation
