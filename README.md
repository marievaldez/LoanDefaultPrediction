# LoanDefaultPrediction
This code explores different techniques to build an interpretable binary classification model that predicts which clients will likely default on a home equity loan product based on data used to evaluate recently approved loans.

## Problem statement
The bank’s consumer credit department aims to streamline its home equity loans’ underwriting process using a predictive modeling technique. Per regulations, this model has to be explainable, as the bank needs to justify any adverse behavior (rejections).

## Proposed solution and its benefits
The proposed solution is to include a tuned XGBoost loan default prediction classifier in the home equity loan application process. This model:
* Identifies loan defaults with a recall of 83%, precision of 72%, and overall accuracy of 90%.
* Performs consistently on the training and test data.
* Based on a widely-used, efficient, and scalable machine learning algorithm (XGBoost) that combines many decision trees to form a robust classifier.
* Can be explained at a general and individual level, meaning rejections can be explained.

This model employs the following as the top 5 most important features in predicting a loan default. 
1.	Availability of debt-to-income ratio
2.	Number of delinquent loans
3.	Age of the oldest credit line
4.	Debt-to-income ratio 
5.	Value of the property

When implemented, this solution can:
* Improve the bank’s loan portfolio quality by reducing defaults, saving the bank on costs related to defaults.
* Improve loan processing time, which can then increase revenue with an increase in good-quality loans and more efficient use of available loan capital.
* Improve data accuracy and quality. Rejected loans can be flagged for review for data accuracy and completeness. 

## Methodology
This proposed model was chosen from different iterations of logistic regression and decision-tree-based algorithms. It is generalized and has the best performance among tested models. (See below.) The model was trained on data obtained via the existing loan underwriting process from recent applicants approved for credit. This dataset has missing values and also has outliers. The missing values were imputed based on similar records, and outliers were trimmed. 

<img width="410" alt="image" src="https://user-images.githubusercontent.com/38260314/235371579-af5efb7c-4dbc-4526-9931-58b7564bbfc2.png">
