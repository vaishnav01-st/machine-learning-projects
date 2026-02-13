# KNN & Naive Bayes Classification on Social Network Ads

## Problem
Predict whether a user will **purchase a product** based on **Age** and **Estimated Salary** using **KNN or Naive Bayes classification**.

---

## Dataset
- Source: [Social Network Ads CSV](https://huggingface.co/datasets/Rodrigopiva/Social_Network_Ads.csv)  
- Features:  
  - `Age` → Age of the user (numeric)  
  - `EstimatedSalary` → Salary of the user (numeric)  
- Target:  
  - `Purchased` → 1 if product purchased, else 0  
- Rows: ~400  

✅ All numeric features, no encoding required for `Age` and `EstimatedSalary`.

---

## Steps
1. Load dataset using `pandas`.  
2. Extract features `X` = [`Age`, `EstimatedSalary`] and target `y` = `Purchased`.  
3. Split data into training and testing sets (typically 75/25).  
4. Scale features using `StandardScaler` (important for KNN).  
5. Train model:  
   - **KNN:** `KNeighborsClassifier`  
   - **Naive Bayes:** `GaussianNB`  
6. Make predictions on test data or new sample inputs.  
7. Evaluate model using **accuracy** and **confusion matrix**.  
8. Optional: Plot **decision boundaries** for training and test sets using `matplotlib`.

---

## Sample Predictions

| Age | Estimated Salary | Predicted Outcome |
|-----|-----------------|-----------------|
| 22  | 19000           | No (0)          |
| 35  | 20000           | No (0)          |
| 47  | 43000           | Yes (1)         |
| 50  | 70000           | Yes (1)         |
| 30  | 87000           | Yes (1)         |

---

## Insights
- Users with lower age and salary are less likely to **purchase** the product.  
- Users with higher age or higher salary are more likely to **purchase**.  
- KNN relies on **distance between data points**, so feature scaling is crucial.  
- Naive Bayes assumes features are **conditionally independent**; works well with numeric features.

---

