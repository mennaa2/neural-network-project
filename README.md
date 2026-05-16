# 🧠 Neural Network Project - Handwritten Digit Recognition

## 📌 Project Overview
This project uses a Multilayer Perceptron (MLP) neural network to classify handwritten digits (0–9) using the MNIST dataset.

Different experiments were performed using different activation functions and neuron sizes to compare model performance and achieve the best accuracy.

---

# 📊 Dataset

Name: MNIST Dataset

Dataset Link:
https://keras.io/api/datasets/mnist/

Target:

0 → Digit Zero  
1 → Digit One  
2 → Digit Two  
...  
9 → Digit Nine

Dataset contains:
- 60,000 training images
- 10,000 testing images
- Images size: 28×28 grayscale

---

# ⚙️ Data Preprocessing

Applied preprocessing steps:

- Flatten images from 28×28 → 784 vector
- Normalize pixel values from 0–255 → 0–1
- One-hot encoding for labels
- Checked missing values using NumPy

Split data into:
- Training set
- Validation set
- Testing set

---

# 🧠 Model Architecture

## Experiment 1 & 2
- Input Layer: 784 neurons
- Hidden Layer 1: 128 neurons
- Hidden Layer 2: 64 neurons
- Dropout Layer: 0.3
- Output Layer: 10 neurons (Softmax)

## Experiment 3
- Input Layer: 784 neurons
- Hidden Layer 1: 256 neurons
- Hidden Layer 2: 64 neurons
- Dropout Layer: 0.3
- Output Layer: 10 neurons (Softmax)

Techniques used:
- Dropout
- Adam Optimizer
- Categorical Crossentropy

---

# 🧪 Experiments

| Experiment | Activation | Accuracy |
|---|---|---|
| Exp 1 | ReLU | 97.38% |
| Exp 2 | Tanh | 97.22% |
| Exp 3 | ReLU (256 neurons) | 97.98% |

---

# 📈 Results

- ReLU achieved higher accuracy than Tanh
- Increasing neurons improved learning performance
- Dropout reduced overfitting
- Experiment 3 achieved the best accuracy

---

# 📊 Visualization

The notebook includes:
- Loss Comparison Graph
- Accuracy Comparison Graph
- Confusion Matrix for each experiment

---
# 🏁 Conclusion

The MLP model successfully classified handwritten digits with very high accuracy.

Results showed that:

- ReLU performs better than Tanh
- Larger networks improve feature learning
- Dropout helps improve generalization

The best model was Experiment 3 using:

- ReLU activation
- 256 neurons
- 20 epochs

## ✅ Final Accuracy
97.98%

# 🚀 How to Run

Install dependencies:

```bash
pip install tensorflow matplotlib scikit-learn numpy
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```bash
Final_project_NN.ipynb
```

Run all cells step by step.

---

# 👩‍💻 Author

Mennatallah Mohsen
