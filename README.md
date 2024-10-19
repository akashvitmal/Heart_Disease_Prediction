# Heart Disease Prediction Project

## Overview
This project focuses on developing a predictive model for heart disease using a dataset with 180 samples and 15 features. We analyzed various machine learning algorithms, including Logistic Regression, K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), and Random Forest.

## Dataset Features
The dataset includes the following features:
- **Patient ID:** Unique identifier for each patient.
- **Slope of ST Segment:** Slope of the ST segment during peak exercise.
- **Thal:** Type of thalassemia.
- **Blood Pressure:** Resting blood pressure.
- **Chest Pain Type:** Classification of chest pain.
- **Major Vessels:** Count of major blood vessels.
- **Fasting Blood Sugar:** Levels of fasting blood sugar.
- **EKG Result:** Resting EKG results.
- **Cholesterol:** Total cholesterol levels.
- **Oldpeak:** ST depression during exercise.
- **Sex:** Gender of the patient.
- **Age:** Age of the patient.
- **Max Heart Rate:** Highest heart rate achieved during exercise.
- **Angina:** Exercise-induced angina.
- **Heart Disease Present:** Target variable indicating presence of heart disease.

## Model Performance Summary
The evaluation of models yielded the following results:
- **Logistic Regression:** 
  - Accuracy: 83.33%, Recall: 78.57%
  
- **KNN:** 
  - Accuracy: **88.89%**, Recall: **85.71%**
  
- **SVC:** 
  - Accuracy: 83.33%, Recall: 71.43%
  
- **Random Forest:** 
  - Accuracy: 86.11%, Recall: 71.43%

**Best Model:** KNN was selected for implementation due to its superior performance in accuracy and recall.

## Challenges Faced
- **Small Dataset Size:** Utilized cross-validation to improve reliability.
- **Imbalanced Dataset:** Applied stratified sampling and adjusted class weights.
- **Overfitting Risk:** Conducted hyperparameter tuning to optimize model settings.

## Conclusion
KNN emerged as the most effective model for predicting heart disease, offering a balance of accuracy, recall, and F1-score. Ongoing evaluation and updates will be necessary to maintain model effectiveness.
