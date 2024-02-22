# Project-1 Spam Detection Model
#### **Author: Saikumar Kalyankrishnan**

## Background
Let's say you work at an Internet Service Provider (ISP) and you've been tasked with improving the email filtering system for its customers. You've been provided with a dataset that contains information about emails, with two possible classifications: spam and not spam. The ISP wants you to take this dataset and develop a supervised machine learning model that will accurately detect spam emails, so it can filter them out of its customers' inboxes.

## Goal
To create two classification models to fit the provided data, and evaluate which model is more accurate at detecting spam. The two models are: 
1. Logistic Regression Model
2. Random Forest Model

## Steps
1. **Split the Data into Training and Testing Sets**
   * Read the data from https://static.bc-edx.com/mbc/ai/m4/datasets/spam-data.csv to an external site into a Pandas DataFrame. 
   * In the appropriate markdown cell, make a prediction as to which model you expect to do better. 
   * Create the labels set (`y`) from the “spam” column, and then create the features (`X`) DataFrame from the remaining columns. 
   * A value of 0 in the `spam` column means that the message is legitimate. A value of 1 means that the message has been classified as spam. 
   * Check the balance of the labels variable (`y`) by using the `value_counts` function. 
   * Split the data into training and testing datasets by using `train_test_split`.
2. **Scale the Features**
   * Create an instance of `StandardScaler`. 
   * Fit the Standard Scaler with the training data. 
   * Scale the training and testing features DataFrames using the transform function.
3. **Create a Logistic Regression Model**
   * Fit a logistic regression model by using the scaled training data (`X_train_scaled` and `y_train`). Set the `random_state` argument to `1`. 
   * Save the predictions on the testing data labels by using the testing feature data (`X_test_scaled`) and the fitted model. 
   * Evaluate the model’s performance by calculating the accuracy score of the model.
4. **Create a Random Forest Model** 
   * Fit a random forest classifier model by using the scaled training data (`X_train_scaled` and `y_train`). 
   * Save the predictions on the testing data labels by using the testing feature data (`X_test_scaled`) and the fitted model. 
   * Evaluate the model’s performance by calculating the accuracy score of the model.
5. **Evaluate the Models**
   * Which model performed better? 
   * How does that compare to your prediction?