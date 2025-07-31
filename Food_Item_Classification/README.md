# Food Item Classification

## Project Overview
- This is dataset contians some informations for 13260 of food items with some features like (Calories, Total Fat, Cholesterol, Sodium, Sugars, Vitamin C, Iron) and a class label to represent the food type.

- The main goal is making models can predict the food type after balance the data to can get better results.

## Exploratory Data Analysis (EDA)
- Generated descriptive statistics for all numerical features.
- Created visualizations to explore distributions and feature relationships.
- Identified key data issues:
  - Positive skewness across features.
  - Presence of multiple outliers.

## Data Preprocessing
- **Outliers**: Removed using the **Interquartile Range (IQR)** method.
- **Skewness**: Addressed via **log transformation**.
- **Class imbalance**: Solved using **SMOTE**.

## Modeling
- **Multinomial Logistic Regression**
  - Ridge
  - Lasso
  - Elastic Net
- **One-vs-Rest Logistic Regression**

## Justify the best-performing model
- The best performing model is the multibomial logistic regression without regularization.
- It get the best acccuracy and f1score.
