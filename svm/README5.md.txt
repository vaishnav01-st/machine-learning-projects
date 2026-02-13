# Iris Flower Classification using SVM

## Problem
Predict the **species of an Iris flower** (Setosa, Versicolor, Virginica) based on its **sepal and petal measurements** using a **Support Vector Machine (SVM)** classifier.

---

## Dataset
- **Source:** Built-in Iris dataset from `scikit-learn`  
- **Samples:** 150  
- **Features:**  
  1. Sepal Length (cm)  
  2. Sepal Width (cm)  
  3. Petal Length (cm)  
  4. Petal Width (cm)  
- **Target Classes:**  
  - 0 → Setosa  
  - 1 → Versicolor  
  - 2 → Virginica  

✅ All features are numeric, no encoding required.

---

## Steps

1. Load the Iris dataset using `scikit-learn`.  
2. Separate features `X` and target labels `y`.  
3. Split data into **training** and **testing** sets (typically 80/20).  
4. Scale features using `StandardScaler` (important for SVM).  
5. Train **SVM model**:  
```python
from sklearn.svm import SVC
model = SVC(kernel='linear', C=1.0, random_state=42)
model.fit(X_train_scaled, y_train)
