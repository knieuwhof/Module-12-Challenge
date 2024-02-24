# Module-12-Challenge

## Credit Risk Analysis Report

### Overview of the Analysis:

Credit risk poses a classification problem that’s inherently imbalanced. The reason for this is that healthy loans easily outnumber risky loans. For this Challenge, I used various techniques to train and evaluate models with imbalanced classes. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

### The Results:

**Logistic regression model, fit with the original data:**
- Balanced accuracy score: 97.2%
- Precision scores:
  - Class 0: 1.00
  - Class 1: 0.87
- Recall scores:
  - Class 0: 1.00
  - Class 1: 0.95

**Logistic regression model, fit with the resampled data:**
- Balanced accuracy score: 99.6%
- Precision scores:
  - Class 0: 1.00
  - Class 1: 0.87
- Recall scores:
  - Class 0: 1.00
  - Class 1: 1.00

### Summary:

The RandomOverSampler technique was used to resample the data and balance the value counts of each data set. Overall, we can see that the logistic regression model fit with the resampled data outperformed the model fit with the original data. Noted by the bulleted points above, the balanced accuracy score for the model fit with resampled data was 99.6%, compared to 97.2% with the original data. The recall scores for the model fit with resampled data were 1.0 for both class “0” and class “1” – meaning the model was able to correctly identify all actual healthy loans and all actual high-risk loans. The precision scores for both models were the same. As demonstrated by these results, we can distinguish that the model fit with the resampled data is recommended as it demonstrates a stronger ability to distinguish between healthy and high-risk loans.



