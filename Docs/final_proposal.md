# Draft Proposal for Prediction of risk in bond investment

## What is Bond Investment?
1)	Bonds can be issued by companies or governments and generally pay a stated interest rate.
2)	The market value of a bond changes over time as it becomes more or less attractive to potential buyers.
3)	Bonds that are higher quality (more likely to be paid on time) generally offer lower interest rates.
4)	Bonds that have shorter maturities (length until full repayment) tend to offer lower interest rates.


## Risks in bond investment: 
There are several types of risks in bond investment credit risk, interest rate risk, reinvestment risk, and liquidity risk. Investing involves risk and investors may incur a profit or loss.

## Why this project?
Risk prediction models are a valuable tool for identifying individuals and even organizations at risk for a variety of adverse outcomes. By identifying those at risk, interventions can be targeted to those most likely to benefit.

Risk analytics helps to manage risk-related issues by using technologies and techniques to deduce insights, calculate likely scenarios, and to predict future events. The goal is to minimize the impact of negative risks and capitalize on positive opportunities. 

## Research Questions 
+ How is the principal amount distributed among all organizations?
+ Does Issuer Group/Type have an impact on ADTR reportable status?
+ Which model is best for prediction?
+ Does the best model accuracy increase if hyperparamter tuning is performed? 

## Dataset
•	This dataset is intended for public access and use
•	This dataset contains 1508 rows, 66 columns
•	The data has all floating-type data

### Link to dataset: https://catalog.data.gov/dataset/kern-county

## Features
There are many features in this dataset, they are : CDIAC Number, Issuer, Issuance Documents, Sold Status, Sale Date, ADTR Report, ADTR Filing Status, ADTR Reportable, ADTR Reportable Next Fiscal Year, ADTR Last Reported Year, Debt Policy, Issuer County, MKR Authority, Local Obligation, MKR CDIAC Number, Issuer Group, Issuer Type, Project Name, Principal Amount, New Money, Refunding Amount, Net Issue Discount/Premium, Environmental/Social Impact Bonds, Debt Type, Purpose, Source of Repayment, TIC Interest Rate, NIC Interest Rate, Interest Type, Other Interest Type, Federally Taxable, First Optional Call Date, Final Maturity Date, CAB Flag, S and P Rating, Moody Rating, Fitch Rating, Other Rating, Guarantor Flag, Guarantor, Sale Type (Comp/Neg), Private Placement Flag, Underwriter, Lender, Purchaser, Placement Agent, Financial Advisor, Co-Financial Advisor, Bond Counsel, Co-Bond Counsel, Disclosure Counsel, Borrower Counsel, Trustee, Issue Costs Pct of Principal Amt, Total Issuance Costs, UW Takedown, UW Mngmt Fee, UW Expenses, UW Total Discount/Spread, Placement Agent Fee, Financial Advisor Fee, Bond Counsel Fee, Co-Bond Counsel Fee, Disclosure Counsel Fee, Borrower Counsel Fee, Trustee Fee, Credit Enhancement Fee, Rating Agency Fee, Other Issuance Expenses

I will be using only important columns as features, that will help me in my prediction. Target variable is "s and p rating."

I will filter out the imortant columns based on data analysis and exploring the data set thoroughly. 

As of now the important columns I can see in the dataset are(these may change based on analysis in the future)

1)CDIAC number - object - (The CDIAC Number is a unique sequential number that, along with the issuance year (the year in which the issuance was entered into the CDIAC database), identifies the issuance)
2)Issuer - Object - (issuer is a organization who is placing there bonds)
3)Sold Status - Object (it specifies that if the data is sold or not)
4)Sale Date - Object - (Date the bond is sold)
5)Credit Enhancement fee - float64 - (Credit Enhancement Fees means collective reference to payment or other Distributions made by Borrower to Guarantors)
6)s and p rating - object - (Standard & Poor's (S&P) is a leading index provider and data source of independent credit ratings)
7)ADTR report - object - (Annual Debt Transparency Report)
8)ADTR reportable - object - (whether iADTR is reportable or not)(yes/no)
9)CAB flag - object (capital appreciation bond)

I am planning on taking many other columns based on the analysis in the future. 

## ML Models 
I will try to check different regression models like linear regression, Adaboost regressor, decision tree regressor, ridge regression, and lasso regression. I will check the accuracy of each one and will try to perform hyperparameter tuning to improve the r2 score. I’ll compare everything and see what works best for this prediction.

## Expectations 
To find the best regression model for the prediction of risk in bond investment 

## Reference 
https://www.expressanalytics.com/blog/everything-you-need-to-know-about-risk-prediction-models/
