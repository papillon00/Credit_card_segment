## Analyze Credit Card Customer Segmentation 

### Goal 
To see which customer segment the credit card provider should focus on for retention efforts <BR>
* the attributes I want to focus on are as follows: 
1. Credit limit value and relative utilization value - Monetary value they can spend (higher the better)
2. Month of inactive_12_mon - Recency (lower the better)
3. Frequency of transactions - Consistency of spending habits (Highter the better)


To analyze what kind of customers are more likely to discontinue w/ the card<BR>
* Attributes I want to explore:
1. Income level : explore if there's a relationship between income level and churn rate
2. Credit limit amount: explore if there's a relationship between low credit limit and churn rate
3. month of inactive_12_mon: assumes higher number indicate higher possibility of churning
4. Total_Relationship_Count: explore if >= 1 indicate less churn rate

### Dataset
Dataset downloaded from [Kaggle](https://www.kaggle.com/datasets/thedevastator/predicting-credit-card-customer-attrition-with-m/data)

I kept the below columns:

* CLIENTNUM: Unique identifier for each customer. (Integer)
* Attrition_Flag: Flag indicating whether or not the customer has churned out. (Boolean)
* Customer_Age: Age of customer. (Integer)
* Gender: Gender of customer. (String)
* Dependent_count: Number of dependents that customer has. (Integer)
* Education_Level: Education level of customer. (String)
* Marital_Status: Marital status of customer. (String)
* Income_Category: Income category of customer. (String)
* Months_on_book: How long customer has been on the books. (Integer) ->number of months that have passed since the customer's account was opened
* Total_Relationship_Count: Total number of relationships customer has with the credit card provider. (Integer)
* Months_Inactive_12_mon: Number of months customer has been inactive in the last twelve months. (Integer)
* Contacts_Count_12_mon: Number of contacts customer has had in the last twelve months. (Integer)
* Credit_Limit: Credit limit of customer. (Integer)
* Total_Revolving_Bal: Total revolving balance of customer. (Integer)
* Avg_Open_To_Buy: Average open to buy ratio of customer. (Integer) -> average amount of unused credit a customer has compared to their credit limit.
* Total_Amt_Chng_Q4_Q1: Total amount changed from quarter 4 to quarter 1. (Integer)
* Total_Trans_Amt: Total transaction amount. (Integer)
* Total_Trans_Ct: Total transaction count. (Integer)
* Total_Ct_Chng_Q4_Q1: Total count changed from quarter 4 to quarter 1. (Integer)
* Avg_Utilization_Ratio: Average utilization ratio of customer. (Integer) -> amount of credit to total available credit limit cx use on average

### Clustering Techniques to Use

**1. RFM Anlaysis**
    
A marketing technique used to quantitatively rank and group customers based on their transaction history to identify the best customers and tailor marketing strategies accordingly. RFM stands for Recency, Frequency, and Monetary value, each corresponding to a key customer trait.

**2. K-Means Clustering:**

This is a popular unsupervised learning technique that groups data points into a predefined number of clusters based on their similarity. 
