# PHASE1 Census_Income
This analysis focuses on the Census Income Dataset, where the income variable is the target. The goal is to predict whether an individual’s annual income exceeds $50,000 based on demographic and employment attributes.

Dataset Overview
Target Variable: Income 
Data Size: 32,561 rows and 15 columns.
Missing Values: Missing values are represented by ? in the dataset.

Missing values (?) were replaced with NaN.
Imputation techniques were applied to handle the missing values effectively.

Finding Duplicates:
Identified and removed 24 duplicate records using the drop_duplicates() function.
Outlier Detection and Handling:

Detected outliers in numerical features using the  (IQR) method.
Outliers were capped within the acceptable range based on lower and upper bounds.

Exploratory Data Analysis (EDA):

Visualizations were created to analyze feature distributions, relationships between variables

Feature Engineering
Target Variable (y):

The target variable income is categorical.
Converted into numeric using Label Encoding: <=50K as 0 and >50K as 1.

Features (X):

X contains several categorical variables (e.g., workclass, education, occupation).
Converted categorical variables into numerical values using One-Hot Encoding.

Feature Selection
Applied Random Forest Classifier for feature selection to identify the most important predictors of income.
Extracted feature importance scores, ranked the features, and selected the top features contributing significantly to the model's accuracy.
