# Machine-Learning-using-Decision-Trees-Random-Forest-Lending-Club-Dataset

This project explores the dataset from LendingClub.com. Lending Club is a service that connects borrowers with people who have money 
(investors).We will try to create a model that will help predict if a person has a high probability of paying the loan back.


# Data
The dataset contains lending data from 2007-2010.Our objective is to classify and predict if the borrower paid back their loan.

The data set contains the following features:

credit.policy: 1 if customer meets the credit underwriting criteria of LendingClub.com, and 0 otherwise.                       
purpose: Purpose of the loan (takes values "credit_card", "debt_consolidation", "educational", "major_purchase", "small_business", and "all_other").                       
int.rate: Interest rate of the loan,(a rate of 11% is stored as 0.11). Borrowers judged by LendingClub.com to be more risky are assigned higher interest rates.                 
installment: Monthly installments owed by the borrower if the loan is funded.               
log.annual.inc: The natural log of the self-reported annual income of the borrower.              
dti: Debt-to-income ratio of the borrower (amount of debt divided by annual income).                      
fico: FICO credit score of the borrower.
days.with.cr.line: Number of days borrower has had a credit line.                       
revol.bal: Borrower's revolving balance (amount unpaid at the end of the credit card billing cycle                     
revol.util: Borrower's revolving line utilization rate (the amount of the credit line used relative to total credit available).       
inq.last.6mths: Borrower's number of inquiries by creditors in the last 6 months.              
delinq.2yrs: Number of times borrower had been 30+ days past due on a payment in the past 2 years.            
pub.rec: Borrower's number of derogatory public records (bankruptcy filings, tax liens, or judgments).           


![image](https://user-images.githubusercontent.com/35156789/41815609-75553894-773e-11e8-914b-f0b55fa16757.png)

![image](https://user-images.githubusercontent.com/35156789/41815654-9c1653ea-773f-11e8-84c4-fe4b02871833.png)

![image](https://user-images.githubusercontent.com/35156789/41815660-bb89f0e2-773f-11e8-9d5c-16a878e46a36.png)

![image](https://user-images.githubusercontent.com/35156789/41815663-cf8c1048-773f-11e8-98f4-1be00b4c8e71.png)


# Exploratory Data Analysis
Identifying the relationship between different variables in the dataset.

# Dual histogram of the FICO score of the borrowers,depending on the credit policy (i.e. if a borrower met the underlying criteria).

![image](https://user-images.githubusercontent.com/35156789/41815671-0c62511c-7740-11e8-9ed0-76fa377840ae.png)

![image](https://user-images.githubusercontent.com/35156789/41815674-1efb4338-7740-11e8-829c-c937480ffa7f.png)

# Dual Histogram of the FICO score of the borrowers based on the 'not.fully.paid' column.
![image](https://user-images.githubusercontent.com/35156789/41815678-35b69e06-7740-11e8-8735-24fb3ba2f52f.png)

# Visualization representing if a borrower fully paid the loan back

![image](https://user-images.githubusercontent.com/35156789/41815693-94d71776-7740-11e8-8cc6-bc1729bb68a8.png)

# Trend between FICO score and interest rate.
![image](https://user-images.githubusercontent.com/35156789/41815703-c229c73c-7740-11e8-8202-46175cb591f6.png)

# Model Building
The purpose column is categorical.We transform  using dummy variables so sklearn will be able to understand them.

![image](https://user-images.githubusercontent.com/35156789/41815907-d9aecf60-7745-11e8-928e-4a2c0e89d7c4.png)

# Train Test Split

![image](https://user-images.githubusercontent.com/35156789/41815914-09734a14-7746-11e8-9681-3eaab4838916.png)

# Training a Decision Tree Model

![image](https://user-images.githubusercontent.com/35156789/41815924-2e5fdcde-7746-11e8-96c9-64acf06f39c6.png)

# Predictions and Evaluation of Decision Tree

![image](https://user-images.githubusercontent.com/35156789/41815984-92c6423e-7747-11e8-9f61-661406278be5.png)

![image](https://user-images.githubusercontent.com/35156789/41816015-4ae4c07a-7748-11e8-909a-61858ba88a21.png)

# Training the Random Forest model

![image](https://user-images.githubusercontent.com/35156789/41816107-1e44f448-774a-11e8-93ef-683345cdf322.png)

![image](https://user-images.githubusercontent.com/35156789/41816018-672a185c-7748-11e8-95ba-6ceeebad1a8b.png)

# Predictions and Evaluation of Random Forest

![image](https://user-images.githubusercontent.com/35156789/41816022-86a93d02-7748-11e8-8530-3f4d06ae0319.png)


