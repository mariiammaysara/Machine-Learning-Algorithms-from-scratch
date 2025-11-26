#  Naive Bayes — From Scratch

This folder contains a clean, NumPy-only implementation of the **Gaussian Naive Bayes** classifier.  
The goal is to understand how probabilistic classification works without relying on scikit-learn.

---

##  What is Naive Bayes?

Naive Bayes is a **probabilistic classifier** based on **Bayes’ Theorem**, where each class is chosen according to which one gives the highest **posterior probability**.

The core idea:

$$
P(y|x) \propto P(x|y)\, P(y)
$$

Where:

- $P(y|x)$ → Posterior probability of class $y$ given features $x$  
- $P(x|y)$ → Likelihood of the features under class $y$  
- $P(y)$ → Prior probability of class $y$  
- $\propto$ → “Proportional to”, because the denominator $P(x)$ is constant across classes  

The “naive” assumption:  
All features are **conditionally independent** given the class label — making computations fast and simple.

---

##  Gaussian Likelihood
The Gaussian likelihood measures how likely a given feature value is to appear within a specific class, assuming that the feature follows a normal (Gaussian) distribution.

In **Gaussian Naive Bayes**, each feature of each class is modeled using a **normal distribution**:

$$
P(x_i|y) = \frac{1}{\sqrt{2\pi\sigma^2}}
\exp\left(-\frac{(x_i - \mu)^2}{2\sigma^2}\right)
$$

NB computes:

- Per-class means  
- Per-class variances  
- Per-class priors  
- Log-likelihood for each class  

And predicts the class with the highest:

$$
\log P(y) + \sum \log P(x_i|y)
$$

---

##  What's Implemented in This Notebook?

- Synthetic dataset generation  
- Priors for each class  
- Per-class means and variances  
- Gaussian PDF  
- Log-likelihood computation  
- Posterior comparison  
- Prediction for each sample  
- Decision boundary visualization  
- Accuracy evaluation  

---

##  Model Evaluation

- **Accuracy:** ~0.993  
- The decision boundary is **curved**, which is expected for Gaussian likelihoods.  
- Blue region → Class 0 has higher posterior probability  
- Red region → Class 1 has higher posterior probability  
- The separator naturally arises from comparing log-probabilities of both classes  
- The classifier fits the data distribution extremely well  

---

##  Summary

- Gaussian Naive Bayes is extremely fast  
- Works well when class distributions follow Gaussian shapes  
- Produces **non-linear** decision boundaries  
- Ideal for high-dimensional data  
- Great baseline model for classification  

---

##  Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* collection.
