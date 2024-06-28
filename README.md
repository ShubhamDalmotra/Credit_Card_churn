# Credit_Card_churn

In this repository, I do machine learning modeling that can later be used to predict customer churn on credit card services.  The case in this dataset is a binary classification with an unbalanced proportion of target variables,  In this dataset there are several features that are used as parameters to make predictions, including:


CLIENTNUM: customer account number.
Attrition_Flag: customer status (Existing and Attrited).
Customer_Age: age of the customer.
Gender: gender of customer (M for male and F for female).
Dependent_count: number of dependents of customers.
Education_Level: customer education level (Uneducated, High School, Graduate, College, Post-Graduate, Doctorate, and Unknown).
Marital_Status: customer's marital status (Single, Married, Divorced, and Unknown).
Income_Category: customer income interval category (Less than $40K, $40K-$60k, $60K-$80K, $80K-$120K, $120K +, and Unknown).
Card_Category: type of card used (Blue, Silver, Gold, and Platinum).
Months_on_Book: period of being a customer (in months).
Total_Relationship_Count: the number of products used by customers in the bank.
Months_Inactive_12_mon: period of inactivity for the last 12 months.
Contacts_Count_12_mon: the number of interactions between the bank and the customer in the last 12 months.
Credit_Limit: credit card transaction nominal limit in one period.
Total_Revolving_Bal: total funds used in one period.
Avg_Open_To_Buy: the difference between the credit limit set for the cardholder's account and the current balance.
Total_Amt_Chng_Q4_Q1: increase in customer transaction nominal between quarter 4 and quarter 1.
Total_Trans_Amt: total nominal transaction in the last 12 months.
Total_Trans_Ct: the number of transactions in the last 12 months.
Total_Ct_Chng_Q4_Q1: the number of customer transactions increased between quarter 4 and quarter 1.
Avg_Utilization_Ratio: percentage of credit card usage.



We need to come up with a classification model that will help the bank improve its services so that customers do not renounce their credit cards


STEP 1
The first step, I will do Exploratory Data Analysis by using several functions and graphic visualization.  In this dataset there are features that have a very strong correlation, namely Credit_Limit and Average_Open_to_Buy.

STEP 2
The next step  was Data Preprocessing with reference to the findings that I got in the Exploratory Data Analysis stage, the steps I took were as follows:

Deleting the Credit Limit feature

Based on the results of the heatmap, there are two features that have a very strong correlation, namely the Credit_Limit and Average_Open_to_Buy features. Here I will delete one of the features from the two features and the feature I choose to remove is Credit_Limit. 

Data Scaling

Based on the results of the EDA, there are several features that have an abnormal data distribution. 

Categorical Encoding

 There are two techniques that I use, namely Label Encoding and One Hot Encoding. 
 
Split Data into Training and Testing sets

Here I divide the dataset into training data and testing data with a proportion of 70% for training data and 30% for testing data. 

Dataset Balancing


STEP 3
The last stage, I did the modeling using 3 algorithms, namely, Random Forest Classifier, and Gradient Boosting Classifier. The parameters that I use to see the performance of the model are the Accuracy, Precision, Recall, and Cross Entropy Loss scores. I use the Accuracy Score to see the model's ability to make predictions correctly for the entire data being tested. 


Try different classifier method and check which one give best results.

Result - here best model is gradient boost because in another Random Forest model train accuracy is 100% which is sign of over fitting
