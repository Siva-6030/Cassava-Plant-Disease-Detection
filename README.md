
# Cassava Leaf Disease Classification (Hybrid Quantum-Classical Model)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)
![PennyLane](https://img.shields.io/badge/PennyLane-Quantum-purple?style=flat-square)

## 📌 Overview
This repository contains a hybrid classical-quantum machine learning project designed to classify cassava leaf diseases. By integrating a traditional Convolutional Neural Network (VGG16) with quantum computing layers via PennyLane, this model accurately categorizes leaf images to help identify agricultural diseases early.

## 📊 Dataset
The project utilizes the [Cassava Leaf Disease Classification](https://www.kaggle.com/datasets/nirmalsankalana/cassava-leaf-disease-classification) dataset from Kaggle. 

The model classifies images into the following five categories:
1. **Bacterial Blight**
2. **Brown Streak**
3. **Green Mottle**
4. **Mosaic Disease**
5. **Healthy**

## 🧠 Architecture
* **Classical Base:** VGG16 (Pre-trained on ImageNet, fine-tuned for this dataset)
* **Quantum Component:** 2 Qubits and 2 Quantum Layers using PennyLane (`default.qubit` device)
* **Image Processing:** Images are downscaled to 128x128 pixels for efficient processing.
* **Epochs:** Configured for 10 epochs for both VGG and Quantum layers.
