# 🧠 Employee Salary Classification

A machine learning project to predict whether an individual's income exceeds $50K/year based on demographic and employment attributes from the Adult Dataset.

---

## 📁 Dataset

Features:
- Age  
- Workclass  
- Education / Education-Num  
- Marital Status  
- Occupation  
- Relationship  
- Race  
- Gender  
- Capital Gain / Loss  
- Hours per Week  
- Native Country  
- **Income** (target variable: `>50K` or `<=50K`)

---

## 🎯 Objectives

- Clean and preprocess dataset for ML  
- Train various classification models  
- Evaluate model performance and metrics  
- Save and deploy best model via web interface

---

## 🔧 Project Workflow

### 1️⃣ Data Preprocessing
- Replace `?` with NaN and drop missing rows  
- Encode categorical features using LabelEncoder  
- Scale numerical features using MinMaxScaler  

### 2️⃣ Model Training & Evaluation
Models used:
- K-Nearest Neighbors (KNN)  
- Logistic Regression  
- Support Vector Classifier (SVC)  
- Random Forest  
- Gradient Boosting  
- MLP Classifier (Neural Network)

> ✅ **Best-performing model**: Gradient Boosting (Accuracy ≈ 87.22%)

### 3️⃣ Saving Model
- Saved trained model: `retrained_best_model.pkl`  
- Saved scaler: `scaler_retrained.pkl`

---

## 🌐 Streamlit Web Application

### Features:
- Interactive form-based input for individual prediction  
- Batch predictions from uploaded CSV file  
- Displays prediction results and confidence scores

### Deployment:
- Hosted locally using Streamlit  
- Shared publicly using **ngrok**

---

## 📊 Results
- Gradient Boosting Classifier achieved highest accuracy (~87.22%)  
- Robust and responsive UI supports both real-time and batch predictions  
- Project ready for deployment and further enhancement

---
## 🚀 Access the Web App

You can try the Employee Salary Classification tool online via the Streamlit interface:  
🔗 https://e61718c1b6c6.ngrok-free.app

> Note: This app is hosted locally via Streamlit and made publicly available using ngrok. The URL may change each time the server restarts.

