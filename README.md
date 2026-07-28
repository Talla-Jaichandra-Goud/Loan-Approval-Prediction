# Loan Approval Prediction using Classification Algorithms

A machine learning project focused on predicting whether a loan application will be **Approved** or **Rejected** by leveraging classification algorithms trained on applicant financial details, credit history, and asset information.

---

# 📌 Project Overview

This project implements a complete end-to-end Machine Learning workflow for loan approval prediction. It includes data preprocessing, exploratory data analysis (EDA), feature engineering, feature scaling, model building using multiple classification algorithms, hyperparameter tuning, and model evaluation. The objective is to assist financial institutions in making faster, more consistent, and data-driven loan approval decisions.

---

# 🧰 Tech Stack

**Language:** Python

**Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost

**Environment:** Jupyter Notebook

---

# 🔄 Workflow Summary

## 1. Data Collection

The dataset contains loan application records with applicant and financial information, including:
Number of Dependents, Education, Self Employed Status, Annual Income, Loan Amount, Loan Term, CIBIL Score, Residential Asset Value, Commercial Asset Value, Luxury Asset Value, Bank Asset Value, Loan Status (Target Variable)

---

## 2. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand the characteristics of the dataset.

* Analysed feature distributions
* Checked missing values and duplicate records
* Identified outliers in numerical features
* Visualised relationships between variables
* Generated correlation matrix for numerical features
* Compared feature distributions across loan approval status

---

## 3. Feature Engineering

Prepared the dataset for machine learning by:

* Cleaning and standardising column names
* Encoding categorical variables
* Creating additional features such as Total Asset Value
* Scaling numerical features using StandardScaler and RobustScaler
* Splitting the dataset into training and testing sets

---

## 4. Modelling

Classification algorithms used:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* K-Nearest Neighbors (KNN)
* XGBoost Classifier

Hyperparameter tuning was performed using **RandomizedSearchCV** to optimise the Random Forest model.

---

## 5. Evaluation

Models were evaluated using the following classification metrics:

* Accuracy Score
* F1 Score
* ROC-AUC Score
* Confusion Matrix
* Classification Report
* Cross Validation

**Result:** The tuned Random Forest model delivered the best overall performance and was selected as the final prediction model.

---

## 6. Prediction & Insights

The trained model predicts whether a loan application is likely to be approved or rejected based on applicant information.

Key insights obtained from the analysis include:

* Applicants with higher CIBIL scores have a significantly higher probability of loan approval.
* Income, loan amount, and total asset value strongly influence lending decisions.
* Tree-based models captured complex relationships better than linear models.
* Hyperparameter tuning improved model performance and generalisation capability.

---

# 📁 Project Structure

```text
Loan-Approval-Prediction/
│── Loan_Approval_prediction.ipynb
│── loan_approval_dataset.csv
│── README.md
│── requirements.txt
```

---

# 📈 Key Findings

* CIBIL score is one of the most influential factors in predicting loan approval.
* Applicants with higher income and stronger asset portfolios are more likely to receive loan approval.
* Random Forest outperformed other classification models by effectively capturing non-linear relationships in the data.
* Feature engineering and proper data preprocessing significantly improved prediction accuracy.

---

# 🚀 Future Improvements

* Deploy the model as a web application using Streamlit or Flask.
* Integrate real-time loan application prediction through an interactive user interface.
* Apply Explainable AI techniques such as SHAP or LIME to improve model transparency.
* Experiment with advanced ensemble methods such as LightGBM and CatBoost.
* Continuously retrain the model with new loan application data to improve long-term performance.

