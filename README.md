# MNIST
# MNIST Handwritten Digit Classification using CNN

## Project Overview

This project focuses on handwritten digit classification using a Convolutional Neural Network (CNN) implemented with PyTorch.
The model was trained and evaluated on the MNIST dataset, which is one of the most popular benchmark datasets in Deep Learning and Computer Vision.

The project demonstrates the complete Deep Learning workflow including:

* Data preprocessing
* Building a CNN architecture
* Model training
* Performance evaluation
* Optimizer comparison

---

# Dataset

The project uses the MNIST dataset, which contains grayscale images of handwritten digits from 0 to 9.

Dataset details:

* 60,000 training images
* 10,000 testing images
* Image size: 28 × 28 pixels
* Number of classes: 10

---

# Data Preprocessing

Several preprocessing techniques were applied before training:

* Converting images into tensors using `ToTensor()`
* Normalizing pixel values using `Normalize()`
* Loading data using PyTorch `DataLoader`

---

# Model Architecture

A Convolutional Neural Network (CNN) was implemented for image classification.

The architecture includes:

* Convolutional Layers for feature extraction
* ReLU activation function
* MaxPooling layers for dimensionality reduction
* Dropout layer to reduce overfitting
* Fully Connected layers for classification

Model Flow:

Input Image
→ Convolution Layer
→ ReLU
→ MaxPooling
→ Convolution Layer
→ ReLU
→ MaxPooling
→ Flatten
→ Fully Connected Layer
→ Output Layer

---

# Training

The model was trained using:

* CrossEntropyLoss as the loss function
* Multiple epochs for learning
* GPU acceleration when available

Two different optimizers were tested:

1. Adam Optimizer
2. SGD Optimizer

---

# Experiments and Results

| Optimizer | Test Accuracy |
| --------- | ------------- |
| Adam      | 99.15%        |
| SGD       | 99.05%        |

---

# Performance Analysis

Both optimizers achieved excellent performance on the MNIST dataset.

Observations:

* Adam achieved slightly higher accuracy
* SGD also produced very strong results
* The difference between both optimizers was very small because MNIST is considered a relatively simple dataset

---

# Technologies Used

* Python
* PyTorch
* Torchvision
* Matplotlib

---

# Conclusion

This project successfully demonstrated how CNNs can achieve very high accuracy in handwritten digit classification tasks.

The implemented model achieved more than 99% testing accuracy, showing the effectiveness of Convolutional Neural Networks for image recognition problems.
