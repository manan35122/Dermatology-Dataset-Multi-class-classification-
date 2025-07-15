# 🧠 Dermatology Disease Classification with Softmax Regression

This project implements a Softmax Regression (Multinomial Logistic Regression) model to classify dermatological diseases based on clinical and histopathological features.

---

## 📊 Dataset

The dataset used is the **Dermatology Dataset** from the UCI Machine Learning Repository.

- **Features**: 34 attributes (clinical and histopathological), including `age`, `erythema`, `scaling`, `itching`, etc.
- **Target**: Multiclass labels (6 different dermatology conditions)
- **Missing values**: Handled by replacing `"?"` with `NaN` and filling the `age` column with the median.

---

## 🚀 Model Used

- **Algorithm**: Softmax Regression (Multinomial Logistic Regression)
- **Library**: `scikit-learn`
- **Preprocessing**:
  - Converted non-numeric values to `NaN`
  - Filled missing values (`age` → median, others → mean)
  - Normalized features (optional)
- **Training**: Model trained using gradient descent (manual or using `LogisticRegression`)

---

## 📈 Accuracy

Achieved **98.6% accuracy on training data** using `scikit-learn`’s Logistic Regression implementation.  
To validate the model further, consider applying a **train-test split** or cross-validation.

---

## 🛠️ Requirements

```bash
pip install numpy pandas scikit-learn

