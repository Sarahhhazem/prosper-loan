# Prosper Loan Data Exploration
## by Sarah Hazem 


## Dataset

> The Prosper Loan Dataset consists of 113,937 loans with 81 variables for each loan. These variables include Loan Original Amount, Borrower APR, Income Range, Employment Status, Prosper Rating and more. I wanted to look at the characteristics of borrowers that could be used to predict their borrower APR and the probability of a borrower defaulting on a loan. To do that, I added an extra "defaulted" binary feature where 1 indicates a customer has defaulted and 0 otherwise. 
Data feature documentation is available here: https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit


## Summary of Findings
In the exploration, I found that there was an approximately linear relationship between Borrower APR and Loan Original Amount. Surprisingly, when I isolated customers who defaulted, the negative relationship between Borrower APR and Loan Original Amount turned gradually into a positive relationship across all prosper ratings. Moreover, As the prosper rating gets higher, the correlation between borrower APR and loan original amount gets reversed gradually from a negative correlation to a positive correlation, which is interesting but can be explained by the fact that well-off people get charged higher rates as the loan value increases. Furthermore, customers who didn't default had on average higher loan amounts and lower APRs than those who defaulted.

Outside the main variables of interest, I found out that as the income range increases, the loan amount increases and the borrower APR reaches much lower levels. However, interestingly, there seems to be no relationship between prosper ratings and employment statuses, as for each employment status the ratings seem to be equally divided. Lastly, for both customers who defaulted and those who didn't default, the negative relationship between borrower APR and prosper rating remained the same.


## Key Insights for Presentation

For the presentation,  I wanted to focus at the characteristics of borrowers that could be used to predict their borrower APR and the probability of a borrower defaulting on a loan. The main focus was on the following characteristics: Prosper Rating, Loan Original Amount and Income Range.

I start by introducing the first variable of interest Borrower APR variable, followed by the the distribution of the loan original amount, then plot the relationship between the two using a scatterplot with a regression fitted line. After that, I plot Borrower APR against our two categorical variables: prosper rating using a violin plot and Income Range using a bar chart. 

Next, I introduce the second variable of interest by plotting a pie chart showing the percentage of customers who defaulted vs. those who didn't. I then plot the percentage of defaulting customers by borrower APR and loan original amount to clearly see how these three variables interact. Next, I plot the defaulting variable against our two categorical variables prosper rating and income range using stacked bar charts. Next, I emphasize the negative relationship between borrower APR and prosper rating by adding in the defaulting variable and plotting a dodged point plot. Lastly, I present the most interesting conclusion by plotting borrower APR and loan original amount by prosper rating for customers who fefaulted using a scatterplot and a sequential palette for prosper rating. 
