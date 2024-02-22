# Project-2 Predict Student Loan Repayment with Deep Learning
#### **Author: Saikumar Kalyankrishnan**

## Background
You work at a company that specializes in student loan refinancing. If the company can predict whether a borrower will repay their loan, it can provide a more accurate interest rate for the borrower. Your team has asked you to create a model to predict student loan repayment.

The business team has given you a CSV file that contains information about previous student loan recipients. With your knowledge of machine learning and neural networks, you decide to use the features in the provided dataset to create a model that will predict the likelihood that an applicant will repay their student loans. The CSV file contains a variety of information about these students, including their credit ranking.

## Goal
To create a Deep Learning model to predict student loan repayment.

## Steps
1. **Prepare the data for use on a neural network model.**
   * Using your knowledge of Pandas and scikit-learn’s `StandardScaler()`, preprocess the dataset so that you can use it to compile and evaluate the neural network model later. 
   * Read the data from https://static.bc-edx.com/mbc/ai/m6/datasets/student_loans.csv to an external site. into a Pandas DataFrame. Review the DataFrame, looking for columns that could eventually define your features and target variables. 
   * Create the features (`X`) and target (`y`) datasets. The target dataset should be defined by the “credit_ranking” column. The remaining columns should define the features dataset. 
   * Split the features and target sets into training and testing datasets. 
   * Use scikit-learn's `StandardScaler` to scale the features data.
2. **Compile and evaluate a model using a neural network.**
   * Use your knowledge of TensorFlow to design a deep neural network model. This model should use the dataset’s features to predict the credit quality of a student based on the features in the dataset. Consider the number of inputs before determining the number of layers that your model will contain or the number of neurons on each layer. Then, compile and fit your model. Finally, evaluate the model to calculate its loss and accuracy.
   * Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using Tensorflow’s Keras.
   * Compile and fit the model using the `mse` loss function, the `adam` optimizer, and the `mse` evaluation metric.
   * Evaluate the model using the test data to determine the model’s loss and accuracy. 
   * Save and export your model to an HDF5 file, and name the file `student_loans.h5`.
3. **Predict loan repayment success by using your neural network model.**
   * Use the model you saved in the previous section to make predictions on your reserved testing data.
   * Reload your saved model. 
   * Make predictions on the testing data. 
   * Create a DataFrame that includes both the predictions and the actual values. 
   * Display a sample of the DataFrame you created above. Compare the prediction and actual values in this sample and describe what you notice.


