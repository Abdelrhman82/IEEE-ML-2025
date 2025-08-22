# Stroke Prediction

## Project Overview
- The primary objective of this project is to build predictive models to identify patient who are likely to get stroke.
- This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status.
- Each row in the data provides relavant information about the patient.

### Data Description
1) id: unique identifier
2) gender: "Male", "Female" or "Other"
3) age: age of the patient
4) hypertension: 0 if the patient doesn't have hypertension, 1  if the patient has hypertension
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) ever_married: "No" or "Yes"
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) Residence_type: "Rural" or "Urban"
9) avg_glucose_level: average glucose level in blood
10) bmi: body mass index
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12) stroke: 1 if the patient had a stroke or 0 if not

## Exploratory Data Analysis (EDA)
- Generated descriptive statistics for all numerical features.
- Created visualizations to explore distributions and feature relationships.
- Identified key data issues:
  - Positive skewness in feature.
  - Presence of multiple outliers.
  - imbalanced classes

## Data Preprocessing
- **Outliers**: Removed using the **Interquartile Range (IQR)** method.
- **Skewness**: Addressed via **boxcox transformation**.
- **Class imbalance**: Solved using **RandomOverSampler**.

## Modeling
- **Hard Margin SVM**
- **Soft Margin SVM**
  - Linear Kernel
  - RBF Kernel
  - Polynomial Kernel

## Justify the best-performing model
- The best performing model is the multibomial logistic regression without regularization.
- RBF kernel model is the best model with highest test accuracy and highest train accuracy with best f1-score.
