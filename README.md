# deep-learning-
# Malaria Cell Image Classification Using Deep Learning

## Project Overview

This project was developed as part of the **7053SCN – Deep Learning and Computer Vision** module at **Coventry University**.

The objective of this project is to automatically classify microscopic blood cell images into two categories:

* **Parasitized**
* **Uninfected**

Two deep learning approaches were implemented and compared:

* Custom Convolutional Neural Network (CNN)
* MobileNetV2 Transfer Learning

---

# Dataset

**Dataset:** Malaria Cell Images Dataset

The original dataset contains microscopic blood smear images of infected and healthy blood cells.

For this project, a balanced subset of **13,000 images** was used:

* Parasitized: 6,500 images
* Uninfected: 6,500 images

Dataset split:

* Training: 10,400 images (80%)
* Validation: 1,300 images (10%)
* Testing: 1,300 images (10%)

---

# Project Workflow

1. Device Configuration
2. Dataset Loading
3. Exploratory Data Analysis (EDA)
4. Data Preprocessing
5. Train–Validation–Test Split
6. CNN Model Development
7. CNN Training and Evaluation
8. MobileNetV2 Development
9. MobileNetV2 Training and Evaluation
10. Model Comparison
11. Computational Analysis
12. Ethical Considerations

---

# Models Used

## Model 1 – Custom CNN

The CNN architecture consists of:

* Convolution Layers
* Batch Normalization
* ReLU Activation
* MaxPooling
* Adaptive Average Pooling
* Dropout
* Fully Connected Layers

### CNN Test Accuracy

**95.15%**

---

## Model 2 – MobileNetV2

Transfer learning was applied using MobileNetV2 pretrained on ImageNet.

Only the classifier layers were trained while the feature extraction layers were frozen.

### MobileNetV2 Test Accuracy

**92.85%**

---

# Model Comparison

| Metric               |        CNN | MobileNetV2 |
| -------------------- | ---------: | ----------: |
| Test Accuracy        | **95.15%** |  **92.85%** |
| Precision            |       0.95 |        0.93 |
| Recall               |       0.95 |        0.93 |
| F1-Score             |       0.95 |        0.93 |
| Total Parameters     |    110,466 |   2,388,098 |
| Trainable Parameters |    110,466 |     164,226 |

---

# Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Google Colab

---

# Results

The custom CNN achieved the best overall performance with a **95.15% test accuracy**, outperforming the MobileNetV2 transfer learning model, which achieved **92.85%**.

---

# Future Work

Possible improvements include:

* Fine-tuning MobileNetV2
* Testing additional transfer learning models such as EfficientNet or DenseNet
* Using larger and more diverse malaria datasets
* Applying explainable AI techniques such as Grad-CAM

---

# Author

**Chandan Pandit**

MSc Data Science

Coventry University

Module: 7053SCN – Deep Learning and Computer Vision
