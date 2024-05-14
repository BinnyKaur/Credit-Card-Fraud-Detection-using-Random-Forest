# Credit-Card-Fraud-Detection-using-Random-Forest
#Overview
This project explores credit card dataset, apply some data exploration techniques and builds a predictive model at the end. 

#Dataset
The Dataset used for this project is obtained from Kaggle.It includes transactions made by European Cardholders in September 2013. This dataset presents transactions that occured in two days with 492 fraud transactions out of 284,807 total transactions. 

#Data Attributes 
1. V1,V2,V3....V28 are principal components obtained through prinicipal component analysis
2. Time is the seconds elapsed between current transaction and the first transaction in dataset.
3. Amount refers to transaction amount
4. Class is a label indicating whether transaction is fraudulent with value of 1 and non-fraudulent with 0 value.

#Exploratory Data Analysis 
Some initial exploratory data analysis included 
1. Checking null values- Dataset did not include any null values
2. Class Imbalance:- It was highly imbalanced with only 492 fraud transaction out of 284,907 transactions
3. Amount of Fraudulent transaction varied from 0 to 2125.87
4. Feature Correlation:- using heatmap no notable correlation observed between V1-V28. Certain correlation between Time and V3. Also between V7, V2O and Amount.

#Algorithm used
Random Forest Classifier with validation criteria of Gini (Gini Impurity and Log Loss) GINI = 2 * (AUC) - 1, where AUC is the Receiver Operating Characteristic - Area Under Curve (ROC-AUC. Number of estimators is set to 100 and number of parallel jobs is set to 4.
