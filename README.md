![](https://hbr.org/resources/images/article_assets/2020/11/Nov20_06_1215016292.jpg)
# Credit Risk Classification

The purpose of this analysis is to find the risk factors of a peer-to-peer lending company by dividing the loans into two classes: low_risk and high_risk.
the feature that have been used for this analysis are loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks and otal_debt.
The label  has the following ratio of low_risk to high-risk loan status in the original dataset:75036/2500. that is not balanced.
The first part of the analysis is focused on creating a Logistic regression model and fitting it on the original dataset. In the second part, the data is resampled to balance the two classes by oversampling the minority class and redoing the logistic regression modeling again. 

## Machine learning models evaluation

* Logistic model trained on the original dataset:
  * balance accuracy score: 94%
  * Accuracy: 99%
  * precision of low-risk class: 100%
  * precision of high-risk class: 87%
  * recall of low_risk class: 100%
  * recall of high-risk class: 89%
 
* Logistic model trained on the balanced dataset:
  * balance accuracy score: 100%
  * Accuracy: 100%
  * precision of low-risk class: 100%
  * precision of high-risk class: 87%
  * recall of low_risk class: 100%
  * recall of high-risk class: 100%

## Summary
Between the two models, the one trained on balanced data is a better option because its performance on healthy loans is not degraded, but its performance on high-risk loans is improved. 
The importance of each class depends on the application. For example identifying healthy loans can be essential to de_risk investing in peer-to-peer loans; on the other hand, identifying high-risk loans can be necessary for the lending platform not to approve it for their market health.

