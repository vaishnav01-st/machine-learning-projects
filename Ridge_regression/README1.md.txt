# Ridge Regression on Advertising Dataset

## Problem
Predict **sales** based on advertising budgets spent on **TV, Radio, and Newspaper**.

---

## Dataset
- Source: [Advertising Dataset CSV](https://raw.githubusercontent.com/rkmishracs/dataset/main/advertising.csv)  
- Features: TV, Radio, Newspaper (all numeric)  
- Target: Sales (numeric)

---

## Steps
1. Load dataset with `pandas`.  
2. Split into features `X` and target `y`.  
3. Train/test split (`80/20`).  
4. Scale features with `StandardScaler`.  
5. Train **Ridge Regression** using `GridSearchCV` to find best alpha.  
6. Evaluate model with **MSE** and **R²**.  
7. Make predictions for sample ad budgets.

---

## Sample Predictions

| TV | Radio | Newspaper | Predicted Sales |
|----|-------|-----------|----------------|
| 160 | 50    | 30        | 18.61          |
| 200 | 25    | 15        | 18.20          |
| 100 | 40    | 20        | 15.85          |
| 50  | 30    | 10        | 11.90          |
| 300 | 60    | 50        | 25.30          |

---

## Insight
- TV & Radio budgets strongly influence sales.  
- Ridge regularization with `alpha=20` helps stabilize predictions.  
- Newspaper ads have minimal effect.

---

## How to Run
```bash
pip install pandas scikit-learn
python ridge_advertising.py
