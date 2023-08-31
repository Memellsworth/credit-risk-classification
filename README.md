# credit-risk-classification

## Machine Learning is applied to analyze data from a peer-to-peer lending services company's historical data. THis was done to identify the creditworthiness of borrowers

### Overview of the Analysis

## Factors concereded in the analysis include:
- The size of the loan
- Interest rate
- Borrowers income
- Debt to income ratio
- Borrower's number of accounts 
- Derogatory marks 
- Total debt 

the dataset had 77,536 data points. This was split into training and testing sets. 

## Analysis Methodology 

 - **Data Preprocessesing:** Importing the neccesary libraries, checked for  inbalanced classes, and divided into training and testing sets. 
 - **Model Training and Evaluation:**Trained a logistic regression module using the `LogisticRegression` module from `scikit-learn` on the original data to evaluate the performance using various methions like balanced accurac, confusion matrix and classification report
  - **Oversampling:** Due to class imblance, the `RandomOverSampler` technique to oversample the high-risk -loans in the training data to get better class balance 
 - **Modele Training and EvaluationL Trained another logistic regression using the oversampleded training data and evaluated the performance as we did with the original data

### Results 

## Model 1 

The logistic regression model shows a strong performance in predicting high-risk-loans  with a precision of 0.87, recall of 0.89. Meaning that the model correctly identifies a large amount of high-risk-loands along with minimizing the false positives.  In addition, the model has a strong performance in predicting low-risk loans. 

## Model Two 
The logistic regression with the oversampled data shows an even better performance in predicting high risk loans, still with a precision of 0.87, but with a recall of 1.00. While the model does predict a health loan (low-risk loan) at 100% s