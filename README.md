# Heart Disease Prediction Project

## Project Overview
The goal of this project was to develop a robust predictive model for heart disease using a dataset containing 180 entries and 15 features. Various machine learning algorithms were evaluated, including Logistic Regression, K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), Random Forest, Gradient Boosting, AdaBoost, and XGBoost. This report summarizes their performance and suggests the most suitable model for implementation.

## Dataset Features
The dataset includes the following features:

- **Patient ID**: Unique identifier for each patient.
- **Slope of Peak Exercise ST Segment**: Indicates the slope of the ST segment during peak exercise (1: Upsloping, 2: Flat, 3: Downsloping).
- **Thal**: Type of thalassemia (Normal, Reversible defect, Fixed defect).
- **Resting Blood Pressure**: Blood pressure measured at rest.
- **Chest Pain Type**: Types of chest pain (TA, ATA, NAP, ASY).
- **Number of Major Vessels**: Counts major blood vessels (0 to 3).
- **Fasting Blood Sugar**: Fasting blood sugar levels (1: >120 mg/dL, 0: ≤120 mg/dL).
- **Resting EKG/ECG Result**: Measures the heart's electrical activity (0: Normal, 1: ST-T wave abnormality, 2: Left ventricular hypertrophy).
- **Serum Cholesterol**: Total cholesterol levels in the blood.
- **Oldpeak (ST Depression)**: ST depression induced by exercise.
- **Sex**: Gender of the patient (1: Male, 0: Female).
- **Age**: Age of the patient in years.
- **Max Heart Rate**: Highest heart rate achieved during exercise.
- **Exercise-Induced Angina**: Presence of angina during exercise (0: No, 1: Yes).
- **Heart Disease Present**: Indicates whether heart disease is present (0: No, 1: Yes).

## Data Preprocessing
- **Univariate, Bivariate, and Multivariate Analysis**: Explored feature distributions and relationships.
- **Outlier Removal**: Identified and removed outliers to improve model accuracy.
- **Standardization and SMOTE**: Standardized features and applied SMOTE for class balancing.

## Model Performance Summary

### Evaluated Models

| Model                     | Cross-Validation Accuracy | Test Accuracy | Recall (Heart Disease) | F1-Score (Heart Disease) | AUC Score |
|---------------------------|--------------------------|---------------|------------------------|--------------------------|-----------|
| Logistic Regression       | 83.37%                   | 83.33%        | 78.57%                 | 0.79                     | 0.90      |
| K-Nearest Neighbors (KNN) | 85.93%                   | 88.89%        | 85.71%                 | 0.86                     | 0.95      |
| Support Vector Classifier  | 84.66%                   | 83.33%        | 71.43%                 | 0.77                     | 0.91      |
| Random Forest             | 82.08%                   | 86.11%        | 71.43%                 | 0.80                     | 0.92      |
| Gradient Boosting         | 77.56%                   | 80.56%        | 71.43%                 | 0.74                     | 0.88      |
| AdaBoost                 | 79.48%                   | 80.56%        | 71.43%                 | 0.74                     | 0.78      |
| XGBoost                  | 82.70%                   | 80.56%        | 71.43%                 | 0.74                     | 0.90      |

### Conclusion
KNN was chosen as the best model due to its highest test accuracy (88.89%) and recall (85.71%), making it the most effective for identifying patients at risk for heart disease.

## Challenges Faced
- **Small Dataset Size**: Only 180 entries can lead to overfitting.
  - **Technique Used**: Cross-validation for reliable performance assessment.
  
- **Imbalanced Dataset**: Fewer cases of heart disease can bias models.
  - **Technique Used**: Stratified sampling and adjusted class weights.
  
- **Feature Selection**: Identifying impactful features among 15 columns.
  - **Technique Used**: Analyzed feature importance scores from Random Forest models.
  
- **Overfitting Risk**: Complex models may overfit limited data.
  - **Technique Used**: Cross-validation and hyperparameter tuning to optimize models.
  
- **Evaluation Metrics Selection**: Important for medical diagnostics.
  - **Reason for Emphasizing Recall**: To minimize false negatives, ensuring at-risk individuals are identified.

## Conclusion
KNN is the recommended model for heart disease prediction due to its robust performance metrics. It effectively balances accuracy, recall, and F1-score, making it suitable for clinical applications. Continuous evaluation and model updates are essential to adapt to changing patient data.

## Suggestions for Hospitals to Improve Heart Disease Predictions
- **Implement Predictive Analytics Tools**: Use advanced algorithms and regularly update models.
- **Integrate Health Data Sources**: Combine EHRs, lab results, and data from wearables.
- **Enhance Screening Programs**: Conduct regular risk assessments for high-risk populations.
- **Increase Staff Training**: Educate healthcare professionals on predictive analytics.
- **Patient Education Initiatives**: Inform patients about risk factors and importance of early detection.
- **Develop Decision Support Systems**: Assist providers in making informed decisions based on analytics.
- **Utilize Telehealth Services**: Monitor high-risk patients remotely and provide timely interventions.
- **Community Outreach and Collaboration**: Promote heart health initiatives, especially in underserved areas.
- **Continuous Research and Improvement**: Invest in research to identify new risk factors.

By adopting these strategies, hospitals can enhance predictive capabilities for heart disease, leading to timely interventions and improved patient outcomes.
