# K-Means Clustering — From Scratch

This folder contains a clean, fully-documented implementation of the **K-Means clustering algorithm**, written entirely from scratch using Python + NumPy — without using scikit-learn.

This notebook is part of the **Machine Learning Algorithms From Scratch** series.

---

## Files Included

- **kmeans.ipynb** — Full step-by-step Notebook  
  Includes:
  - Synthetic dataset generation  
  - K-Means mathematical explanation  
  - Custom implementation using NumPy only  
  - Cluster assignment  
  - Centroid updates  
  - Convergence detection  
  - Final cluster visualization  
  - Centroid plotting  

---

## What is K-Means?

K-Means is an **unsupervised learning algorithm** used to partition data into **K clusters** based on similarity.

The algorithm tries to minimize the **within-cluster variance**, defined as:

$$
J = \sum_{i=1}^{K} \sum_{x \in C_i} \| x - \mu_i \|^2
$$

Where:

- $K$ — number of clusters  
- $C_i$ — cluster $i$  
- $\mu_i$ — centroid of cluster $i$  
- $\| x - \mu_i \|^2$ — squared Euclidean distance  

---

## How K-Means Works

K-Means repeats the following steps until convergence:

1. **Initialize K centroids randomly**  
2. **Assign each point** to the nearest centroid  
3. **Update centroids** as the mean of assigned points  
4. **Check for convergence** (centroids stop changing)

This produces **compact, spherical clusters**.

---

## Visualizations Included

- Unlabeled dataset scatter plot  
- Clustered dataset with color-coded labels  
- Red `X` markers for centroids  
- Clear visualization of cluster separation  

---

## How to Run

1. Open the notebook

2. Run all cells in order.

3. Inspect:
   - Implementation logic  
   - Cluster assignments  
   - Final centroids  
   - Plots and results  

---

## Skills Demonstrated

- Implementing algorithms manually  
- Understanding unsupervised learning  
- Euclidean distance computation  
- Centroid update logic  
- NumPy vectorization  
- Matplotlib visualization  
- Clean and modular notebook design  

---

## Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.
