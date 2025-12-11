# 🧠 CIFAKE Detection using a Custom CNN  
A lightweight CNN model trained to classify **real vs AI-generated images (CIFAKE dataset)**.  
What surprised me the most is how **even my own eyes couldn’t reliably tell fake from real**, yet a basic CNN picked up subtle patterns and hit strong accuracy.  
This project became my personal crash course in **Explainable AI** and how mysterious model decisions really are.

---

## 🚀 Project Overview
This project focuses on:
- Training a **custom CNN** on the Kaggle CIFAKE dataset  
- Using **PyTorch** with AMP + RAM caching for faster training  
- Evaluating accuracy, loss, and predictions  
- Understanding how deep models differentiate between **real and synthetic** images

---

## 📂 Dataset
**CIFAKE: Real vs AI-Generated Images**  
Kaggle link: https://www.kaggle.com/datasets/vivmankar/cifake-real-and-ai-generated-images

- 60k real images  
- 60k AI-generated images  
- 32x32 resolution  

Perfect for explainability experiments since humans struggle with this classification while models excel.

---

## 🏗 Model Architecture
A simple yet effective CNN:
- 3 Convolutional blocks  
- ReLU + BatchNorm  
- MaxPooling  
- Fully connected layers for 2-class output  
- Trained with **CrossEntropyLoss** + **Adam** optimizer  
- AMP (Automatic Mixed Precision) enabled for speed

---

## 📊 Training Results
Typical performance achieved:
- **Accuracy:** ~90 percent  
- **Loss:** stable and smooth  
- CNN learns tiny texture differences that humans cannot notice  

This project highlights why **Explainable AI is important**, because the model clearly sees something we don’t.

---

## 🧪 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/cifake-cnn.git
cd cifake-cnn
