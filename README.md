# 🩺 Diabetes Prediction using Machine Learning

This project is part of **GTC ML Project 2**, where we build and evaluate machine learning models to predict whether a patient is **Diabetic** or **Non-Diabetic** based on diagnostic measurements.

---

## 📊 Dataset
- Source: `diabetes.csv` (Pima Indians Diabetes Dataset).
- Target variable: **Outcome**
  - `0` → Non-Diabetic
  - `1` → Diabetic

### Features:
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

---

## 🚀 Project Workflow

### Phase 1: Exploratory Data Analysis (EDA)
- Checked class balance (Diabetic vs Non-Diabetic).
- Visualized the relationship between **Glucose**, **BMI**, and **Outcome**.
- Generated correlation heatmaps and summary statistics.

### Phase 2: Data Preparation
- Standardized all features using `StandardScaler`.
- Split dataset into **train (80%)** and **test (20%)** sets with stratification.

### Phase 3: Modeling & Evaluation
Implemented and compared three models:
1. **Logistic Regression**  
2. **Support Vector Machine (SVM)** with GridSearchCV  
3. **Random Forest** with GridSearchCV  

### Phase 4: Prediction Function
- Created a `predict_diabetes()` function that:
  - Accepts patient data as input.
  - Returns prediction (`Diabetic` or `Non-Diabetic`).
- Tested the function with different **example patients**:
  - Clear Diabetic case.
  - Clear Non-Diabetic case.
  - Borderline / Confusing cases.

---

## 📈 Results

### Logistic Regression
- Accuracy: **71%**
- Precision (Diabetic): 0.61
- Recall (Diabetic): 0.52
- F1-score (Diabetic): 0.56

### Support Vector Machine (SVM)
- Accuracy: **73%**
- Precision (Diabetic): 0.65
- Recall (Diabetic): 0.52
- F1-score (Diabetic): 0.58

### Random Forest
- Accuracy: **75%**
- Precision (Diabetic): 0.65
- Recall (Diabetic): 0.61
- F1-score (Diabetic): 0.63

---

## ⚙️ Technologies Used
- Python 3.x
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
