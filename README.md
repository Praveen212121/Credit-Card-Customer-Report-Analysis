# Credit Card Transaction and Customer Report Analysis

## Objective
To develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends, enabling stakeholders to monitor and analyze credit card operations effectively.

## Dataset Description
Our data set consists of the following observations which include:

### Customer
- **Client_Num** - Unique identifier for each customer
- **Customer_Age** - Age of the customer
- **Gender** - Gender of the customer
- **Dependent_Count** - Number of dependents associated with the customer
- **Education_Level** - Education level of the customer
- **Marital_Status** - Marital status of the customer
- **state_cd** - State where the customer resides
- **Zipcode** - Postal code for the customer's location
- **Car_Owner** - Indicates whether the customer owns a car
- **House_Owner** - Indicates whether the customer owns a house
- **Personal_loan** - Indicates whether the customer has a personal loan
- **contact** - Contact method for reaching the customer
- **Customer_Job** - Job category of the customer
- **Income** - Annual income of the customer
- **Cust_Satisfaction_Score** - Satisfaction score provided by the customer

### Credit Card
- **Client_Num** - Unique identifier for each customer (linked to the customer dataset)
- **Card_Category** - Type of credit card the customer holds (e.g., Platinum, Gold, etc.)
- **Annual_Fees** - Annual fee for the credit card
- **Activation_30_Days** - Indicates if the customer activated the card within 30 days
- **Customer_Acq_Cost** - Acquisition cost for the customer
- **Week_Start_Date** - Start date for the data collection week
- **Week_Num** - Week number of the year for the data collection period
- **Qtr** - Quarter of the year during which the data was collected
- **current_year** - The year during which the data was collected
- **Credit_Limit** - Total credit limit of the customer’s card
- **Total_Revolving_Bal** - Total revolving balance on the customer's card
- **Total_Trans_Amt** - Total transaction amount made using the card
- **Total_Trans_Ct** - Total number of transactions made with the card
- **Avg_Utilization_Ratio** - Average utilization ratio of the credit card
- **Use Chip** - Whether the card has been used with a chip
- **Exp Type** - Type of the expiration (e.g., fraud, theft, etc.)
- **Interest_Earned** - Interest earned on the customer's card
- **Delinquent_Acc** - Whether the customer has any delinquent accounts

  ## Tools Used

- **Power Query**: Data extraction, cleaning, and transformation.
- **Python (Pandas, NumPy)**: Data processing and analysis.
- **SQL**: For querying and managing data in relational databases.
- **Power BI**: Data visualization and dashboard creation.
- **Excel**: For manual data inspection and supplementary analysis.

---

## Project Overview

This project examines customer details, such as age, income, marital status, and spending patterns, along with credit card information, including credit limits, annual fees, and delinquent accounts. Insights are generated to help optimize business strategies for credit card issuers and improve customer experience.

### Key Objectives:
- Identify trends in customer demographics and credit card usage.
- Analyze factors affecting credit limit and account delinquency.
- Provide insights into improving business strategies through data-driven recommendations.

---

## Data Cleaning & Preprocessing

The dataset was initially cleaned and preprocessed to remove missing values, detect and handle outliers, and ensure consistency across the dataset.

### Key Steps:
1. **Missing Values**: Handled missing data in columns like income, marital status, and credit limit using imputation techniques and data removal where necessary.
2. **Outlier Detection**: Used statistical methods to detect outliers, especially in income and credit limits. Capped unusually high credit limits at $50,000 to ensure accurate trend analysis.
3. **Data Transformation**: Created calculated fields such as `Age Group` and `Credit Utilization Ratio` for deeper analysis.

---

## Key Insights

### Customer Demographics:
- **Income vs. Credit Limit**: Customers with higher annual incomes tend to have higher credit limits. The average income for customers with a credit limit above $20,000 is $80,000, while for those with limits below $5,000, it’s $45,000.
- **Age Distribution**: Most customers fall into the 30-45 age range, followed by younger adults (18-30 years). Older adults (60+ years) are less likely to hold high credit limits.
  
### Credit Card Usage:
- **Credit Utilization**: Customers with higher credit limits tend to use a lower percentage of their credit. 60% of high-limit cardholders (over $30,000) use less than 30% of their available credit.
- **Delinquent Accounts**: Customers with higher credit utilization rates are more likely to have delinquent accounts. 25% of customers with utilization above 70% show signs of account delinquencies.

### Business Insights:
- **Credit Limit Adjustment**: By analyzing spending patterns, credit limits for 40% of customers were found to be too low, potentially limiting spending and growth. Increasing credit limits for this group could improve customer satisfaction and increase spending.
- **Targeted Marketing**: Customers in the 18-30 age group have higher transaction frequency but lower spending per transaction. Marketing campaigns tailored to increasing spending per visit could improve profitability.

---

## Analysis & Visualizations

### Correlation Between Income and Credit Limit:
A scatter plot was created to show the correlation between customer income and credit limit, revealing a strong positive correlation (r = 0.75). Higher income customers tend to receive higher credit limits.

### Age vs. Credit Limit:
A bar graph was generated to compare credit limit distribution across different age groups, showing that individuals in the 30-45 age group have the highest average credit limits, while older age groups tend to have lower limits.

### Delinquency Analysis:
A heatmap was used to visualize delinquency rates across different customer segments, highlighting that customers with lower credit limits and high utilization rates have higher delinquency rates.

---

## Dashboard

---
## Business Recommendations

1. **Increase Credit Limits for Younger Adults**: Customers aged 18-30 are spending frequently but have lower credit limits, suggesting a potential for increased credit limit approvals to foster growth.
2. **Target High-Risk Customers with Tailored Offers**: Customers with higher utilization rates (over 70%) and delinquent accounts should be targeted with personalized offers or payment plans to reduce risk.
3. **Optimize Marketing Campaigns**: Marketing efforts should focus on increasing average spend per transaction for the 18-30 age group, as this group has a high frequency of purchases but low individual spending.

---

## Future Improvements

- **Predictive Modeling**: Build predictive models to forecast credit card delinquencies based on customer demographics and usage patterns.
- **Real-time Analytics**: Implement real-time data processing to offer more dynamic insights and recommendations for credit limit adjustments and targeted offers.

		

