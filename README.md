# 🧠 MNIST Digit Classification using CNN

This project implements a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset using TensorFlow and Keras. The notebook includes data preprocessing, model training, evaluation, and visualization of results.

---

## 📌 Objective

To build and evaluate a deep learning model capable of accurately identifying digits (0–9) from 28x28 grayscale images.

---

## 📊 Dataset

- **Name**: MNIST (Modified National Institute of Standards and Technology)
- **Source**: Loaded directly via `tensorflow.keras.datasets`
- **Training Samples**: 60,000
- **Test Samples**: 10,000
- **Image Size**: 28x28 pixels, grayscale
- **Number of Classes**: 10 (digits 0–9)

---

## 🏗️ Model Architecture

The CNN architecture used in this project:

- **Input Layer**: 28x28 grayscale image
- **Conv2D** (32 filters, 3x3) + ReLU
- **MaxPooling2D** (2x2)
- **Conv2D** (32 filters, 3x3) + ReLU
- **MaxPooling2D** (2x2)
- **Flatten**
- **Dense** (64 units) + ReLU
- **Dense** (32 units) + ReLU
- **Dense** (10 units) + Softmax

Compiled using:
- **Loss Function**: `categorical_crossentropy`
- **Optimizer**: `adam`

---

## ⚙️ Training Details

- **Epochs**: 20
- **Batch Size**: 64
- **Validation**: Performed on test dataset
- **Training Accuracy**: High 90s
- **Test Accuracy**: ~98%

---

## 📈 Evaluation & Results

- The model achieves around **98% accuracy** on unseen test data.
- Loss and accuracy curves are plotted to monitor overfitting or underfitting.
- Sample predictions on test images are displayed.

---

## 🧪 Sample Predictions

The model is tested on a few examples with predicted labels displayed for visual confirmation.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/DhruvJainPy/MNISTClassification.git
cd MNISTClassification
