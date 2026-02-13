# Iris Flower Classification using Random Forest

## 📌 Problem Statement
Build a Machine Learning model to classify iris flowers into three species:
- Setosa
- Versicolor
- Virginica

based on four features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The model used for classification is **Random Forest Classifier**.

---

## 📊 Dataset Information

- Dataset: Iris Dataset (built-in from scikit-learn)
- Total Samples: 150
- Features: 4 (all numeric)
- Classes: 3

### Target Mapping
- 0 → Setosa
- 1 → Versicolor
- 2 → Virginica

No missing values.
No categorical encoding required.

---

## 🛠 Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn

---

## ⚙️ Steps Performed

1. Import required libraries
2. Load Iris dataset
3. Split dataset into training and testing sets (80/20)
4. Apply StandardScaler for feature scaling
5. Train RandomForestClassifier
6. Evaluate model using:
   - Accuracy Score
   - Classification Report
   - Confusion Matrix
7. Test model on custom sample inputs

---

## 🤖 Model Details

```python
RandomForestClassifier(
    n_estimators=100,
    max_depth=None,
    random_state=42
)
