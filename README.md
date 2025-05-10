# Normalization in Machine Learning

This notebook demonstrates the concept and application of **Normalization**, a feature scaling technique used in data preprocessing.

---

## 📘 What is Normalization?

Normalization transforms the values of features to a common scale, typically in the range **[0, 1]**. Unlike standardization (which centers the data around the mean), normalization is useful when:
- You do **not assume** data is normally distributed.
- You want all features to have **equal importance** regardless of their original scale.

---

## 🧠 Why Use Normalization?

Some machine learning models (like K-Nearest Neighbors, Neural Networks, and Gradient Descent-based algorithms) perform **better and faster** when features are on the same scale.

Normalization helps:
- Avoid bias toward features with larger ranges.
- Improve convergence time for optimization algorithms.
- Enhance model accuracy and interpretability.

---

## 🛠️ Tools Used

- `pandas` for data handling
- `numpy` for numerical operations
- `sklearn.preprocessing.MinMaxScaler` for normalization

---

## 🚀 How to Use

1. Load your dataset.
2. Import `MinMaxScaler` from `sklearn.preprocessing`.
3. Fit and transform your dataset using the scaler.

Example:
```python
from sklearn.preprocessing import MinMaxScaler

scaler = MinMaxScaler()
normalized_data = scaler.fit_transform(original_data)
