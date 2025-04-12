# 🧠 Customer Churn Prediction - American Express Credit Card

This project predicts **customer churn** for American Express credit card users using a **Random Forest Classifier**, with complete preprocessing, evaluation, and visualizations done using **Matplotlib**.

---

## 📌 Problem Statement

Credit card companies face significant losses due to customer churn. Identifying potential churners early helps in targeted retention strategies.

This project:
- Analyzes customer data
- Builds a machine learning model to predict churn (`Closed = 1`)
- Visualizes data insights and evaluation metrics

---

## 📁 Dataset Info

The dataset contains fields related to customer demographics, account history, and credit activity.

### 🔑 Features:
- `Credit Score` (numerical)
- `Geography` (categorical)
- `Gender` (categorical)
- `Age` (numerical)
- `Customer Since` (numerical)
- `Current Account` (numerical)
- `Num of products` (numerical)
- `UPI Enabled` (binary)
- `Estimated Yearly Income` (numerical)

### 🎯 Target:
- `Closed`: 
  - `0` → Active customer
  - `1` → Churned customer

---

## ⚙️ Workflow

### 1. **Data Cleaning**
- Null values handled:
  - Numerical columns → median imputation
  - Categorical columns → mode imputation
  - Rows with null target dropped

### 2. **Encoding**
- `Gender` and `Geography` encoded using one-hot encoding

### 3. **Exploratory Data Analysis**
Visualized using `matplotlib`:
- Churn distribution bar chart
- Correlation heatmap
- Feature importance chart
- Confusion matrix

### 4. **Modeling**
- **Random Forest Classifier**
- Train-test split: 80/20 stratified

---

## 📊 Classification Metrics

| Metric               | Score   |
|----------------------|---------|
| Accuracy             | 0.89    |
| Precision            | 0.85    |
| Recall               | 0.88    |
| F1 Score             | 0.86    |
| ROC AUC Score        | 0.93    |

> *Scores may vary slightly depending on random state or test size*

---

## 📈 Visualizations

| Visualization             | Description                                  |
|---------------------------|----------------------------------------------|
| 📉 Churn Distribution      | Bar chart of active vs churned customers     |
| 🔗 Correlation Heatmap     | Feature-to-feature correlation map           |
| 🌲 Feature Importances     | Top 10 influential features in model         |
| 🧮 Confusion Matrix        | Actual vs Predicted breakdown (matplotlib)   |

---

## 💡 Future Improvements
- Build a web interface using **Streamlit** for live predictions
- Add feature selection or hyperparameter tuning (GridSearchCV)
- Train and compare with XGBoost/ANN

