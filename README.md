# Module-12

Using your knowledge of the imbalanced-learn library, you’ll use a logistic regression model to compare two versions of the dataset. First, you’ll use the original dataset. Second, you’ll resample the data by using the RandomOverSampler module from the imbalanced-learn library.
For both cases, you’ll get the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.
As part of the README.md file in your GitHub repository, you’ll create a credit risk analysis report based on the provided template in your Starter_Code folder.
Files

Download the following files to help you get started:
Module 12 Challenge files
Instructions

The instructions for this Challenge are divided into the following subsections:
Split the Data into Training and Testing Sets
Create a Logistic Regression Model with the Original Data
Predict a Logistic Regression Model with Resampled Training Data
Write a Credit Risk Analysis Report
Split the Data into Training and Testing Sets

Open the starter code notebook, and then use it to complete the following steps:
Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
NOTE
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.
Check the balance of the labels variable (y) by using the value_counts function.
Split the data into training and testing datasets by using train_test_split.
Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:
Fit a logistic regression model by using the training data (X_train and y_train).
Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
Evaluate the model’s performance by doing the following:
Calculate the accuracy score of the model.
Generate a confusion matrix.
Print the classification report.
Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?
Predict a Logistic Regression Model with Resampled Training Data

Did you notice the small number of high-risk loan labels? Perhaps, a model that uses resampled data will perform better. You’ll thus resample the training data and then reevaluate the model. Specifically, you’ll use RandomOverSampler.
To do so, complete the following steps:
Use the RandomOverSampler module from the imbalanced-learn library to resample the data. Be sure to confirm that the labels have an equal number of data points.
Use the LogisticRegression classifier and the resampled data to fit the model and make predictions.
Evaluate the model’s performance by doing the following:
Calculate the accuracy score of the model.
Generate a confusion matrix.
Print the classification report.
Answer the following question: How well does the logistic regression model, fit with oversampled data, predict both the 0 (healthy loan) and 1 (high-risk loan) labels?
Write a Credit Risk Analysis Report

For this section, you’ll write a brief report that includes a summary and an analysis of the performance of both machine learning models that you used in this Challenge. You should write this report as part of the README.md file that your GitHub repository includes.
Structure your report by using the report template that Starter_Code.zip includes, and make sure that it contains the following:
An overview of the analysis: Explain the purpose of this analysis.
The results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of both machine learning models.
A summary: Summarize the results from the machine learning models. Compare the two versions of the dataset predictions. Include your recommendation, if any, for the model to use the original vs. the resampled data. If you don’t recommend either model, justify your reasoning.



Sources- ChatGpt Xpeert Learning Assistant