# Python-projects-
Credit Approval Prediction
 # Project Title:
Credit Card Approval Prediction System using Machine Learning

# Objective:
To build a machine learning model that can accurately predict whether a credit card application should be approved or rejected based on applicant data such as income, employment status, credit history, and other demographic and financial attributes.

# Problem Statement:
Financial institutions receive a high volume of credit card applications and must evaluate each applicant’s creditworthiness. Traditionally, this process has been manual or rule-based, which can be time-consuming and prone to bias.
The goal of this project is to develop an automated, data-driven system that predicts the approval status of credit card applications to help banks reduce processing time, minimize defaults, and enhance decision-making.

# Step-by-Step Breakdown:
# 1. Import Required Libraries
Import essential Python libraries: pandas, numpy, sklearn, seaborn, matplotlib, joblib for data processing, visualization, modeling, and persistence.

# 2. Load Dataset
Load two CSV files:

application_record.csv: Contains demographic and financial details of applicants.

credit_record.csv: Contains credit behavior data over time.

# 3. Data Cleaning & Preprocessing
Remove duplicate records using unique ID.

Handle categorical variables using LabelEncoder.

Clean the STATUS column in the credit record by replacing missing or ambiguous values.

Create a new binary label Approved:

1: Eligible for approval.

0: Likely to default or reject.

# 4. Merge Datasets
Merge the application and credit datasets using the ID column.

Drop ID post-merge as it's no longer required.

# 5. Feature Scaling and Data Splitting
Standardize features using StandardScaler.

Split the data into training and test sets (80:20 split) using stratified sampling to preserve class balance.

# 6. Model Training
Train a RandomForestClassifier as the base model for classification.

Fit the model on the training data.

# 7. Model Evaluation
Predict on the test set.

Evaluate performance using:

Classification report (precision, recall, F1-score)

Confusion matrix

ROC-AUC score

# 8. Model Persistence
Save the trained model and scaler using joblib to reuse for deployment or predictions on new data.

# 9. Visualizations
Plot class distribution using seaborn.

Display feature importances from the trained Random Forest model to understand which features influence predictions most
