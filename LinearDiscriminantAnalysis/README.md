# Linear Discriminant Analysis (LDA) — From Scratch

This folder contains a clean, fully-documented implementation of the Linear Discriminant Analysis (LDA) algorithm written entirely from scratch using Python + NumPy, without using scikit-learn.

This notebook is part of the **Machine Learning Algorithms From Scratch** series.

---

## Files Included

- **lda.ipynb** — Step-by-step Kaggle notebook  
  Includes:
  - Dataset generation  
  - LDA mathematical explanation  
  - Mean vectors  
  - Within-class scatter matrix  
  - Projection vector (Fisher’s direction)  
  - Custom LDA classifier  
  - Accuracy evaluation  
  - Straight-line decision boundary visualization  

---

## What is LDA?

Linear Discriminant Analysis (LDA) is a **supervised linear classification algorithm** that finds a projection direction that best separates two (or more) classes.

LDA projects data onto a line:

$$
z = w^T x
$$

Where:

- $w$ — projection direction  
- $z$ — projected value  

The goal of LDA is to **maximize separation between class means** while **minimizing within-class variance**.

---

## Fisher Criterion

LDA maximizes the following objective:

$$
J(w) = \frac{(m_1 - m_0)^2}{s_1^2 + s_0^2}
$$

Where:

- $m_0, m_1$ — projected class means  
- $s_0^2, s_1^2$ — within-class variances  

---

## LDA Classification Steps

1. Compute class means  
2. Compute within-class scatter matrix  
3. Compute optimal projection:  

$$
w = S_w^{-1}(\mu_1 - \mu_0)
$$

4. Project samples:

$$
z = w^T x
$$

5. Compute threshold between projected class means  
6. Predict based on which side of the threshold $z$ falls  

LDA produces a **straight-line decision boundary** in 2D.

---

## Visualizations Included

- Scatter plot of the dataset  
- Train vs Test separation  
- Color-coded class visualization  
- **Straight-line LDA decision boundary**  

---

## How to Run

1. Open the notebook `lda.ipynb`  
2. Run all cells in order  
3. Review the implementation and visualizations  

---

## Skills Demonstrated

- Implementing ML algorithms manually  
- Linear algebra foundations (scatter matrices, projections)  
- NumPy vectorized operations  
- Understanding discriminant analysis  
- Data visualization with Matplotlib  
- Clean and modular code structure  

---

## Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.
