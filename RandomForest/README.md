# Random Forest — From Scratch

This notebook implements a **Random Forest Classifier** from scratch using only NumPy.  
No scikit-learn RandomForest functions are used.

## What We Do in This Notebook
- Generate a 2D synthetic dataset  
- Implement a simplified Decision Tree  
- Compute Gini impurity  
- Perform bootstrap sampling  
- Select random feature subsets  
- Build multiple trees in an ensemble  
- Predict using majority voting  
- Visualize the decision boundary  
- Evaluate model accuracy  

---

## What Is a Random Forest?
Random Forest is an **ensemble learning method** that builds multiple decision trees and aggregates their predictions.

Each tree is trained on:
1. A bootstrap sample of the dataset  
2. A random subset of features  

Final prediction is obtained through majority voting.

---

## Mathematical Intuition

### Bootstrap Sampling
Each tree receives a dataset sampled with replacement:

$$
D_t = \{ (x_i,\; y_i) \mid i \in \text{Bootstrap}(1,\dots,N) \}
$$

### Random Feature Selection
At every split, the tree evaluates only a subset of features:

$$
F_t \subseteq \{1,\dots,d\}, \qquad |F_t| = m
$$

### Gini Impurity
Node impurity is computed using the Gini index:

$$
Gini = 1 - \sum_{k=1}^{K} p_k^2
$$

Where:  
- $p_k$ is the proportion of samples belonging to class $k$  
- Lower Gini indicates purer nodes  
- $Gini = 0$ means perfect purity  

### Majority Vote
Final prediction from the forest:

$$
\hat{y} = \text{mode}\big(h_1(x),\; h_2(x),\; \dots,\; h_T(x)\big)
$$

Where $h_t(x)$ is the prediction of tree $t$.

---

## Decision Boundary and Model Evaluation

**Accuracy:** 1.0  

Observations:
- The Random Forest perfectly separates the dataset.  
- The boundary is non-linear and formed by combining multiple trees.  
- Ensemble learning reduces the variance of individual trees.  
- Majority voting produces stable predictions.  

---

## Summary
- Random Forest uses bootstrap sampling to diversify trees.  
- Random feature selection at each split prevents correlation between trees.  
- Majority voting reduces variance and improves generalization.  
- The algorithm forms flexible and stable decision boundaries.  
- This implementation achieves perfect accuracy on this dataset.

---

## Author
Created by **Mariam Maysara**  
Part of the **Machine Learning Algorithms From Scratch** series.
