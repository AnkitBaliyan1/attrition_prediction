# attrition_prediction_using_ML_tools

The project was part of Kaggle competition assignment completed during program at IIM-Indore. This classification problem aims to predict the attrition based on comprehensive data of demography, job related details along with satisfaction score. 

The dataset of 1677 observations was to train the model and predict for 1119 observations with over 30 independent variables. The diverse set of independent variables was indeed tough to handled but feature selection was an important learning from here. 

Variables like ‘Over18’ which capture if the employee is over 18 year of age, which was removed since it was homogenous. And yes, that make sense also, as legal age for work is over 18. 

Other data cleaning and preprocessing task were required to handle not only outliers but also avoid using some observations with really does not make sense for particular variable. One such variable was “Education”. Education level 15 doesn’t make sense with only 1 observation when all other observation were between 1 and 5. For sure, this was an error entry. 

LabelEncoder, StandardScaler and MinMaxScaler from sklearn.preprocessing library were used for data-preprocessing.

Handling abnormal observation for both continuous and categorical variable was not easy. Using Label Encoding and One Hot Encoding for the categorical and MinMaxScaler technique for scaling the continuous variables, I was able to finish the data-preprocessing. 

Multiple model were trained and tested, but LogisticRegression model fetched the best accuracy score of over 80%
Various models trained and tested: 
  1. LogisticRegression
  2. Random Forest Classifier
  3. Decision Tree Classifier


The model predicted correct for around 75% of validation data but it performed better with over 80% accuracy on total test cases. This was 2nd highest accuracy in predicting the attrition of all participating for this competition. 

<img width="876" alt="Screenshot 2023-06-15 at 8 43 53 AM" src="https://github.com/AnkitBaliyan1/attrition_prediction/assets/86275544/ba7223bd-9c21-48fe-aa70-38fef475ade2">
