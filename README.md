# 🏦 Loan Approval Prediction

This project builds a machine learning model to predict **loan approval status** based on applicant data using the **Random Forest Classifier**. The dataset is sourced from Kaggle via the `kagglehub` library.

---

## 📁 Dataset

- **Source**: [Kaggle - Loan Approval Prediction Dataset](https://www.kaggle.com/datasets/architsharma01/loan-approval-prediction-dataset)
- **File Used**: `loan_approval_dataset.csv`
- **Target Column**: `loan_status` (encoded)

---

## 📌 Features

The dataset includes various applicant and financial attributes, such as:

- Applicant Income
- Coapplicant Income
- Loan Amount
- Credit History
- Gender, Education, Marital Status (categorical features handled via one-hot encoding)

---

## 🔧 Tools & Libraries Used

- `kagglehub` – to automatically download the dataset
- `pandas` – for data loading and preprocessing
- `sklearn` – for model training and evaluation
  - `RandomForestClassifier`
  - `train_test_split`
  - `LabelEncoder`
  - `classification_report`, `precision_score`, `recall_score`, `f1_score`, `accuracy_score`

---

## 🧠 Model Training

1. **Label Encoding** is applied to the target column.
2. **One-Hot Encoding** is applied to categorical features.
3. Data is split into training and test sets (`80/20` split).
4. **Random Forest Classifier** is trained on the data.

---

## 📊 Evaluation Metrics

After prediction, the model is evaluated using:

- ✅ **Accuracy**
- 🎯 **Precision** (Weighted)
- 🔁 **Recall** (Weighted)
- 🏅 **F1-Score** (Weighted)

---

## 📈 Output Example (Classification Report)
```text
              precision    recall  f1-score   support

      X          0.79       0.85      0.82       100
      Y          0.85       0.78      0.81       120

    accuracy                          0.82       220
   macro avg       0.82       0.82      0.82
weighted avg       0.82       0.82      0.82
