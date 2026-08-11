# Alzheimer's Disease Classification Using Deep Learning

## 📌 Overview

This project focuses on classifying brain MRI images into two categories: **Healthy** and **Diseased** using deep learning and convolutional neural networks (CNNs).

The project compares multiple CNN architectures to evaluate their effectiveness for Alzheimer's-related MRI image classification.

## 🎯 Objectives

* Classify brain MRI images into Healthy and Diseased categories.
* Compare different CNN architectures.
* Evaluate model performance using consistent patient-wise validation.
* Explore techniques for improving model generalization and handling class imbalance.

## 📊 Dataset

* **10,442 MRI images**
* **68 unique patients**
* Image size: **224 × 224**
* Binary classification:

  * Healthy
  * Diseased

To prevent data leakage, images were split **by patient**, ensuring that images from the same patient did not appear in both training and validation sets.

## 🧠 Models

The following architectures were evaluated:

* **VGG16** — Transfer Learning with ImageNet weights
* **MobileNetV2** — Transfer Learning
* **Custom CNN**
* **Enhanced VGG16** with SMOTE and Grid Search

## ⚙️ Techniques

* Image resizing and normalization
* Data augmentation
* Patient-wise splitting
* 5-Fold Stratified Cross-Validation
* Transfer Learning
* Class weighting
* SMOTE for class balancing
* Early Stopping
* Dropout
* L2 Regularization
* Batch Normalization
* Grid Search

## 📈 Results

| Model          |   Accuracy |
| -------------- | ---------: |
| VGG16          |     75.65% |
| MobileNetV2    |     60.48% |
| **Custom CNN** | **80.69%** |
| VGG16 + SMOTE  |     78.38% |

The **Custom CNN achieved the highest overall accuracy of 80.69%** among the evaluated models.

## 🛠️ Technologies

* Python
* TensorFlow / Keras
* Scikit-learn
* NumPy
* Matplotlib
* Seaborn
* imbalanced-learn (SMOTE)

## 📚 Key Learning Outcomes

Through this project, I gained practical experience in:

* Deep Learning and CNN architectures
* Transfer Learning
* Medical image classification
* Data augmentation and class balancing
* Cross-validation and preventing data leakage
* Model comparison and performance evaluation
* Confusion matrices and classification reports

## ⚠️ Note

This project is an academic machine learning project and is **not intended for clinical diagnosis or medical decision-making**.
