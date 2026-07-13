# Lung Disease Classification using MedMNIST and PyTorch

A deep learning project that classifies chest X-ray images into **Normal** and **Pneumonia** categories using the **MedMNIST** dataset and a Convolutional Neural Network (CNN) implemented with **PyTorch**.

---

## Project Overview

Early detection of lung diseases is essential for improving patient outcomes. This project develops a CNN-based image classification model capable of distinguishing between **Normal** and **Pneumonia** chest X-ray images.

The complete pipeline includes:

- Dataset loading
- Data preprocessing
- CNN model development
- Model training
- Validation
- Performance evaluation
- Model saving
- Visualization of predictions

---

## Dataset

The project uses the **MedMNIST Lung Dataset**, a lightweight benchmark dataset designed for medical image classification tasks.

Dataset Split:

| Dataset | Samples |
|---------|---------:|
| Training | 4,708 |
| Validation | 524 |
| Testing | 624 |

---

## Project Workflow

### 1. Dataset Loading

- Download MedMNIST dataset
- Split into training, validation, and testing sets

---

### 2. Data Preprocessing

- Image normalization
- Tensor conversion
- Batch loading using PyTorch DataLoader

---

### 3. Model Architecture

A custom Convolutional Neural Network consisting of:

- Convolution Layers
- ReLU Activation
- Max Pooling
- Fully Connected Layers
- Softmax Classification

---

### 4. Model Training

- Loss Function: CrossEntropyLoss
- Optimizer: Adam
- Device: CPU
- Epochs: 5

---

### 5. Model Evaluation

The trained model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

---

## Training Results

| Epoch | Training Loss | Validation Loss | Validation Accuracy |
|------:|--------------:|----------------:|--------------------:|
| 1 | 0.1730 | 0.0884 | **96.37%** |
| 2 | 0.1163 | 0.0933 | **96.56%** |
| 3 | 0.0856 | 0.1567 | **94.08%** |
| 4 | 0.0820 | 0.0767 | **97.14%** |
| 5 | 0.0711 | 0.0976 | **96.76%** |

---

## Test Performance

### Overall Accuracy

**85%**

### Classification Report

| Class | Precision | Recall | F1-Score |
|--------|----------:|--------:|----------:|
| Normal | 0.99 | 0.62 | 0.76 |
| Pneumonia | 0.81 | 1.00 | 0.90 |

**Weighted Average**

- Precision: **0.88**
- Recall: **0.85**
- F1-score: **0.84**

---

## Visualizations

The notebook includes:

- Sample chest X-ray images
- Training progress
- Validation metrics
- Confusion Matrix
- Classification Report
- Prediction visualization

---

## Technologies Used

- Python
- PyTorch
- MedMNIST
- NumPy
- Matplotlib
- Scikit-learn

---

## Installation

Install the required libraries:

```bash
pip install torch torchvision medmnist matplotlib numpy scikit-learn
```

---

## Project Structure

```
.
├── MedMnist_Lung.ipynb
├── medmnist_cpu_model.pth
├── README.md
└── requirements.txt
```

---

## Project Pipeline

```
Chest X-ray Images
        │
        ▼
Dataset Loading
        │
        ▼
Data Preprocessing
        │
        ▼
CNN Model
        │
        ▼
Model Training
        │
        ▼
Validation
        │
        ▼
Testing
        │
        ▼
Disease Prediction
```

---

## Applications

This project can be extended for:

- Computer-Aided Diagnosis (CAD)
- Hospital screening systems
- Medical imaging research
- Deep learning education
- Healthcare AI applications

---

## Future Improvements

- Train for more epochs
- Apply transfer learning (ResNet, DenseNet, EfficientNet)
- Add data augmentation
- Hyperparameter tuning
- Deploy with Streamlit or Flask
- Multi-class lung disease classification

---

## Key Results

-  Validation Accuracy: **97.14%**
-  Test Accuracy: **85%**
-  Successfully classified Normal and Pneumonia chest X-rays
-  Model weights saved for future inference

---

##  License

This project is intended for educational and research purposes.

---
