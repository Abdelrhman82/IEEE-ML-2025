# Titanic Survivle Classificsation

## Project Overview
- The primary objective of this project is to build predictive models to identify passenger who are likely to survive from the Titanic incident.
- By analyzing passenger features, the project aims to:

  - Explore and preprocess the data.
  - Use the tree-based models.

### Data Description
This dataset is the Titanic dataset with the following characteristics:

- Size: 891 rows × 12 columns.

- Features:

    - PassengerId – unique identifier.
    - Pclass – passenger class (1st, 2nd, 3rd).
    - Name – passenger’s full name.
    - Sex – gender.
    - Age – age in years.
    - SibSp – number of siblings/spouses aboard.
    - Parch – number of parents/children aboard.
    - Ticket – ticket number.
    - Fare – ticket price.
    - Cabin – cabin number.
    - Embarked – port of embarkation (C, Q, S).

- Target:

    - Survived (0 = No, 1 = Yes).

## Exploratory Data Analysis (EDA)
- Generated descriptive statistics for all numerical features.
- Created visualizations to explore distributions and feature relationships.
- Identified key data issues:
  - Positive skewness in feature.
  - Presence of multiple outliers.
  - imbalanced classes

## Data Preprocessing
- **Outliers**: Removed using the **Interquartile Range (IQR)** method.
- **Skewness**: Addressed via **log transformation**.
- **Class imbalance**: Solved using **Class_weight**.

## Modeling
- **logistic Regression** (BaseLine)
- **Tree based methods**
  - Decision Tree
  - Random Forest
  - Xgboost

## Justify the best-performing model
- The best results can got, it's also has overfitted
- improvements can do is add more data
