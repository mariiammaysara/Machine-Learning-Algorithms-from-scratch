# Linear Regression — From Scratch

This folder contains a full implementation of **Linear Regression** using **NumPy only**, without relying on scikit-learn.  
The goal is to understand the mathematics and logic behind the algorithm by building every component manually.

---

##  What’s Inside?

- **linear-regression-from-scratch.ipynb**  
  A clean, well-structured notebook that walks through the entire implementation including:
  - Dataset generation  
  - Prediction function  
  - Cost function (MSE)  
  - Gradient Descent  
  - Training  
  - Visualization  
  - Model analysis  

---

##  What is Linear Regression?

Linear Regression is a fundamental supervised learning algorithm that models the relationship between an input variable \( X \) and an output variable \( y \) using a straight line:

$$
\hat{y} = \theta_0 + \theta_1 X
$$

Where:
- $$\( \theta_0 \)$$ — Bias (intercept)  
- $$\( \theta_1 \)$$ — Weight (slope)

The objective is to find the values of $$\( \theta_0 \)$$ and $$\( \theta_1 \)$$ that **minimize the prediction error** between \( y \) and $$\( \hat{y} \)$$.  
This is achieved using **Gradient Descent**.

---

##  Steps Implemented

1. Generate a synthetic dataset  
2. Add the bias column  
3. Define the prediction function  
4. Implement the Mean Squared Error (MSE)  
5. Implement Gradient Descent  
6. Train the model  
7. Plot the regression line  
8. Plot the cost curve  
9. Analyze the learned parameters  

---

##  Results & Interpretation

- Learned parameters:  
  - $$\( \theta_0 \)$$ — bias term  
  - $$\( \theta_1 \)$$ — weight  
- The regression line fits the data well  
- The cost decreases smoothly → Gradient Descent converged properly  

---

##  Purpose of This Implementation 

This implementation is designed for learning, understanding, and practicing the fundamentals of Machine Learning by coding algorithms manually — without relying on libraries that hide the underlying mathematics.

---

##  Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.
