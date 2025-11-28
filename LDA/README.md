# Linear Discriminant Analysis (LDA) — From Scratch

This folder contains a clean, fully-documented implementation of the **Linear Discriminant Analysis (LDA)** algorithm written entirely from scratch using Python + NumPy — without using scikit-learn.

This notebook is part of the **Machine Learning Algorithms From Scratch** series.

---

## What is LDA?

Linear Discriminant Analysis (LDA) is a **supervised linear classification algorithm** that finds a projection direction which best separates two (or more) classes.

LDA projects data onto a line:

$$
z = w^T x
$$

The goal is to choose a direction $w$ that maximizes class separability.

### Fisher Criterion

LDA maximizes:

$$
J(w) = \frac{(m_1 - m_0)^2}{s_1^2 + s_0^2}
$$

Where:

- $m_0, m_1$ — projected means of each class  
- $s_0^2, s_1^2$ — within-class variances  

The optimal projection vector is:

$$
w = S_w^{-1}(\mu_1 - \mu_0)
$$

LDA produces a **straight-line decision boundary** in 2D.

---

## Files Included

- **lda.ipynb** — full step-by-step notebook:
  - Synthetic dataset generation  
  - Visualization  
  - Mean vector computation  
  - Within-class scatter matrix  
  - Projection vector  
  - Threshold computation  
  - Predictions  
  - Accuracy evaluation  
  - Linear decision boundary plot  

---

## Algorithm Steps

1. Compute class means:

$$
\mu_0,\ \mu_1
$$

2. Compute within-class scatter:

$$
S_w = \sum_{i=0}^{1} \sum_{x \in C_i} (x - \mu_i)(x - \mu_i)^T
$$

3. Compute optimal direction:

$$
w = S_w^{-1}(\mu_1 - \mu_0)
$$

4. Project samples:

$$
z = w^T x
$$

5. Compute threshold  
6. Predict class based on which side of the threshold the point falls  

---

## Visualizations Included

- Dataset scatter plot  
- LDA linear decision boundary  
- Train vs Test samples  

Example Result from Notebook:

- **LDA Accuracy: 1.000**  
- Clear linear separation between the two clusters  

---

## Skills Demonstrated

- Implementing ML algorithms manually  
- Linear algebra (scatter matrices, projections)  
- Understanding discriminative models  
- NumPy vectorization  
- Data visualization with Matplotlib  
- Clean and modular notebook design  

---

## How to Run

1. Open `lda.ipynb`  
2. Run all cells in order  
3. Inspect:
   - Means  
   - Scatter matrices  
   - Projection vector  
   - Boundary plot  

---

## Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.
