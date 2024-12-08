# Credit Card Transaction and Customer Report Dashboard
![card](https://github.com/user-attachments/assets/a1b986b0-f4f4-44e3-a665-6568c4b8d0bb)


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

# Credit Card Customer Analysis Project

## Tools Used
- Power Query
- SQL
- Python (Pandas, NumPy)
- Power BI
- Excel

## Project Description
This project involves analyzing a dataset containing customer and credit card information, such as customer demographics, credit card details, payment history, and spending behavior. The goal is to uncover trends and generate insights that can be used to optimize customer management and marketing strategies.

## Data Cleaning & Transformation
### Steps for Data Import:
1. Import datasets using Power Query.
2. Perform necessary transformations, including dealing with missing values, duplicate records, and outliers.
3. Merge the customer and credit card data for comprehensive analysis.

### Key Calculated Fields:
- **Age Group**:
    - Categorize customers into age groups (e.g., Children, Young Adults, Adults, Seniors).
- **Credit Limit Category**:
    - Classify customers based on their credit limits (Low, Medium, High).

## Data Analysis

Customer Segmentation:

The dataset provided customer demographics, such as Client_Num, Customer_Age, Gender, Income, and Marital_Status. Analysis showed diverse age groups, with a mix of young adults, middle-aged adults, and seniors across different Income levels.
Income was a key factor in understanding customer behaviors, with higher income levels corresponding to higher credit limits and card categories.

Credit Card Utilization:

The analysis revealed how Credit_Limit and Credit_Balance interact, with some customers utilizing a significant percentage of their available credit. High Credit_Balance relative to Credit_Limit was a key indicator of higher credit risk.
The dataset contained a significant number of Delinquent_Acc, indicating missed payments. A correlation was observed between low-income customers and high credit card balances, leading to missed payments.

Delinquency Patterns:

The analysis showed that a percentage of accounts have missed payments, with lower-income customers experiencing higher delinquency rates.
Delinquent_Acc was used to track and identify customers at risk, and these insights can inform strategies to target specific high-risk customer segments for repayment assistance.
Card Category Insights:

A comparison between the different Card_Category values (e.g., Blue, Gold, Platinum) revealed a clear distinction in income levels and spending behaviors across customers. Premium card categories (e.g., Platinum) had higher annual fees but also attracted higher-income customers with larger credit limits.

Income vs Credit Behavior:

Income and Credit_Limit had a strong relationship, with higher-income individuals receiving higher credit limits. This directly influenced their Credit_Balance, as they were able to carry larger balances without the risk of reaching their limit.

Spending Insights:

Customers with higher incomes generally had higher Credit_Limit but also tended to maintain a higher Credit_Balance. This reflects a trend where customers with more disposable income are likely to spend more, though they may also be at risk of accumulating debt.


## Business Insights:
- **Targeted Marketing**:
    - Customers with premium cards should be targeted for new offers with higher credit limits.
    - Customers with late payment history might benefit from reminders or financial counseling services.
- **Customer Retention**:
    - Focus on customers with lower credit limits who have shown consistent payment behavior, as they may have potential for higher card limits.

## Dashboard
![Credit Card Financial Dashboard-Customer](https://github.com/user-attachments/assets/19a359fd-5d9b-49fa-9613-9a7a0cacb7c1)
![Credit Card Financial Dashboard-Transaction](https://github.com/user-attachments/assets/ce072551-474c-4f94-a397-1264370c35fd)


## Key Metrics & Findings:
Customer Demographics:

The dataset includes customer information such as Client_Num, Customer_Age, Gender, Income, and Marital_Status.
Key demographic insights reveal a diverse customer base across various Income levels and Age groups, enabling targeted segmentation for more personalized offers.

Credit Card Data:

Card_Category: Different categories (such as Blue, Silver, Gold, Platinum) represent varying levels of services and benefits for customers.
Credit_Limit: The dataset contains significant variation in credit limits, with higher limits associated with customers in higher-income brackets.
Annual_Fees: Insights suggest that the Annual_Fees are closely tied to Card_Category, with premium categories charging higher fees.
Delinquent Accounts:

A percentage of accounts have missed payments, and this is correlated with low-income customers and high credit card balances.
Delinquent accounts are identified by Delinquent_Acc and indicate a need for targeted credit management solutions.

Credit Utilization:

The dataset reflects the balance between Credit_Limit and Credit_Balance, with some customers utilizing a significant percentage of their credit, leading to a higher risk of delinquency.
Income and Spending:

Income is a major determinant of credit behavior, with lower-income customers typically carrying higher Credit_Balance to Credit_Limit ratios.
This highlights potential areas for targeted credit limit adjustments to better manage risk.

## Conclusion
This project provides valuable insights into customer spending behaviors, credit usage, and payment habits. By segmenting customers based on income, age, and payment behavior, businesses can create more targeted marketing and retention strategies to enhance customer engagement and profitability.
		

