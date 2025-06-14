# 🧠 Breast Cancer Detection with Random Forest & Hyperparameter Tuning

This project applies **Random Forest Classifier** with **GridSearchCV** to detect whether a tumor is **benign** or **malignant** using the built-in **Breast Cancer dataset** from `scikit-learn`.

---

## Dataset

- Source: `sklearn.datasets.load_breast_cancer()`
- 569 samples, 30 numerical features
- Target classes: `0 = malignant`, `1 = benign`

---

## Workflow

1. Load dataset using `sklearn.datasets`
2. Preprocess and split data using `train_test_split`
3. Train a Random Forest Classifier
4. Apply `GridSearchCV` to tune:
   - `n_estimators`: [50, 100, 150]
   - `max_depth`: [None, 5, 10]
   - `min_samples_split`: [2, 5, 10]
5. Evaluate using:
   - Accuracy score
   - Classification report


