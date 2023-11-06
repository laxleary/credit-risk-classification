# Credit Risk Classification
## Module 20 Challenge

### Overview
This repository uses basic supervised machine learning methods to train and evaluate a model of loan risk. First, the provided data is split into testing and training data, then a logistic regression model is developed to predict whether a loan is healthy or high-risk, and a credit risk analysis report is developed (included here)

### Credit Risk Analysis Report
#### Results

* Logistic Regression Model:
  * The model has a precision score of approximately 99% for healthy loans, so it does not often make the mistake of calling a high-risk loan healthy. The model has a precision of 85% for high-risk loans, so approximately one in six loans declared high-risk by the model are actually healthy loans. 
  * The model has extremely high recall (99%) for the healthy loans, again likely because of the large number of healthy loans compared to the number of high-risk loans. For high-risk loans, the value of 91% recall indicates that approximately 9% of high-risk loands will be "missed", or labelled incorrectly as healthy.
  * The accuracy of the model is about 99%, which indicates that 99% of all results are correct.


#### Summary

Despite having 99% accuracy, the model does not catch about 9% of high-risk loans, and about 1 in 6 of its high-risk predictions will actually be 
healthy loans. The issue in high-risk precision is not likely to be a problem for the bank. This causes them to lose clients who might otherwise have healthy loans, but such cases only account for 0.05% of all applications. However, the first problem (recall) is likely to be an issue for the lenders. High-risk loans can be extremely costly, and missing about one in 10 creates a huge potential for loss. I would recommend that the lenders use this model as a basis for decisions but then follow up with further models or research. Alternatively, one might add some weights to the decision-making ability of this model. For example, if a loan is for a small amount of money, we might be willing to rely more heavily on it despite its potential for error, while if a loan is for a large amount of money we might be more cautious about trusting the model. Overall, a better model might predict the odds of the borrower defaulting on the loan rather than just a yes/no prediction of whether the borrower will default. 

### Outside Resources
The included code was developed exclusively using the starter code provided and knowledge obtained during class. No TAs, instructors, or other students were consulted for help in developing the code.
