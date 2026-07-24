# 🏦 Bank Customer Churn Classifier (ANN)

An Artificial Neural Network (ANN) classifier built in Python to predict customer churn probability for a banking institution. By identifying high-risk churn customers early, retention teams can proactively intervene with targeted offers.

---

## 🎯 Business Problem & Key Objectives

Customer acquisition costs 5x more than customer retention. The goal of this project is to analyze customer demographic and transactional attributes to predict whether a customer will leave the bank (`Exited = 1`).

- **Target Variable:** `Exited` (0 = Stayed, 1 = Churned)
- **Primary Metric:** Recall & ROC-AUC *(False Negatives are costly—missing a churner means losing a customer)*.

---

## 📊 Dataset & Feature Preprocessing

The dataset consists of **10,000 customer records** across 14 raw attributes:

| Feature Category | Columns Used | Preprocessing Applied |
| :--- | :--- | :--- |
| **Identifiers (Dropped)** | `RowNumber`, `CustomerId`, `Surname` | Removed (non-predictive features) |
| **Categorical** | `Geography`, `Gender` | One-Hot Encoding / Label Encoding |
| **Numerical** | `CreditScore`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary` | Standard Scaling (`StandardScaler`) |

---

## 🧠 Model Architecture

The deep learning model was constructed using a Sequential ANN architecture:

- **Input Layer:** Dense layer with `ReLU` activation (scaled input features).
- **Hidden Layers:** Dense layer(s) with `ReLU` + Batch Normalization / Dropout (to prevent overfitting).
- **Output Layer:** Single neuron with `Sigmoid` activation (outputs probability score between 0 and 1).
- **Optimizer:** Adam
- **Loss Function:** Binary Cross-Entropy

---

## 📈 Key Results & Performance

*(Tip: Replace the placeholder numbers below with your actual model outputs)*

- **Accuracy:** ~86%
- **Precision:** ~0.78
- **Recall:** ~0.68
- **ROC-AUC Score:** ~0.85

> **Key Business Insight:** `Age`, `NumOfProducts`, and `IsActiveMember` emerged as the strongest predictors of customer churn. Older customers with multiple products and low activity had the highest churn risk.

---

# 🏦 Bank Customer Churn Classifier (ANN)

An Artificial Neural Network (ANN) classifier built in Python to predict customer churn probability for a banking institution. By identifying high-risk churn customers early, retention teams can proactively intervene with targeted offers.

---

## 🎯 Business Problem & Key Objectives

Customer acquisition costs 5x more than customer retention. The goal of this project is to analyze customer demographic and transactional attributes to predict whether a customer will leave the bank (`Exited = 1`).

- **Target Variable:** `Exited` (0 = Stayed, 1 = Churned)
- **Primary Metric:** Recall & ROC-AUC *(False Negatives are costly—missing a churner means losing a customer)*.

---

## 📊 Dataset & Feature Preprocessing

The dataset consists of **10,000 customer records** across 14 raw attributes:

| Feature Category | Columns Used | Preprocessing Applied |
| :--- | :--- | :--- |
| **Identifiers (Dropped)** | `RowNumber`, `CustomerId`, `Surname` | Removed (non-predictive features) |
| **Categorical** | `Geography`, `Gender` | One-Hot Encoding / Label Encoding |
| **Numerical** | `CreditScore`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary` | Standard Scaling (`StandardScaler`) |

---

## 🧠 Model Architecture

The deep learning model was constructed using a Sequential ANN architecture:

- **Input Layer:** Dense layer with `ReLU` activation (scaled input features).
- **Hidden Layers:** Dense layer(s) with `ReLU` + Batch Normalization / Dropout (to prevent overfitting).
- **Output Layer:** Single neuron with `Sigmoid` activation (outputs probability score between 0 and 1).
- **Optimizer:** Adam
- **Loss Function:** Binary Cross-Entropy

---

## 📈 Key Results & Performance

*(Tip: Replace the placeholder numbers below with your actual model outputs)*

- **Accuracy:** ~86%
- **Precision:** ~0.78
- **Recall:** ~0.68
- **ROC-AUC Score:** ~0.85

> **Key Business Insight:** `Age`, `NumOfProducts`, and `IsActiveMember` emerged as the strongest predictors of customer churn. Older customers with multiple products and low activity had the highest churn risk.

---

> create a **simple interactive Streamlit web app** where users can input customer details and get a churn probability.

---
