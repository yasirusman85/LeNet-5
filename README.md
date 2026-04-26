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
graph LR
    %% Layer Definitions
    Input(["Input: 32x32x1 Image"]) --> C1[["C1: Conv (5x5, 6 filters)"]]
    C1 --> S2{{"S2: Avg Pooling (2x2)"}}
    S2 --> C3[["C3: Conv (5x5, 16 filters)"]]
    C3 --> S4{{"S4: Avg Pooling (2x2)"}}
    S4 --> C5[["C5: Conv (5x5, 120 filters)"]]
    C5 --> F1[/"Flatten"/]
    F1 --> D1(["F6: Dense (84 units)"])
    D1 --> Output(["Output: Softmax (10)"])

    %% Styling for Beauty
    style Input fill:#f9f,stroke:#333,stroke-width:2px
    style C1 fill:#bbf,stroke:#333,stroke-width:2px
    style S2 fill:#dfd,stroke:#333,stroke-width:2px
    style C3 fill:#bbf,stroke:#333,stroke-width:2px
    style S4 fill:#dfd,stroke:#333,stroke-width:2px
    style C5 fill:#bbf,stroke:#333,stroke-width:2px
    style F1 fill:#eee,stroke:#333,stroke-width:1px
    style D1 fill:#fdd,stroke:#333,stroke-width:2px
    style Output fill:#f9f,stroke:#333,stroke-width:4px
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
