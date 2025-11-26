#  Logistic Regression — From Scratch

This directory contains a full **from-scratch implementation of Logistic Regression** using only **NumPy**, without relying on scikit-learn for the model itself.  
The goal is to understand binary classification at the mathematical and algorithmic levels.

---

##  What is Logistic Regression?

Logistic Regression is a **binary classification** algorithm.  
Instead of predicting a continuous value, it predicts a **probability** between 0 and 1 using the sigmoid function.

The hypothesis function:

$$
\hat{y} = \sigma(\theta^T X)
$$

Where the sigmoid function \( \sigma(z) \) is defined as:

$$
\sigma(z) = \frac{1}{1 + e^{-z}}
$$

The model predicts:

- $( \hat{y} \approx 1 )$ → positive class  
- $( \hat{y} \approx 0 )$ → negative class  

---

##  Cost Function (Binary Cross-Entropy)

To measure how well the model fits the data, we use the **Binary Cross-Entropy Loss**:

$$
J(\theta) = -\frac{1}{m} \sum_{i=1}^{m} 
\bigg[ y^{(i)} \log\big(\hat{y}^{(i)}\big) + 
(1 - y^{(i)}) \log\big(1 - \hat{y}^{(i)}\big) \bigg]
$$

This ensures the model learns probabilities close to the true labels.

---

##  Gradient Descent Optimization

To minimize the loss, we compute the gradient:

$$
\nabla_\theta J(\theta) = \frac{1}{m} X^T(\hat{y} - y)
$$

And update:

$$
\theta \leftarrow \theta - \alpha \nabla_\theta J(\theta)
$$

Where:

- $( \alpha \)$ → learning rate  
- $( \theta \)$ → model parameters  

---

##  What’s Implemented in This Notebook

- Generate a synthetic binary classification dataset  
- Add the bias term  
- Implement the sigmoid function  
- Implement the hypothesis function  
- Implement the Binary Cross-Entropy loss  
- Gradient Descent from scratch  
- Plot loss curve over iterations  
- Plot 2D decision boundary  
- Evaluate model behavior  

---

##  Results Overview

- The **loss decreases smoothly**, showing that gradient descent converged properly.  
- The **decision boundary is linear**, which matches the theoretical form of logistic regression.  
- The separator correctly divides the two classes, with a clear transition region around probability 0.5.

---

##  Purpose

This implementation helps in:

- Building mathematical intuition  
- Understanding classification models  
- Practicing NumPy vectorization  
- Learning how decision boundaries form   

---

##  Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.

