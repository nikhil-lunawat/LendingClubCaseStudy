# Lending Club Case Study
> Lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders.

> Objective is to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss.

> Perform EDA analysis to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. This knowledge can be utilised for its portfolio and risk assessment.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- Import required libs and load data set
- Data cleanup, manipulation and conversion to correct data types
- Data filtering and create derived columns
- Univariate Analysis
- Segmented Univariate Analysis
- Bivariate and multi-variate analysis

## Technologies Used
Project is executed on Ubuntu 22.04

- Jupiter notebook
- Python 3.10.x

#### Libraries used and their versions
Please install below libs before executing notebook

- matplotlib 3.9.x
- seaborn 0.13.x
- scipy 1.14.x

## Conclusions
The above analysis for loan data on multiple variables gives below data points.

### Univariate analysis
There is **more number** of defaulting loan when:

1.  Grade is "B"
2.  Loan status is "Not verified"
3.  Purpose of taking loan is "Debt consolidation"
4.  term is "36 months"
5.  Home ownership is "Rent"
6.  Loan amount is between 5000 to 10000
7.  Interest rate is between 10% to 15%
8.  Annual income is between 38k to 55k
9.  Number of open accounts is between 5 to 10
10. Number of inquiries in last 6 months is 0
11. Loan if issues in "December"
12. Applicant's state is "CA"

This analysis gives categories where maximum defaulters are present (does not mean necessarily that probability is high or low).

### Segmented analysis
There is a **high probability** of defaulting loan when:

1.  Loan status is "verified"
2.  Grade is "G". As grade decreases, defaulting probability increases.
3.  Term is "60 months". More number of months to repay increases defaulting probability.
4.  Purpose is "Small business". Risky purpose increases probability.
5.  Interest rate category is between 20-25%. If interest rate increases, defaulting chances also increases.
6.  Loan amount is between 28000 to 35000, highest probability of not paying loan. Higher the loan amount more probability of loan defaulting application.

This analysis gives category wise probability which could result in defaulting cases.

### Correlation analysis

Positive correlation for charged off loans
1. cluster of loan amount, installment and annual inc
2. term and interest rate

### Bivariate or multi-variate analysis
There is a **high credit loss risk** of defaulting loan when:

1.  interest rate higher by 2% across all loan amount categories leads to more defaults
2.  purpose as "small business" requiring loan amount of 14k+. Risky purpose with higher loan amount
3.  home ownership as "mortgage" requiring loan amount of 13k+
4.  annual income between 106k to 123k and loan amount of 18k+
5.  grade is "G" and interest rate is above 20%
    1. As grade goes from "A" to "G" Possibility of defaulter increases too and graph shows that interest rate also goes up.
7.  Grade is either F and loan amount is between 17.5k-20k
8.  interest rate is between 20-25% and loan amount between 14000 to 21000
9.  interest rate is between 20-25% and annual income between 21000 to 38000. More interest rate but lesser annual income result in defaulting loan.

This analysis gives special cases which could result in defaulting loan applications

## Acknowledgements
Project is done by

- Nikhil Ugale
- Nikhil Lunawat (Group Facilitator)

## Contact
Created by [@nikhil-lunawat] - feel free to contact me!
