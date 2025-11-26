#  Support Vector Machine (SVM) — From Scratch

This folder contains a full implementation of a **linear Support Vector Machine (SVM)** classifier from scratch using **NumPy only**.

---

##  Overview

Support Vector Machines are powerful linear classifiers that aim to find the **maximum-margin hyperplane** separating two classes.  
Unlike simple perceptrons, SVM maximizes the distance between the boundary and the closest data points — known as **support vectors**.

The decision boundary is represented by:

$$
w^T x + b = 0
$$

---

##  SVM Objective Function

SVM optimizes the following loss function using **hinge loss + L2 regularization**:

$$
L(w, b) = \frac{1}{2} \|w\|^2 + C \sum_{i=1}^m \max(0,\; 1 - y_i (w^T x_i + b))
$$

Where:

- $w$ → weight vector  
- $b$ → bias term  
- $C$ → regularization strength  
- $y_i \in \{-1, +1\}$ → class labels  
- hinge loss penalizes misclassified samples and points inside the margin  

The margin width is:

$$
\text{margin} = \frac{2}{\|w\|}
$$

---

##  What's Inside the Notebook

- Generate a synthetic dataset  
- Convert labels into `$-1$` and `+1`  
- Implement hinge loss  
- Compute gradients for `$w$` and `$b$`  
- Train SVM using gradient descent  
- Visualize the decision boundary  
- Evaluate model accuracy  

---

##  Results Summary

- **Accuracy:** ~0.9967  
- The learned decision boundary is a **maximum-margin separator**, exactly as expected from SVM theory.  
- The two classes are cleanly separated with a wide margin.  
- Only a few points near the boundary influence the hyperplane (support vectors).  
- Hinge loss decreases smoothly during training, showing stable convergence.  

---

##  Skills Learned

- Implementation of margin-based classifiers  
- Understanding hinge loss and regularization  
- NumPy vectorized gradient computation  
- Visualizing linear decision boundaries  
- Practical understanding of support vectors  

---
##  Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.

