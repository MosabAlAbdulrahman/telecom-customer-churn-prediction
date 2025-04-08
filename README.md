# 📈 Telecom Customer Churn Prediction

This project focuses on building a machine learning solution to predict customer churn in the telecommunications industry. Churn prediction enables businesses to proactively retain customers by identifying those at high risk of cancellation.

## 🔍 Problem Overview

Customer churn is a costly challenge for telecom companies. Accurately predicting which customers are likely to leave allows for timely intervention through targeted promotions, support, or service improvements.

The goal is to develop and evaluate predictive models using the [Telco Customer Churn dataset](https://www.kaggle.com/blastchar/telco-customer-churn), which includes customer demographics, account info, service usage, and churn status.

---

## ✅ Project Highlights

### 1. **Data Preprocessing**
- Converted data types and handled missing values (`TotalCharges`)
- Encoded categorical features using **Label Encoding** and **One-Hot Encoding**
- Created new features such as `TenureGroup` for improved model performance

### 2. **Exploratory Data Analysis (EDA)**
- Visualized churn distribution across variables (e.g., contract types, payment methods)
- Analyzed correlations between numerical features like `tenure`, `MonthlyCharges`, and `TotalCharges`
- Identified key churn drivers

### 3. **Model Development**
Implemented and evaluated multiple classification models:
- **Logistic Regression** (baseline, with class weighting, with SMOTE)
- **Random Forest Classifier** (baseline, balanced, SMOTE, hyperparameter-tuned with GridSearchCV)
- **XGBoost Classifier** (baseline, with SMOTE, and tuned using GridSearchCV)
- **Artificial Neural Network (ANN)** using TensorFlow/Keras

### 4. **Model Evaluation**
Models were assessed using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrices

### 5. **Hyperparameter Tuning**
- Used **RandomizedSearchCV** and **GridSearchCV** to optimize model performance
- Tuned both Random Forest and XGBoost classifiers extensively

### 6. **Model Deployment**
- Final model (XGBoost) deployed via an intuitive **Gradio** app
- Users can input customer data and receive real-time churn predictions with probability scores
- Deployment script includes custom preprocessing logic to align user input with the trained model’s expected format

---

## 🛠️ Technologies Used

- Python  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn, XGBoost, imbalanced-learn  
- TensorFlow & Keras  
- Gradio (for deployment)  
- Joblib (for model persistence)

---

## 🚀 Try the App

The project includes a Gradio-powered web interface for easy interaction with the trained model. Users can simulate input data and receive churn predictions instantly.

---

## 📂 Project Structure

```
📁 customer-churn-prediction/
├── 📊 Data preprocessing and EDA
├── 🤖 Model training and evaluation
├── 🔍 Hyperparameter tuning
├── 🌐 Deployment (Gradio interface)
├── 📈 Performance comparison visualization
└── 📦 Model persistence (.pkl)
```

---

## 📌 Key Takeaways

- End-to-end implementation of a real-world classification problem
- Emphasis on class imbalance handling (via SMOTE, class weights)
- Strong focus on model interpretability and deployment readiness
- A comparative study of classical ML models vs. ANN in churn prediction

