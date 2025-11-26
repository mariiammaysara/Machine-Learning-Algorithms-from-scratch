# Decision Tree — From Scratch


## Overview

This notebook implements a **Decision Tree Classifier** from scratch using only **NumPy**.  
No scikit-learn decision tree functions are used.

---

## What We Do in This Notebook

- Generate a 2D synthetic dataset  
- Compute class impurities  
- Evaluate all possible feature thresholds  
- Select the optimal split using Gini impurity  
- Build the tree recursively  
- Implement prediction logic  
- Visualize the decision boundary  
- Evaluate model accuracy  

---

## What Is a Decision Tree?

A Decision Tree is a supervised learning algorithm that recursively splits the data based on feature thresholds in order to separate classes.

Each split is chosen to maximize **purity** in the child nodes.

---

## Gini Impurity

The impurity of a node is computed using the **Gini index**:

$$
Gini = 1 - \sum_{k=1}^{K} p_k^2
$$


Where:

- $( p_k )$ is the proportion of samples belonging to class \( k \)  
- A lower Gini value indicates purer groups  
- $( Gini = 0 )$ means the node is perfectly pure  

---

## How the Algorithm Works

1. For every feature, scan all unique thresholds  
2. For each threshold:
   - Split the data into left and right subsets  
   - Compute Gini impurity for both subsets  
   - Compute weighted impurity  
3. Select the threshold with the lowest impurity  
4. Recurse on child nodes  
5. Stop when:
   - A node becomes pure  
   - Maximum depth is reached  
   - Minimum samples condition is met  

---

## Decision Boundary and Model Evaluation

- Accuracy: **1.0**  
- The classifier perfectly separates the two classes on this dataset  
- The boundary is **axis-aligned**, which is characteristic of basic Decision Trees  
- While performance is excellent on this data, Decision Trees can overfit in more complex scenarios  

---

## Summary

- Decision Trees split the feature space using simple threshold rules  
- Gini impurity is used to evaluate the quality of splits  
- The algorithm is interpretable and easy to visualize  
- Axis-aligned boundaries arise naturally from threshold-based splitting  
- Perfect accuracy indicates the model fits this dataset extremely well  

---
##  Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.

