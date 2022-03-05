# Table Of Contents
1. About Dataset
2. Objective of this project
3. Exploratory Data Analysis(EDA)
   3a. Data Visualization
   









## About Dataset
* This is a Telco-Customer-Churn dataset, I took this csv file from kaggle. Each row represents a customer, each column contains customer’s attributes described on the column Metadata.

* The data set includes information about:

    * Customers who left within the last month – the column is called Churn

    * Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies

    * Customer account information – how long they’ve been a customer(tenure), contract, payment method, paperless billing, monthly charges, and total charges

    * Demographic info about customers – gender, age range, and if they have partners and dependents. Dataset contains 7043 rows and 21 columns.

## Objective of this project

* **My goal is to predict the number of customers leaving the phone service**. We need to understand better the situation, which customers are likely to leave and why. Once it is clear what features are impacting customer churn, then we can start create Machine Learning Models.

## Exploratory Data Analysis(EDA)
### Data Visualization
![i1.png](i1.png) ![i2.png](i2.png)  ![i3.png](i3.png) ![i4.png](i4.png)  

### Preprocessing
   * There are no null values in this dataset.
   * Encoded 18 categorical columns
   * Standardized 3 columns(tenure, MonthlyCharges, TotalCharges)
   * Checked for outliers

### It is an imbalanced Dataset
![imbalance.png](imbalance.png)

![smote.png](smote.png)

### Discussions from Correlation Heat Map
* The correlation goes from + 1 to - 1 where 1 is total positive linear correlation 0 is no linear correlation and negative 1 is total negative linear correlation.

* From color bar,

   * Yellows are negative correlations,

   * Darker the yellow, stronger negative correlation

   * Middle section where the colors are real light blue where there's not much correlation at all

   * the Dark blues are positive correlation and

   * the darker the blue the stronger positive correlation

   * Churn is highly correlated(positive correlation)with tenure,InternetService_Fiber optic, Contract_Month-to-month, Contract_Two year, PaymentMethod_Electronic check.

   * Churn is strongly correlated with itself.
