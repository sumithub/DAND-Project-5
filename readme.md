# Lending Club Data Exploration
## Dataset
The data given below contains the information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
The source of the data is from https://www.kaggle.com/imsparsh/lending-club-loan-dataset-2007-2011. The feature documentation is also available in above link.

## Summary of findings

Firstly I looked at the summary statistics of loan amount to determine the range of loan amount. Since the target variable is loan_status, I looked at the proportion of loan_status and found 14% of the loans are charged off. <p>
    
I focussed my exploration around loan_status categorical variable. I looked at other categorical variables like Grade, Loan Term, Loan Years, Purpose etc to determine any correlation between the them. I found correlation between grade, term, purpose, intereset rates, installment amount and loan amount to be related with defaults. <p>

Plotting loan purpose against loan term shows that `debt consolidation` has the `highest rate of default` in both loan terms `36 and 60` months.There's an increase in trend of loan defaulters when we move from lower term to higher term. There's much highter default rate 25%+ for 60 months term against only 12% for 36 months period. Also, 60 months term has musch higher default rate almost double than 36 months which can also be considered to be very risky. <p>

Another significant relationship of interest was to see, how default rate varies with Loan amount and interest rates charged. It was found, `high loan amount` are charged `high interest rates`. As the interest rate goes higher, default rates goes up as well. For high loan amount and interest rate between 20-25 % have more than 40% default rates. <p>
  
Finally, it was interesting to see how installment amount and Annual income determine loan status. We've already seen low income group and high installment have high default rates, similar trend can also be seen  where `low income` group having `high installment` have highest rate of defaults. Highest default rate for low income is around 18% and the lowest default rate for high income is 12.5%.<p>
   
We've already seen higher grade tends to default. I was curious to see whether `high grades` and `deb_consolidation` have high defult rate also hold true. Found out, there's an increase in trend for higher order Grades namely E, F and G having `deb_consolidation` as main purpose who defaults the most.
 

## Key Insights for Presentation

- `debt consolidation` has the highest rate of default in both loan terms 36 and 60 months.
- `High loan amount` and `high interest rates` tends to have high default rate
- `low income` group having `high installment` are highest defaulters
- `Grades E, F, G` having high default rates have `debt_consolidation` as their main purpose to obtain loan


```python

```
