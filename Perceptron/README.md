#  Perceptron — From Scratch

This folder contains a full implementation of the **Perceptron** algorithm from scratch using **NumPy only**.

---

##  Overview

The Perceptron is one of the earliest and simplest binary linear classifiers.  
It learns a separating hyperplane by updating its weights **only when it misclassifies a sample**.

The prediction rule is:

$$
\hat{y} =
\begin{cases}
1 & \text{if } w^T x + b \ge 0 \\
0 & \text{otherwise}
\end{cases}
$$

---

##  Perceptron Learning Rule

During training, the model updates its parameters based on the error:

$$
w := w + \eta (y - \hat{y}) x
$$

$$
b := b + \eta (y - \hat{y})
$$

Where:  
- $w$ → weights  
- $b$ → bias  
- $\eta$ → learning rate  

The perceptron works best when classes are **linearly separable**.

---

##  What’s Inside the Notebook

- Generate a synthetic dataset  
- Implement Perceptron prediction  
- Implement the update rule  
- Train the model  
- Plot the decision boundary  
- Evaluate accuracy  

---

##  Results Summary

- **Accuracy:** ~0.97  
- The decision boundary is a **straight linear separator**.  
- Errors occur mainly near the boundary.  
- Fast convergence due to simple update rule.  

---

##  Skills Learned

- Binary classification fundamentals  
- Linear models from scratch  
- NumPy vector operations  
- Decision boundary visualization  
- Understanding perceptron convergence  

---
##  Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.
