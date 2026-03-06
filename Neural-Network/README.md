# 🧠 MNIST Neural Network

> A deep learning project that classifies handwritten digits (0–9) using a neural network built with **TensorFlow/Keras**.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat-square&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-red?style=flat-square&logo=keras)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)

---

## 📌 Overview

This project demonstrates the complete workflow of building a handwritten digit classifier — from raw pixel data to a trained model with visual evaluation.

✅ Load and explore the MNIST dataset  
✅ Normalize and preprocess image data  
✅ Build and compare two neural network architectures  
✅ Train with the Adam optimizer  
✅ Evaluate with test accuracy and a confusion matrix  

---

## 📊 Dataset

The **MNIST dataset** is one of the most well-known benchmarks in machine learning.

| Property | Details |
|---|---|
| 🏋️ Training images | 60,000 |
| 🧪 Test images | 10,000 |
| 🖼️ Image size | 28 × 28 pixels |
| 🔢 Classes | Digits 0–9 |

Each grayscale image represents a single handwritten digit written by different people.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|---|---|
| 🐍 Python | Core language |
| 🔶 TensorFlow / Keras | Model building & training |
| 🔢 NumPy | Array operations |
| 📊 Matplotlib | Visualizations |
| 🎨 Seaborn | Confusion matrix heatmap |

---

## ⚙️ Project Workflow

### 1. 📥 Load Dataset
```python
(X_train, y_train), (X_test, y_test) = keras.datasets.mnist.load_data()
```

### 2. 🔧 Data Preprocessing
- Normalize pixel values: **0–255 → 0–1**
- Flatten images: **28×28 → 784** features

### 3. 🏗️ Model Architecture

#### Basic Model
```
Input (784) → Output (10, Sigmoid)
```

#### ⭐ Improved Model
```
Input (784) → Hidden (100, ReLU) → Output (10, Sigmoid)
```

### 4. 🏋️ Training

```python
model.compile(optimizer='adam',
              loss='sparse_categorical_crossentropy',
              metrics=['accuracy'])

model.fit(X_train, y_train, epochs=5)
```

- **Optimizer:** Adam  
- **Loss:** Sparse Categorical Crossentropy  
- **Epochs:** 5  

### 5. 📈 Evaluation
- Test dataset accuracy score
- Confusion matrix heatmap — shows exactly where the model gets confused between digit classes

---

## 👩‍💻 Author

**Akisha Bhujel**

[![GitHub](https://img.shields.io/badge/GitHub-akisavujel-black?style=flat-square&logo=github)](https://github.com/akisavujel)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-akishabhujel-blue?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/akishabhujel/)
[![Kaggle](https://img.shields.io/badge/Kaggle-akisavujel-20beff?style=flat-square&logo=kaggle)](https://www.kaggle.com/akisavujel)

---

⭐ **If you found this project helpful, consider giving the repository a star — it means a lot!**
