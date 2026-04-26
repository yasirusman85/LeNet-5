This version replaces the GIF with a sleek, structured **Mermaid.js** diagram and further streamlines the text for maximum readability.

---

# 🧠 LeNet-5 CNN: MNIST Recognition

> A high-performance implementation of the 1998 LeCun architecture, bridging the gap between classic computer vision and modern deep learning.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat-square&logo=python) 
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)
![Accuracy](https://img.shields.io/badge/Accuracy-98.62%25-brightgreen?style=flat-square)

---

## 🏗️ Interactive Architecture Flow
The diagram below follows the data transformation from a **32x32** padded image to a **10-digit** classification.

```mermaid
flowchart LR
A[Input Image] --> B[Feature Extraction]
B --> C[Edge Detection]
B --> D[Curve Detection]
B --> E[Shape Detection]
C --> F[Pooling]
D --> F
E --> F
F --> G[Dense Layers]
G --> H[Classification]
```

---

## 📊 Core Metrics

| Metric | Result |
| :--- | :--- |
| **Input Size** | 32 × 32 (Zero-padded) |
| **Total Parameters** | 61,706 |
| **Test Accuracy** | **98.62%** |
| **Test Loss** | 0.0437 |

---

## 💻 Quick Start

1. **Install**
   ```bash
   pip install tensorflow numpy streamlit
   ```
2. **Deploy**
   ```bash
   streamlit run app.py
   ```

---

## 🚀 Advanced Roadmap
* **Activation Swap:** Replace `tanh` with `ReLU` for faster training.
* **Regularization:** Integrate **Dropout** or **Batch Normalization**.
* **Modern Comparison:** Benchmark performance against modern **Vision Transformers (ViT)**.

---

**Author:** Yasir  
*AI | Deep Learning | Computer Vision*
