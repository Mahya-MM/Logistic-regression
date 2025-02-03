# Logistic Regression with a Neural Network Mindset  

This repository implements **Logistic Regression** using a **Neural Network approach** to perform **binary classification**.  

## Mathematical Formulation  

The logistic regression model is defined as follows:  

For a single example \( x^{(i)} \):  

$$
z^{(i)} = w^T x^{(i)} + b
$$

Applying the **sigmoid activation function**:  

$$
\hat{y}^{(i)} = a^{(i)} = \sigma(z^{(i)}) = \frac{1}{1 + e^{-z^{(i)}}}
$$

The **loss function** for one training example:  

$$
L(a^{(i)}, y^{(i)}) = - y^{(i)} \log(a^{(i)}) - (1 - y^{(i)}) \log(1 - a^{(i)})
$$

The **cost function** (averaging over all training examples):  

$$
J = \frac{1}{m} \sum_{i=1}^{m} L(a^{(i)}, y^{(i)})
$$

## Key Steps  

This repository follows these steps to implement **logistic regression**:  

1. **Define the model structure** (e.g., number of input features).  
2. **Initialize model parameters** (\( w \) and \( b \)).  
3. **Train the model** by minimizing the cost function using **gradient descent**:  
   - Compute the loss (**forward propagation**).  
   - Compute the gradients (**backward propagation**).  
   - Update parameters using **gradient descent**.  
4. **Make predictions** on the test set.  
5. **Analyze results and conclusions**.  

All steps are combined into a single function **`model()`**.  

## Dataset  

The dataset used in this project (**train_catvnoncat.h5** and **test_catvnoncat.h5**) consists of:  

- A **training set** of \( m_{\text{train}} \) images labeled as **cat (y = 1)** or **non-cat (y = 0)**.  
- A **test set** of \( m_{\text{test}} \) images labeled similarly.  
- Each image has shape **(num_px, num_px, 3)** (for RGB channels), meaning all images are square (**height = width = num_px**).  

This dataset was obtained from the **Deep Learning Specialization course on Coursera**.  
