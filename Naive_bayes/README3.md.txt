# Naive Bayes Classification on Student Scores Dataset

## Problem
Predict whether a student **Passes or Fails** based on **hours studied** using **Naive Bayes classification**.

---

## Dataset
- Source: [Student Scores CSV](https://raw.githubusercontent.com/AdiPersonalWorks/Random/master/student_scores%20-%20student_scores.csv)  
- Feature:  
  - `Hours` → number of hours studied (numeric)  
- Target:  
  - `Pass` → 1 if score ≥ 50, else 0  
- Rows: ~25  

✅ All numeric features, no encoding required.  

---

## Steps
1. Load dataset with `pandas`.  
2. Convert `Scores` → `Pass/Fail` (1 = Pass, 0 = Fail).  
3. Split data into features `X` and target `y`.  
4. Perform train/test split (80/20).  
5. Train **Gaussian Naive Bayes** model (`GaussianNB`).  
6. Make predictions on test data or new samples.  
7. Evaluate model using **accuracy** and **classification report**.

---

## Sample Predictions

| Hours Studied | Predicted Outcome |
|---------------|-----------------|
| 4             | Fail (0)        |
| 6             | Pass (1)        |
| 8             | Pass (1)        |

---

## Insights
- Students studying fewer hours are more likely to **Fail**.  
- Students studying more hours are more likely to **Pass**.  
- Naive Bayes works well here because **feature distribution is roughly Gaussian**.  

---


