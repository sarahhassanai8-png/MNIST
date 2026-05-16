# 🧠 MNIST Handwritten Digit Classification using CNN

## 📌 Project Overview

This project focuses on handwritten digit classification using a Convolutional Neural Network (CNN) implemented with PyTorch.

The model was trained and evaluated on the famous MNIST dataset, one of the most widely used benchmark datasets in Deep Learning and Computer Vision.

The project demonstrates the full Deep Learning pipeline including:

- Data preprocessing
- CNN model design
- Model training and validation
- Performance evaluation
- Optimizer comparison

---

# 📂 Dataset

The project uses the MNIST Handwritten Digits Dataset.

Dataset Details:

| Property | Value |
|---|---|
| Training Images | 60,000 |
| Testing Images | 10,000 |
| Image Size | 28 × 28 Pixels |
| Image Type | Grayscale |
| Number of Classes | 10 Digits (0–9) |

---

# ⚙️ Data Preprocessing

Before training, several preprocessing techniques were applied:

- Converting images into tensors using ToTensor()
- Normalizing pixel values using Normalize()
- Loading data using DataLoader

### Applied Transformations
transforms.Compose([
    transforms.ToTensor(),
    transforms.Normalize((0.5,), (0.5,))
])

---

# 🧠 CNN Model Architecture

A Convolutional Neural Network (CNN) was implemented for image classification.

The architecture includes:

- Convolutional Layers for feature extraction
- ReLU activation function
- MaxPooling layers for dimensionality reduction
- Batch Normalization
- Dropout layer to reduce overfitting
- Fully Connected layers for classification

---

# 🔄 Model Flow
Input Image
   ↓
Convolution Layer
   ↓
ReLU Activation
   ↓
MaxPooling
   ↓
Convolution Layer
   ↓
ReLU Activation
   ↓
MaxPooling
   ↓
Flatten
   ↓
Fully Connected Layer
   ↓
Output Layer

---

# 🚀 Training

The model was trained using:

| Parameter | Value |
|---|---|
| Loss Function | CrossEntropyLoss |
| Batch Size | 64 |
| Epochs | 5 |
| Learning Rate | 0.001 |
| Device | CPU / GPU |

---

# 🔥 Optimizers Used

Two different optimizers were tested and compared:

1. Adam Optimizer
2. SGD Optimizer

---

# 📊 Experiments and Results

| Optimizer | Test Accuracy |
|---|---|
| Adam | 99.24% |
| SGD | 99.24% |

---

# 📈 Performance Analysis

Both optimizers achieved excellent performance on the MNIST dataset.

### Observations

- Adam achieved very fast convergence during training
- SGD also produced strong and stable results
- Both optimizers achieved over 99% accuracy
- MNIST is considered a relatively simple dataset for CNN models

---

# 🛠️ Technologies Used

- Python
- PyTorch
- Torchvision
- Matplotlib
- NumPy

---

# 📉 Visualizations

The project includes visualizations for:

- Training Loss
- Validation Loss
- Training Accuracy
- Validation Accuracy

These graphs help analyze the learning performance of the model during training.

---

# ▶️ How to Run the Project

## 1️⃣ Install Dependencies
pip install torch torchvision matplotlib numpy

## 2️⃣ Open Jupyter Notebook
jupyter notebook

## 3️⃣ Run the Notebook

Open and run:
deep mnist.ipynb

---

# 📁 Project Structure
├── deep mnist.ipynb
├── data/
├── README.md
└── images/

---

# 🎯 Conclusion

This project successfully demonstrated how Convolutional Neural Networks (CNNs) can achieve very high accuracy in handwritten digit classification tasks.

The implemented model achieved more than 99% testing accuracy, showing the effectiveness of CNNs in image recognition and computer vision applications.

