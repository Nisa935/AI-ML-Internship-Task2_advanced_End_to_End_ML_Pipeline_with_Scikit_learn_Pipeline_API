# Customer Churn Prediction using ML Pipeline

## Objective
The objective of this project is to build a reusable and production-ready machine learning pipeline to predict customer churn using the Telco Customer Churn dataset.

---

## Dataset
Telco Customer Churn Dataset

Download link:
https://www.kaggle.com/datasets/blastchar/telco-customer-churn

Note:
Dataset is not included in this repository due to size. Please download it and place it in the project folder before running the code.

---

## Methodology / Approach

1. Data Preprocessing:
   - Removed unnecessary columns (customerID)
   - Handled missing values
   - Converted categorical data into numerical format

2. Pipeline Construction:
   - Used Pipeline and ColumnTransformer
   - Applied StandardScaler for numerical features
   - Applied OneHotEncoder for categorical features

3. Model Training:
   - Logistic Regression
   - Random Forest Classifier

4. Hyperparameter Tuning:
   - Used GridSearchCV for both models

5. Model Evaluation:
   - Accuracy Score
   - F1 Score
   - Classification Report

6. Model Selection:
   - Best model selected based on F1-score

7. Model Export:
   - Saved final pipeline using joblib

---

## Results

| Model                | Accuracy | F1 Score |
|---------------------|----------|----------|
| Logistic Regression | ~0.79    | ~0.56    |
| Random Forest       | ~0.79    | ~0.56    |

Best Model: Logistic Regression

--

## Key Observations

- The dataset is imbalanced, which affects the F1-score.
- Logistic Regression slightly outperformed Random Forest.
- Pipeline ensures a clean, reusable, and production-ready workflow.

---

## Project Structure
