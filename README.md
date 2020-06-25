# Exploration of Loan Data from Prosper Funding LLC.

## Dataset
The Prosper Loan dataset consists of information on 113,937 loans from Prosper
Funding LLC (the first peer-to-peer lending marketplace in the United States).
This dataset holds 81 variables on each loan, including loan amount, borrower
rate (or interest rate), current loan status, borrower income range,
Prosper Score, and many others. Since the Prosper Score is applicable for loans
that originated after July 2009, I will be using only the data from July 2009.
The dataset can be found here
https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv,
with feature documentation available here,
https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0.


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
status of the loan and the year the loan was made. There is a greater proportion
of "In Trouble" loans between 2006 and 2008, which makes sense since it coincides
with the subprime mortgage crisis around that time. I also found that more than
half of the loans were taken for out for Debt Consolidation and almost a half
of those loans were "Troubled" loans. The data also suggests that there are
proportionally more "In Trouble" loans in the lower income ranges as well as in
those loans where the borrower is unemployed. I also found that the
borrower's mean monthly income is lower by almost $800 for "In Trouble" loans
than those that are Active or Completed.

I also saw a relationship between the borrower rate and the borrower's
Employment Status, the Prosper Scores, whether the borrower is
a homeowner, and whether the borrower's income is verifiable.

## Key Insights for Presentation

For the presentation, I focus on just the influence of different borrower
attributes on the borrower rate. I start by introducing the borrower rate
variable, followed by the pattern in Prosper scores and then plot the
regression plot for average borrower rate vs Prosper scores.

Afterwards, I introduce each of the categorical variables one by one. To start,
I use the violin plots of borrower rate and Prosper Score vs employment status.
The other two variables of Income Verifiability and Homeownership Status are
covered later on using regression models. I've made sure to use different color
palettes for each quality variable to make sure it is clear that they're
different between plots.

## References
https://stackoverflow.com
https://matplotlib.org
https://seaborn.pydata.org
https://www.prosper.com
https://www.markdownguide.org/cheat-sheet/
