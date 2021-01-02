
apr rate 
https://www.prosper.com/loans/rates-and-fees/?refac=CANMB&refmc=6YRANV&refd=prosperblog


*********
Things to submit
1. A report with exploratory data analysis(pdf or html. use notebook)
2. A slide deck presentation with your explanatory analysis, in PDF or HTML format.
3. A readme document



https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0

-Status: LoanStatus
-Borrower's credit grade : ProsperRating (numeric), CreditScoreRangeLower
-Borrower's income/asset related data :EmploymentStatus, IsBorrowerHomeowner
-Borrower's financial related data : IncomeRange, StatedMonthlyIncome, DebtToIncomeRatio, CurrentDelinquencies, AmountDelinquent, PublicRecordsLast12Months, BankcardUtilization, 
-Loan condition : LoanOriginalAmount, BorrowerAPR
-Others :ListingCategory (numeric)


outlier when there are many number .

how i should check . should i narrow down to the one with defaulted.

c_loan_vars = ['LoanStatus', 'ListingCategory (numeric)']
c_fin_vars = ['ProsperRating (numeric)', 'EmploymentStatus', 'IsBorrowerHomeowner', 'IncomeRange']


Firstly, in terms of Listing Category, 9 (boat) has in general high credit score compared to the others, which is imaginable considering that boat is a laxual pourchase.
category 1(Debt Consolidation),3(Business) and 14(Large Purchases)have higher median and Q3 of loan amount compared to others. Also, 10(Cosmetic Procedure) and 13(Household Expenses) have slightly higher APR. And Q1 and Q4 of 8-20 are all surprisingly matching. 0-7 has spread wider than 8-20. Debt to income ratio has a lot of higher outliers. 9 

Secondly, in terms of Prosper rating, it shows interaction with credit score, but Prosper rating of 1-3 are not interacting compared to 4-7. Low Prosper ratings tend to have more higher outlier in debt to income ratio. Also, Prosper rating of 7 shows lower bank card utilization percentatge compared to others. And, Prosper rating shows positive relationship with original loan amount, although 5-7 doesn't show significant difference. On the other hand, it shows strong negative releationship with APR, as expected.


Thirdly, in terms of employment status, the median doesn't show significant difference but interestingly, self employed people and not employed people has slightly higher median compared to employed, and retired people. And, credit score of self-employed people and retired people has more spread. not employed people has high debt to income ratio, which is understandable. And, employed people has higher amount of original loan compared to the others. In terms of the loan amount, employed people has the highest 4Q, but the median is around the same with self-employed people. Not employed and retired people has low rate.　And  self-employed, employed and retired people has higher 4Q of bank card utilization, while median has no significant difference between employmetn status. Also, not employed people has slightly higher APR rate.