# Logistic Regression with a Neural Network Mindset  

This repository implements **Logistic Regression** using a **Neural Network approach** to perform **binary classification** (cat vs. non-cat). The implementation is inspired by the **Deep Learning Specialization by Andrew Ng**.

---

## 🚀 Project Overview  

Logistic Regression is a fundamental machine learning algorithm used for binary classification. This implementation follows a **Neural Network mindset**, using:  
✅ **Vectorized computations** for efficiency.  
✅ **Gradient descent optimization** for learning.  
✅ **Visualization of the cost function** across iterations.  
✅ **Analysis of different learning rates** to improve performance.  

---

## 📂 Repository Structure  

- **`L_R.ipynb`** → Jupyter Notebook containing the full implementation, step-by-step explanations, and visualizations.  
- **`lr_utils.py`** → Helper functions for loading and processing the dataset.  
- **`datasets/train_catvnoncat.h5`** → Training dataset.  
- **`datasets/test_catvnoncat.h5`** → Test dataset.  
- **`images`** → For further analysis and testing the trained logistic regression with other images.
---

## 🏗️ Model Architecture  

The logistic regression model follows these steps:  

1️⃣ **Initialize Parameters**: Set $W$ and $b$ to zero.  

2️⃣ **Forward Propagation**: Compute $Z = W^T X + b$, then apply the **sigmoid activation function**:  
   $\hat{Y} = \sigma(Z) = \frac{1}{1 + e^{-Z}}$ 

3️⃣ **Compute Cost**: Use **binary cross-entropy loss** to measure the difference between predictions and true labels:  
   $J = -\frac{1}{m} \sum \left( Y \log(\hat{Y}) + (1-Y) \log(1-\hat{Y}) \right)$  

4️⃣ **Backward Propagation**: Compute gradients \( dW \) and \( db \) to determine how to adjust parameters.  

5️⃣ **Update Parameters**: Apply **gradient descent** to optimize \( W \) and \( b \):  
   $W = W - \alpha dW, \quad b = b - \alpha db$  

6️⃣ **Make Predictions**: Convert probabilities into binary labels:
Make Predictions: Convert probabilities into binary labels: 
ŷ =
{1,  if A ≥ 0.5  
0,  if A < 0.5}


   🤝 Contributing
Feel free to fork, submit issues, or contribute improvements! 🚀
