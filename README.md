# 🩺 Diabetes Prediction with KNN

Predicting diabetes using **K-Nearest Neighbors (KNN)** on the **Pima Indians Diabetes Dataset**.  
This project demonstrates a full machine learning workflow: from data cleaning to model evaluation.

---

## 📊 Dataset
- **Source**: National Institute of Diabetes and Digestive and Kidney Diseases (via UCI / Kaggle)
- **Rows**: 768 patients
- **Features**:
  - Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age
- **Target**: Outcome (0 = No Diabetes, 1 = Diabetes)
- **Challenge**: Missing values (zeros treated as NaN), moderate class imbalance (~65/35)

---

## ⚙️ Workflow
1. Exploratory Data Analysis (EDA)
2. Data cleaning & preprocessing  
   - Handle missing values  
   - Scaling for KNN  
3. Train/test split (stratified)
4. Baseline KNN model
5. Cross-validation (ROC-AUC)
6. Hyperparameter tuning with GridSearchCV
7. Model evaluation (confusion matrix, ROC curve, precision-recall curve)
8. Threshold adjustment for recall

---

## 🔑 Results
- **Accuracy**: 77%  
- **ROC-AUC**: 0.81 (good discriminatory power)  
- **Recall (diabetes cases)**: 0.60 → improved via threshold tuning  

---

## 📂 Project Structure
- `diabetes_knn_classification.ipynb` → notebook
- `requirements.txt` → dependencies
- `README.md` → project overview

---

## 🚀 Next Steps
- Compare with Logistic Regression & Random Forest
- Feature engineering (interaction terms, polynomial features)
- Threshold optimization for medical use cases
