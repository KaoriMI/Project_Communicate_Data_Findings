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