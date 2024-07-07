# LP2-belize
A supervised machine learning project to predict customer churn

# **Predicting Customer Churn** 

 ## Introduction

Customer attrition is one of the biggest expenditures of any organization. Customer churn otherwise known as customer attrition or customer turnover is the percentage of customers that stopped using your company's product or service within a specified timeframe.
For instance, if you began the year with 500 customers but later ended with 480 customers, the percentage of customers that left would be 4%. If we could figure out why a customer leaves and when they leave with reasonable accuracy, it would immensely help the organization to strategize their retention initiatives manifold.

In this project, we aim to find the likelihood of a customer leaving the organization, the key indicators of churn as well as the retention strategies that can be implemented to avert this problem.



## Business Understanding

 ### *Explanation of Features* 

 Data Dictionary
   - Customer ID; nique customer code
   - Gender; sex of the customer
   - Senior Citizen; age of the customer
   - Partner; marital status of the customer
   - Dependants; if the customer has dependants 
   - Tenure; number of years as a customer
   - Phone Service 
   - Multiple Lines
   - Internet Service
   - Online Security
   - Online Backup 
   - Device Protection
   - Tech Support
   - Streaming TV
   - Streaming Movies
   - Contract
   - Paperless Billing
   - Payment Method
   - Monthly Charges
   - Total Charges
   - Churn


  ### *Hypothesis - Contract period*

 **Null Hypothesis** - The contract type has no significant on the level of attrition

 **Alternate Hypothesis** - The contract type has significant impact on the level of attrition

 ###  *Analytical Questions*
1. What are the key factors affecting customer churn?
2. How does customer tenure affect the likelihood of churn?
3. Which demographic factors influence customer churn?
4. Does the contract period affect customer churn?
5. Does the type of Internet Service affect customer churn?


 ## Data Understanding

### Importation

### Load Datasets

### Exploratory Data Analysis (EDA)

##### Explore the data

Online Security, Online Backup, Device Protection, Tech Support, Streaming TV and Streaming Movies columns have 21.7% missing values followed by Total Charges column with 0.17% missing values and finally Churn columns with 0.03% missing values

##### Summary Statistics

- The average tenure is 32.5 months with a range of 0 - 72 months which shows there are new customers and loyal customers in the data
- The average monthly charge is 65.34 with a range of 18.40 - 118.65
- The average total charge is 2,301.28 with a range of 18.80 - 8,564.75

- The male customers are more than female customers with a frequency of 137
- Most customers do not use multiple lines
- The most common internet service is Fibre Optic
- The most common contract is month-to-month
- The most popular payment method is Electronic check

##### Inspecting Columns

##### Concatenate the datasets

##### Dropping Columns

I am going to drop the Total Charges column. I am making the assumption that the total charges column is a multiplication of the tenure and monthly charges colums.
That does however not reflect in the column hence why I am dropping it. I am also making the assumption that the tenure is in months and 0 means the client has been subscribed
for less than a month
The goal of dropping this row is also to get the correct datatype, it should be float not object

##### Univariate Analysis

##### Bivariate Analysis

##### Multivariate Analysis

### Answering Analysis Questions

### Hypothesis Testing
Reject the null hypothesis. The contract type has no significant impact on the level of attrition.

### Conclusion

Based on the analysis and the Chi-Square Test for Independence, we reject the null hypothesis, indicating a significant relationship between customer attrition and the type of contract. The count plot illustrates a higher number of customers leaving the company, particularly among those with a Month-to-Month contract. This suggests that contract terms play a crucial role in customer retention. To enhance customer retention strategies, the marketing department should consider tailoring promotional efforts or loyalty programs to address the needs and preferences associated with different contract types. Specifically, for those with a Month-to-Month contract, they should put more effort into convincing them to consider other contract types, such as one year or two years. Additionally, targeted communication and incentives could be designed to encourage long-term commitment, thereby reducing the likelihood of churn within specific contract segments.




