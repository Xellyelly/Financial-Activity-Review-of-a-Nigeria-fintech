# Financial-Activity-Review-of-a-Nigeria-fintech

## Overview:
> The management is interested in understanding user behavior and business performance across regions, products, and platforms between year 2023 to 2024 

**Objectives:** 
1. What’s the trend of transaction volume and value across time (monthly)?
2. What age group transacts the most and through what channels?
3. Are there any patterns in failed transactions (e.g., by platform, location, transaction type)?
4. Is there a peak period (month/day) for financial transactions?
5. Which transaction type is used the most?
6. What is the average transaction amount by transaction type?
7. Which platform/channel processes the most transactions in volume and value?
8. Which city has the highest volume of transactions?
9. What percentage of transactions were successful, failed, or pending?
Business Objective: Improve customer experience and detect unusual transaction behavior.

**Data source:**  From a Nigeria Fintech company with 10 columns and 7000 rows
**Key Features:**
 -	`Transaction ID`: Unique ID for each transaction
 -	`Customer ID`: Unique ID for each Customers
 -	`Customer Age`: Age of each customer
 -	`Gender`: Male and Female
-	`Location`: The city or region where the transaction took place, there are 8 different state   Abuja, Port Harcourt, Kano, Ibadan, Benin city, Lagos, Kaduna, Enugu.
 -	`Transaction type`: The nature of the transaction type, which are Deposit, Withdrawal, Transfer, Payment ,airtime and loan repayment
 -	`Channel`: The platform used for the transaction, which are web, agent, Mobile app, pos, ussd
 -	`Amount`: value of the transaction in naira 
-	`Transaction Date`: Date in which the transaction is being made
 -	`Status`: Status of the transaction either successful, failed or pending 
Tools – Excel(Data cleaning)  and Power bi (Dax,visualization)
## Data Cleaning
Checked for:
-	Missing values in Gender, Location, Status
-	Inconsistency in data entries
-	Duplicated transactions
-	Converted data to date format 
- Amount to numeric type 
- Display Amount in Nigeria currency (Naira)
Feature Engineering
- Created a new column, Age bin from customer age column 
## Key Performance Indicator (KPIs)
- Total no of customers (7,000)
- Total volume of transaction (7,000)
-	Total Amount of Transaction (₦71.01M)
  -Average Transaction amount (₦10.14K)


