# Time-Series-Classification
This is a project for my machine learning course focusing on classification of time series. I aim to classify the activities of humans based on time series obtained by a Wireless Sensor Network.

# Data Source:
https://archive.ics.uci.edu/ml/datasets/Activity+Recognition+system+based+on+Multisensor+data+fusion+\%28AReM\%29

# Data Description:
- 7 folders that represent 7 types of activities
- in each folder, there are multiple files each of which represents an instant of a human performing an activity
- Each file contains 6 time series collected from activities of the same person
- 88 instances in the dataset, each of which containes 6 time series and each time series has 480 consecutive values

# Tasks:
## Feature Extraction
- Extract the time-domain features (min, max, mean, median, sd, q1, q3) for all of the 6 time series in each instances.
- Bootstrap confidence interval for the standard deviation of each feaature
## Binary Classification: Classify bending from other activities using Logistic Regression
- Backward selection & Recursive Feature Elimination
- 5-fold cross-validation: report cross-validation accuracy
- Use stratified cross validation to handle class-imbalance
- Report confusion matrix, ROC, AUC, parameters, p-values
- Report accuracy on the test set
## Binary Classification: Classify bending from other activities using Logistic Regression with case-control sampling to handle imabalanced clasees
- Report confusion matrix, ROC, AUC, parameters, p-values
- Report accuracy on the test set
## Binary Classification: Classify bending from other activities using L1-penalized logistic regression
- Find optimal paraments through cross-validation
- Variable selection using p-values
## Multi-class Classification: Classify all activities using L1-penalized multinomial regression model
- Find optimal parameters through cross-validation
- Report test error & accuracy
- Report confusion matrices
## Multi-class Classification: Classify all activities using Gaussian Naive Bayes' Classifier
- Find optimal parameters through cross-validation
- Report test error & accuracy
- Report confusion matrices
## Multi-class Classification: Classify all activities using Multinomial Naive Bayes' Classifier
- Find optimal parameters through cross-validation
- Report test error & accuracy
- Report confusion matrices
