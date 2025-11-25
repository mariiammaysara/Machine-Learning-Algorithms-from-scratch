#  K-Nearest Neighbors (KNN) — From Scratch

This folder contains a clean, fully-documented implementation of the **K-Nearest Neighbors (KNN)** algorithm written entirely from scratch using **Python + NumPy**, without relying on scikit-learn.

---

##  Files Included
- **`knn.ipynb`** — Step-by-step Kaggle notebook  
- Implementation of:
  - Euclidean distance  
  - Custom KNN classifier  
  - Train/Test split  
  - Accuracy evaluation  
  - Decision boundary visualization  

---

##  Overview: What is KNN?

**KNN** is a simple, intuitive, non-parametric machine learning algorithm used for classification.

Instead of “training” a model, KNN works by:
1. Measuring distance between the query point and every training sample  
2. Selecting the **K closest points**  
3. Taking a **majority vote** among their labels  
4. Returning the predicted label  

This makes KNN:
- Easy to understand  
- Highly interpretable  
- Effective for small datasets  
- Sensitive to noise and feature scaling  

---

## Math Behind KNN

We use the **Euclidean distance**:

$$
d = \sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}
$$

Implemented manually using NumPy.


---

##  Visualizations Included
The notebook includes:
- Scatter plot of the dataset  
- Color-coded class separation  
- Smooth, high-resolution **decision boundary**  
- Train vs Test point visualization  

---

##  How to Run
1. Open the notebook:  
   **`knn.ipynb`**
2. Run all cells in order  
3. Review:
   - Implementation  
   - Results  
   - Visualizations  

---

##  Skills Demonstrated
- Writing ML algorithms **from scratch**  
- NumPy vectorization  
- Understanding distance metrics  
- Model evaluation  
- Clean and modular code structure  
- Data visualization with Matplotlib  

---

