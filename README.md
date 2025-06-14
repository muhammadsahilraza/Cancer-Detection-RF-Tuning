# Breast Cancer Detection with Random Forest & Hyperparameter Tuning

This project uses a **Random Forest Classifier** with **GridSearchCV** to classify breast tumors as **benign** or **malignant**, based on the **Breast Cancer Wisconsin (Diagnostic) Dataset** from **Kaggle**.

---

## Dataset

- Source: [Kaggle - Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- 569 samples, 30 features (e.g. radius, texture, perimeter)
- Diagnosis labels:
  - `M = Malignant`
  - `B = Benign`  
- Converted to:
  - `1 = Malignant`
  - `0 = Benign`

---

## Workflow

1.Load the dataset from CSV
2. Preprocess: drop unnecessary columns and map target labels
3. Split data into training/testing sets
4. Train a Random Forest model
5. Apply `GridSearchCV` to tune:
   - `n_estimators`: [50, 100, 150]
   - `max_depth`: [None, 5, 10]
   - `min_samples_split`: [2, 5, 10]
6. Evaluate using:
   - Accuracy score
   - Classification report


