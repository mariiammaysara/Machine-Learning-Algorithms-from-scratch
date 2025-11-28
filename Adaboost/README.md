# AdaBoost — From Scratch

This folder contains a clean, fully-documented implementation of the **AdaBoost (Adaptive Boosting)** algorithm written entirely from scratch using Python + NumPy — without using scikit-learn.

Part of the **Machine Learning Algorithms From Scratch** series.

---

## What is AdaBoost?

AdaBoost is a **boosting algorithm** that combines multiple **weak learners** (usually decision stumps) into one **strong classifier**.

Final model:

$$
F(x) = \sum_{t=1}^{T} \alpha_t h_t(x)
$$

Where:

- $h_t(x)$ — prediction of weak learner (decision stump)  
- $\alpha_t$ — weight of the weak learner  
- $T$ — number of boosting rounds  

### Weight Update Rule

After each stump, sample weights are updated:

$$
w_i \leftarrow w_i \exp(-\alpha_t y_i h_t(x_i))
$$

Misclassified samples receive **higher weights**, forcing the next stump to focus on them.

---

## Files Included

- **adaboost.ipynb** — full step-by-step notebook:
  - Synthetic non-linear dataset  
  - Decision stump implementation  
  - Boosting loop  
  - Weight updates  
  - Strong classifier output  
  - Decision boundary visualization  
  - Accuracy evaluation  

---

## Algorithm Steps

1. Initialize sample weights equally  
2. Train a weak learner (decision stump)  
3. Compute weighted classification error  
4. Compute stump weight:

$$
\alpha_t = \frac{1}{2} \ln \left( \frac{1 - \epsilon_t}{\epsilon_t} \right)
$$

5. Update sample weights  
6. Normalize weights  
7. Repeat for T rounds  

---

## Visualizations Included

- Dataset scatter plot  
- Boosted decision boundary  
- Points colored by predicted class  

Example (from notebook):

- AdaBoost Accuracy: **0.96**  
- Clearly separable boosted decision regions  

---

## Skills Demonstrated

- Implementing boosting algorithms manually  
- Understanding weak vs strong learners  
- Exponential weight updates  
- Decision stump logic  
- Matplotlib visualization  
- Clean, modular coding structure  
- NumPy vectorization  

---

## How to Run

1. Open `adaboost.ipynb`  
2. Run all cells sequentially  
3. Inspect:
   - Boosting rounds  
   - Stump behavior  
   - Final classifier  
   - Decision boundary  

---

## Author

Created by **Mariam Maysara**  
Part of the *Machine Learning Algorithms From Scratch* series.
