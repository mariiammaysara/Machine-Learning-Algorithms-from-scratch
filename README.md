#  ML Algorithms From Scratch

This repository contains a growing collection of **Machine Learning algorithms implemented entirely from scratch** using **Python + NumPy**.  
All implementations include **math explanations, clean code, visualizations**, and step-by-step notebooks (mostly Kaggle Notebooks).

The goal of this repo is to **fully understand how ML works under the hood**, without relying on scikit-learn for the core logic.

---

##  Algorithm Roadmap

- K-Nearest Neighbors
- Linear Regression
- Logistic Regression
- Naive Bayes
- Perceptron
- Support Vector Machine
- Decision Tree
- Random Forest
- Principal Component Analysis
- K-Means Clustering
- AdaBoost
- Linear Discriminant Analysis

Each algorithm has its own folder containing:
- A clean Jupyter notebook (`.ipynb`)
- Math explanation
- From-scratch implementation
- Visualization (where applicable)
- Small README inside the folder

---

##  Repository Structure

```text
Machine-Learning-Algorithms-from-scratch/
│
├── KNN/
│   ├── knn.ipynb
│   └── README.md
│
├── LinearRegression/
│   ├── linear_regression.ipynb
│   └── README.md
│
├── LogisticRegression/
│   ├── logistic_regression.ipynb
│   └── README.md
│
├── NaiveBayes/
│   ├── naive_bayes.ipynb
│   └── README.md
│
├── Perceptron/
│   ├── perceptron.ipynb
│   └── README.md
│
├── SVM/
│   ├── svm.ipynb
│   └── README.md
│
├── DecisionTree/
│   ├── decision_tree.ipynb
│   └── README.md
│
├── RandomForest/
│   ├── random_forest.ipynb
│   └── README.md
│
├── PCA/
│   ├── pca.ipynb
│   └── README.md
│
├── KMeans/
│   ├── kmeans.ipynb
│   └── README.md
│
├── AdaBoost/
│   ├── adaboost.ipynb
│   └── README.md
│
├── LDA/
│   ├── lda.ipynb
│   └── README.md
│
└── README.md   ← Main README for the entire project
```

##  Learning Philosophy

This project follows one core rule:

> **Implement all Machine Learning algorithms manually using NumPy only.**

Other libraries (like scikit-learn) are used **only for:**
- Generating datasets  
- Testing models  
- Comparing results  
- Avoiding unnecessary boilerplate code  

This ensures a strong understanding of:
- The math behind each algorithm  
- Vectorization concepts  
- Optimization behavior  
- Model evaluation techniques  
- Decision boundary intuition  
- Bias–variance dynamics  

---

## Requirements

NumPy — core implementation of all algorithms

Matplotlib — visualizations

Pandas — optional (for loading datasets)

Scikit-learn — only for dataset generation + evaluation

⚠️ Only NumPy is used to implement the algorithms themselves.

## How to Run Algorithms

If running as Python modules:

python -m mlfromscratch.<algorithm-file>


Example:

python -m mlfromscratch.linear_regression


Or simply open the corresponding notebook (recommended):

Kaggle Notebook version

Local Jupyter Notebook version

## Why This Repository?

Build strong intuition for Machine Learning

Understand how algorithms work internally

Practice clean, modular, NumPy-based implementations
