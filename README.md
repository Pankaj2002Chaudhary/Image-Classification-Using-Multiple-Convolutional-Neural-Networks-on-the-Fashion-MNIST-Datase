# Image-Classification-Using-Multiple-Convolutional-Neural-Networks-on-the-Fashion-MNIST-Datase
With the rising elderly population, service robots are becoming essential for assisting with daily tasks. This study applies CNN models for clothing recognition. The proposed MCNN15 achieved 93.11% accuracy on Fashion-MNIST and 81.5% on the Fashion-Product dataset.

# Multiple Convolutional Neural Networks (MCNN9, MCNN12, MCNN15, MCNN18)

This repository implements four deep convolutional neural network architectures
(MCNN9, MCNN12, MCNN15, MCNN18) inspired by the paper:

**"Image Classification Using Multiple Convolutional Neural Networks on the Fashion-MNIST Dataset"**  
*Sensors (MDPI), 2022*

The goal is to evaluate how increasing network depth affects performance on the
Fashion-MNIST dataset.

---

## 📌 Project Overview

This project trains and compares four CNN architectures:

- **MCNN9**  –  9 convolutional layers  
- **MCNN12** – 12 convolutional layers  
- **MCNN15** – 15 convolutional layers  
- **MCNN18** – 18 convolutional layers  

Each network is trained:

- on **100% of the Fashion-MNIST dataset**  
- for **20 epochs**  
- using the same training pipeline  
- to ensure a fair comparison  

The study helps understand how deeper architectures impact accuracy, 
generalization, and training stability.

---

## 📂 Dataset

### **Fashion-MNIST**
- 60,000 training images  
- 10,000 test images  
- 10 clothing categories  
- 28×28 grayscale images  

Dataset Source:  
https://www.kaggle.com/datasets/zalando-research/fashionmnist

---

## 🧠 Model Architecture

Each MCNN follows the same design principle:

- Repeated blocks of:  
  **Conv2D → BatchNorm → ReLU → MaxPool**
- Deeper models simply include more convolutional layers
- Fully connected layers at the end for classification

| Model | Conv Layers | Parameters | Depth |
|-------|-------------|------------|-------|
| MCNN9  | 9  | moderate | shallow |
| MCNN12 | 12 | deeper | medium |
| MCNN15 | 15 | deep | strong performer |
| MCNN18 | 18 | very deep | may overfit |

---

## 🚀 How to Run

### 1️⃣ Install dependencies
```bash
pip install tensorflow numpy matplotlib tqdm
