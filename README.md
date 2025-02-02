# Logistic-regression
This repository build a Logistic Regression, using a Neural Network mindset to perform binary classification.

**Mathematical expression of the algorithm**:

For one example x^(i):

1. z^(i) = w^T x^(i) + b
2. y_hat^(i) = a^(i) = sigmoid(z^(i))
3. L(a^(i), y^(i)) = -y^(i) log(a^(i)) - (1 - y^(i)) log(1 - a^(i))

The cost is then computed by summing over all training examples:

J = (1/m) * Σ [L(a^(i), y^(i))] for i = 1 to m

**Key steps**:

This repository carry out the following steps: 
- Define the model structure (such as number of input features).
- Initialize the parameters of the model.
- Learn the parameters for the model by minimizing the cost. 
  Loop:
    - Calculate current loss (forward propagation)
    - Calculate current gradient (backward propagation)
    - Update parameters (gradient descent)
- Use the learned parameters to make predictions (on the test set)
- Analyse the results and conclude.

These steps build separately and integrate into one function called `model()`.

**Dataset**:
Given dataset ("train_catvnoncat.h5" and "test_catvnoncat.h5") containing:
- a training set of m_train images labeled as cat (y=1) or non-cat (y=0).
- a test set of m_test images labeled as cat or non-cat .

Each image is of shape (num_px, num_px, 3) where 3 is for the 3 channels (RGB). Thus, each image is square (height = num_px) and (width = num_px).
You will build a simple image-recognition algorithm that can correctly classify pictures as cat or non-cat.

Data set downloaded from deeplearning specialization coursea course.
