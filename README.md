# Employee Attrition Prediction using Machine Learning

## Overview

This project was completed as part of a Kaggle competition assignment during a program at IIM-Indore. The objective of this classification problem is to predict employee attrition based on comprehensive data, including demographic information, job-related details, and satisfaction scores.

The dataset consists of 1,677 observations used for training the model and predicting attrition for 1,119 observations. There are over 30 independent variables in the dataset, making it a challenging task. However, this project provided valuable insights into feature selection and data preprocessing techniques.

## Data Cleaning and Preprocessing

Handling a diverse set of independent variables required extensive data cleaning and preprocessing. Several steps were taken to prepare the data for modeling:

- **Feature Selection**: Variables like 'Over18,' which capture whether the employee is over 18 years of age, were removed since they were homogenous and didn't provide meaningful information.

- **Outlier Handling**: Outliers in both continuous and categorical variables were addressed to ensure the model's robustness.

- **Data Entry Errors**: Data entry errors, such as an education level of 15 with only one observation while all others were between 1 and 5, were identified and corrected.

- **Data Scaling**: LabelEncoder, StandardScaler, and MinMaxScaler from the sklearn.preprocessing library were used for data preprocessing. LabelEncoding and One-Hot Encoding were used for categorical variables, and MinMaxScaler was used for scaling continuous variables.

## Model Training and Testing

Multiple machine learning models were trained and tested on the preprocessed data. The Logistic Regression model achieved the highest accuracy score of over 80%. Other models were also evaluated, including Random Forest Classifier and Decision Tree Classifier.

## Results

The model achieved a correct prediction rate of around 75% on the validation data. However, it performed even better on the total test cases, with an accuracy of over 80%. This accuracy rate ranked as the second-highest among all participants in the competition for predicting attrition.

<img width="876" alt="Screenshot 2023-06-15 at 8 43 53 AM" src="https://github.com/AnkitBaliyan1/attrition_prediction/assets/86275544/ba7223bd-9c21-48fe-aa70-38fef475ade2">

This project demonstrates the effectiveness of machine learning in predicting employee attrition and highlights the importance of data preprocessing and feature selection in achieving accurate results.

