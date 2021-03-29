# Loan Data from Prosper Exploration
## Introduction

In this project, I explore Loan Data from [Prosper](https://www.prosper.com/). Prosper is the first peer-to-peer lending marketplace in the United States and has facilitated more than $\$$18 billion in loans to more than 1,080,000 people.
This project is focused on visualising data and illustrating interesting discovery.

* <b>exploration_Loan_Data.ipynb</b></br> This is a report with my exploratory data analysis.
* <b>slide_deck_loan_data_analysis.slides.html</b></br> This is a slide desck presentation with my explanatory analysis.

## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found [here](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000) and the detail of the dataset's variables can be found [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


## Summary of Findings

In the exploration, I found that there was a strong negative correlation between APR and the Prosper ratings/credit score ratings as expected. A certain category of employment status affects the credit score range and 
Employment status doesn't always affect APR. However, employed people, in general, has lower APR compared to the other group of employment status. 
The loan amount also has a strong negative relationship with APR. The multivariate exploration here showed that there is indeed a negative effect of increased Prosper rating on APR, but interestingly the income range doesn't give a consistent effect on this relationship. Also, in the "employed" group, as income increases, the APR decreases in any loan amount group except income range of $\$$0. However, in different employment status, the income doesn't show consistent effects on APR.

## Key Insights for Presentation

For the presentation, I focus on the influence of the employment status, income range and original loan amount on APR.

I start by introducing each variable and its distribution, followed by the relationship between APR and other features.
Afterwards, I look at the APR by Employment status and Income range for the selected original loan amount.
To polish the plots, I included title, labels, legends and color bar where necessary. Also, I used heatmap to show the distribution of APR vs Original loan amount more clear.