# Lasso Regression on Student Scores Dataset

## Problem
Predict **student exam scores** based on the **number of hours studied** using **Lasso regression**.

---

## Dataset
- Source: [Student Scores CSV](https://raw.githubusercontent.com/AdiPersonalWorks/Random/master/student_scores%20-%20student_scores.csv)  
- Features:  
  - `Hours` → number of hours studied (numeric)  
- Target:  
  - `Scores` → exam score (numeric)  
- Rows: ~25  

✅ All numeric, no encoding required.

---

## Steps
1. Load dataset with `pandas`.  
2. Split features (`X`) and target (`y`).  
3. Train/test split (80/20).  
4. Scale features with `StandardScaler` (optional, but recommended).  
5. Train **Lasso regression** with hyperparameter `alpha`.  
6. Evaluate model using **Mean Squared Error (MSE)** and **R² score**.  
7. Make predictions for sample study hours.

---

## Sample Predictions

| Hours | Predicted Score |
|-------|----------------|
| 2     | 21.5           |
| 4     | 42.7           |
| 6     | 64.0           |
| 8     | 85.2           |
| 9.25  | 96.8           |

---

## Insights
- Exam scores increase approximately linearly with hours studied.  
- **Lasso regression** can shrink the coefficient to reduce overfitting if dataset grows larger.  

---