# Prosper loan dataset exploration
## Omolayo Ipinsanmi


## Dataset

The loan dataset by prosper contains 81 variables with 113,937 entries. the variables includes  loan amount, borrower rate or interest rate, BorrowerRate, LenderYield, EstimatedEffectiveYield, EstimatedLoss, EstimatedReturn and many others.
This [link](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0) to the data dictionary contains more details about the dataset.


## Summary of Findings

Before the exploration, I removed rows in the data where the feauture of interest (Borrower APR) was missing. In the exploration, I found out that majority of the borrowers are from CA(California) followed by TX(Texas) and then NY(New York). This expected as Claifornia is the most populous state in the US followed by Texas, Florida and then New Your according to [this](https://www.infoplease.com/us/states/state-population-by-rank) report. California also houses the Silicon valley which is a base for many tech startups. After removing general categories like 'others' and 'professional' from occupation, I found out that computer programmers obtained loans the most followed by Executives and then Teachers. Computer programmers might have obtained more loans due to the fact that they run more startups than many other categories especially in the tech category. This futher corroborates the observation on California having the largest population im out dataset for more loan application.

Borrowers APR was seen to generally lie between 0.1 an 0.4 with two distcint peak occuring at 2.0 corresponding to 20% and 3.6 corresponding to 36% APR. Also the distribution of borrowers APR was seen to be similar to that of Borrowers interest rate (Borrower rate). This makes sense as APR comprises of rate and other fees therfore the more the rate, the more the APR. I then went ahead to remove entries where stated monthly income was higher than 35,000 dollars as this was looking like outliers. A strong positive relationship was seen between Borrowers rate and borrowers APR, this confirms the similarity in distribution noticed ealier. I also found a negative correlation between the loan original amount and Average borrower APR Meaning the APR tends to decrease as the loan amount increases. This makes sense as a low APR will encourage people to take more loans and discourage them from taken small amounts. The prosper rating shows a negative relationship with borrowers APR with low rated borrowers having high APR.

Outside of the main variables of interest, I observed a high correlation between laon amount and monthly income. This is plausible becuase individuals who make more money can afford more loan. There is also a very strong relationship between loan amount and monthly payment, a relationship which is totally expected because the higher the loan amount, the more the borrower is expected to pay back over the time period. A positive relationship was also observed between loan term and monthly payment meaning people who take long term loan pay slightly higher amount back monthly. This could be related to the loan amount taken as this has been seen to correlate positively with term.


## Key Insights for Presentation

For the presentation, I looked into factors that affects the borrowers APR. I looked at loan term vs borrower APR, Loan Original Amount, Borrower APR and Loan Term, Loan Original Amount and Borrower APR, and also Borrower APR, Prosper Rating and Employment Status. This factors were seen to correlate with APR and can guide both lenders and borrowers choice on loan operation.
