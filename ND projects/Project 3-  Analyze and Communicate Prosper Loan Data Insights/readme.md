# Prosper Loan Data Exploration

# Dataset 
the datast contains 81 variables for 113937 loans including information about the borrower and the lender. The dataset can be found from here:
https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1605993250865000&usg=AOvVaw0XhSWEQqDx03LMX6H2UCu3
The data dictionary is provided here: https://docs.google.com/spreadsheets/u/0/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit?usp=sharing

# Summary of findings
In the exploration, I start with the univariate analysis of the 12 variables. 
I found that only 5 loans of all loans are cancelled and 50 % of loans are currently ongoing. Sum of all Past due loans make up only 1.8% of data.
 Most loans (77%) are 36 month in duration and least loans (1.42%) are 60 month in duration.
 Payments are mostly multiples of 5000. Largest portion of loans are paying less than 500 amonth and only less than 10 are paying more than 2000 amonth.

I then do bivariate analysis, I find a strong linear relationship between borrower apr and borrower rate.
An interesting pattern where The higher the monthly income,on average, the less due days past the deadline of payment.
 People with highest monthly income ,on average, are the ones who are doing their final loan payment.
Numbers of home owners and non home owners are very similar across different loan statuses, so it doesn't contribute to loan status as much.
Loans with longest duration (60 month) have lowest monthly payments, whereas shortest duration loans have highest monthly payments.

# key insights for presentations
In the presentation, At first, I focused on anwering how each variable affects Loan Status. 
Monthly income affects Loan status, where Completed, Current and FinalPayment Loans have relatively higher mean income and Defaulted, Chargedoff and Past Due date loans have lower incomes.
An interesting Finding I observed where The higher the monthly income,on average, the less due days past the deadline of payment.Interestingly, Defaulted and Chargedoff loans having similar mean loan original amount to completed loans which might be explained by having lower monthly income, thus more likely to not being consistent in completing the loan.Numbers of home owners and non home owners are very similar across different loan statuses, so it doesn't contribute to loan status as much.

Second, I assess some variables and their effect on Borrower APR and Monthly Payments.
I find a strong linear relationship between borrower apr and borrower rate.A Ratio above 1 show slighlt increasing trend of Borrower APR, which can be reflected as increase of risk (Higher APR) as Debt to to income ratio increases.
An exception to that is the ratio of 10, where it means worst case of debt but still having wide range of BorrowerAPR.A decreasing trend starting above 200 investors shows that as number of investors increase, borrower APR generally tend to decrease which could be interpreted as safer lower risk loan.
Up to 4 recommendations, APR seems to have wide range of values and for more than 4 recommendations, borrower APR decreases gradually to less than 0.1 when exceeding 14 recommendations except for one observation.
A general decreasing trend is observed of Borrower APR as Monthly income increases.Employed, full-time, retired distributions, part-time are right skewed where BorrowerAPR tends to be of a lower value.
Not employed shows clear left skew and APR tends to be higher, other and self-employed are less ditinguishable as they contain bimodal.Loans with longest duration (60 month) have lowest monthly payments (smallest slope), whereas shortest duration loans have highest monthly payments (largest slope), and payments in between those values tend to be for moderate loan durations.
Monthly Loan payment is found to be affected by employment status where employment tends to associate higher monthly payment and bing part-time or retired or not employed tends to associated less monthly payment.

