# 🤖 CAPTCHA Solving using Convolutional Neural Networks (CNN)

A deep learning-based solution to automatically decode CAPTCHA images using Convolutional Neural Networks. This project leverages TensorFlow and Keras to build, train, and optimize a model capable of recognizing distorted alphanumeric text from noisy image backgrounds.

---

## 📌 Features

- 🎯 **High Accuracy CAPTCHA Solver** – Custom-trained CNN to crack alphanumeric CAPTCHA images.
- 🧹 **Image Preprocessing** – Grayscale conversion, noise filtering, and segmentation techniques applied.
- 🧠 **CNN Architecture** – Designed a multi-layered model with convolution, pooling, and dropout layers for effective learning.
- 📈 **Model Optimization** – Applied regularization, data augmentation, and learning rate tuning for enhanced performance.

---

## 🧠 Tech Stack

| Tool/Library | Purpose |
|--------------|---------|
| Python       | Core Programming Language |
| TensorFlow & Keras | Deep Learning Framework |
| OpenCV       | Image Processing |
| NumPy        | Numerical Computations |
| Matplotlib   | Visualizations & Debugging |

---


## 🏗️ Model Architecture

Input (Captcha Image - 200x50x1)
│
├── Conv2D (32 filters, 3x3) + ReLU
├── MaxPooling2D (2x2)
├── Dropout (0.25)
│
├── Conv2D (64 filters, 3x3) + ReLU
├── MaxPooling2D (2x2)
├── Dropout (0.25)
│
├── Flatten
├── Dense (128) + ReLU
├── Dropout (0.5)
└── Dense (Output Layer - Softmax for each character)