# Analysis:
## **Transaction across time** 
![Screenshot 2025-06-18 101213](https://github.com/user-attachments/assets/636a94c7-54e7-4d65-bb3f-266c4e1a5be7)

-	2023 Transaction volume peak occur in 3rd quarter with 933 transactions
-	2024 Transaction volume peak occur in the 1st quarter with 897 transactions, indicating reduction in growth rate 
-	Transaction volume is high and low in 1st and 4th quarter respectively for both years
-	Highest transaction volume in 2023 is July with 320 Transactions
-	Highest transaction volume in 2024 is January with 327 Transactions
-	Total yearly transaction value dropped from ₦35.92M (2023) to ₦35.10M (2024) indicating reduction in growth rate with about -1.08%
  ![image](https://github.com/user-attachments/assets/b1f5ad8e-d6ac-4f80-8b76-8b1d4c388c9b)

## **Trend of transaction across age group**
-	Age bin is created from customer age, grouped into 5 different groups 18-24, 25-34, 35-44, 45-54 and 55-64
  ![image](https://github.com/user-attachments/assets/774b95d6-d958-4627-bf43-1cc5bcc7abb0)
-	35-44 age group had the highest transaction value of about 15.9 million naira while 18-24 had the lowest of about 9.8 million naira
-	Customer within the age of 35-44 had highest number of transactions in kano (214), the location with the lowest is Lagos (175)
-	 Age group of 35-44 had highest amount of transactions in kaduna ₦2.36M indicating large fund transaction from people within this age in kaduna, the state with the lowest is port Harcourt ₦1.77M
-	Web channel is most used by age 35–44  
-	Airtime transaction type had the highest avg. transaction (₦11,680) for this age group

## **Transaction Status Overview:**
![image](https://github.com/user-attachments/assets/af0479d0-2164-41fc-bdf6-85a04702de0b)

 
-	There is 84.79% of successful transaction, 10.30% failed rate and 4.91% pending
-	There is 12.4% reduction in failed transaction status in 2024 compared to 2023
-	Airtime, Payment, Transfer had highest failure counts, loan payment has the lowest volume of failed transaction 
-	Payment method has  highest failed transaction amount, withdraw has the lowest failed transaction amount 
-	Benin city record the most failed transaction compared to other states 
-	Mobile app has the largest volume of failed transaction
-	Chanel type web record most pending transaction, Ibadan is the state with record most pending transaction compare to other state
-	Deposit transaction type has more record of pending status
-	
# **Transaction types:**
-	There is consistency across transaction showing stable transaction behavior over transaction type
  ![image](https://github.com/user-attachments/assets/8a8f01c1-c86c-44b7-9a24-a3a4da5d4ca2)

-	Payment method has most record but Transfer method has highest amount of transaction and highest average transaction of 10,485.17 
-	Abuja has highest number of transfer while Enugu has the lowest 

## **Channel Performance**
-	Transaction made through web channel has high transaction volume but the Agent Channel has highest Amount of transaction 
-	Failed transaction rate by Agent is more than web, web and ussd have the least failed rate compare to other Channel, probably explains why the most common age group prefer web over Agent
-	
## **Transaction across state**
-	There is little difference among location based on volume of transaction but there is significant difference in overall transaction amount from kano is higher than any other state of about almost 10million naira
  ![image](https://github.com/user-attachments/assets/8eddf8c7-ed12-4db3-b869-9885f7132f3d)

-	Withdrawal method is the most common transaction type in kano and the lowest is payment method

## **What Contributed to Growth Decline in 2024?**

![image](https://github.com/user-attachments/assets/e8c3c539-060f-4ca0-b37a-d4cc9a58ea8d)

-	Drop in transaction volume in Benin and Enugu
  ![image](https://github.com/user-attachments/assets/66e41839-5aab-486b-9bef-0070a51b4951) 
-	Drop in Lagos transaction volume in year 2024 probably due to low trust
-	Kano still maintain stable transaction volume in 2024
-	Payment transaction type decrease the most in 2024 followed by transfer and deposit, possibly due to failed or pending transaction
-	Airtime transactional type increase the most in 2024 followed by payment loan 
-	Age group 34-45 fell almost across all the location except port Harcourt where there is significant increase in 2024
  ![image](https://github.com/user-attachments/assets/e691dc58-36dc-400b-8384-8de8a902383a)

-	Pending transaction status increases by 9.76% in 2024

# Summary:
-	Total yearly transaction value dropped in 2024 by -1.08%, Transaction volume is high and low in 1st and 4th quarter respectively in 2023 and 2024
-	2023 reached peak in July and 2024 in January
-	35-44 age group had the highest transaction value , also in kano but but  kaduna had the highest amount , Kaduna Customers within this age group perform high amount of transaction, but there is reduction in the number transactions performed in kaduna in 2024, Web transaction is most common between this age group than Agent which record the highest amount , The preference of Web over Agent might result from high failed transaction by agent channel 
-	Transaction status success rate got better in 2024 compare to 2023, Failed transaction is also reduced in 2024 by 12.2% but pending status got bad in 2024 by 9.76% increase affecting deposit payment type, web Channel type and also Transactions at Ibadan are mostly affected compared to other location
-	Benin city is mostly affected by failed transaction status compare to other states, the channel method that filed the most in Benin is pos 
-	The channel with most failed transaction is mobile app then agent
-	Agent generate the highest amount of value compare to other channel type, it’s also the 2nd most common channel used and also 2nd most failed transaction
-	kano has highest amount of transaction compared to other state mostly use withdrawal transaction type even when payment and transfer is the most common transaction type

# Recommendation
-	Target campaigns and promotions around Q4 to improve transaction value when it's usually low across the year
-	Age Group 35–44 in Kaduna, has high transaction value  but reduced activity in 2024, Use personalized offers and loyalty programs to re-engage them and Promote Web channel usage where they’re most active and successful
-	Add real-time feedback to users on pending status to reduce drop-off
-	Conduct a POS infrastructure review in Benin and check other features that cause high failed transactions 
-	Prioritize mobile app updates that improve payment reliability and speed
-	Invest in support systems for agents to reduce failed transactions
-	Kano leads in total value but mostly uses withdrawals, Encourage use of Payments and Transfers through Discount, Utility payment integrations, Bonus offers for digital payment
-	Collaborate with local businesses or influencers to boost awareness and trust in city with low performance location like Lagos

## Skills used for this analysis
-	`Data Cleaning`
-	`Data Exploration (EDA)`
-	`Feature Engineering`
-	`Data Visualization`
-	`Statistical Thinking`
-	`Storytelling & Insight Communication`










