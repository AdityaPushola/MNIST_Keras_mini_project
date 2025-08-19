# MNIST Neural Network from Scratch (TensorFlow 2.x) and Pytorch

## 📌 Overview
This project implements a **Multilayer Perceptron (MLP)** from scratch in TensorFlow 2 to classify handwritten digits from the **MNIST dataset** (0–9).

- Uses **low-level TensorFlow ops** (`tf.Variable`, `tf.matmul`, `tf.GradientTape`)
- No `Dense` layers or `model.fit()` — everything (forward pass, loss, backprop, optimizer) is coded manually
- Helps understand how neural networks **learn through gradient descent**

---

## 🧠 Model Architecture
- **Input layer:** 784 neurons (flattened 28×28 images)
- **Hidden Layer 1:** 128 neurons, Sigmoid activation
- **Hidden Layer 2:** 256 neurons, Sigmoid activation
- **Output Layer:** 10 neurons, Softmax activation (digit probabilities)

---

## ⚙️ Training Details
- **Loss function:** Categorical Cross-Entropy
- **Optimizer:** Stochastic Gradient Descent (SGD)
- **Batch size:** 256
- **Training steps:** 3000
- **Learning rate:** 0.001

---

## 📊 Results
- **Training:** Loss decreases steadily over iterations
- **Test Accuracy:** ~95% (after 3000 steps)
