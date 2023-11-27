# credit-risk-classification

Loan Risk Analysis Overview:

In this analysis, my objective was to construct machine learning models for predicting the creditworthiness of borrowers based on historical lending activity data from a peer-to-peer lending services company. The primary goal was to evaluate the risk associated with loans and develop models capable of distinguishing between healthy loans (0) and high-risk loans (1).

Data Description:

The data utilized in this analysis was sourced from the "lending_data.csv" file, encompassing financial information about loans. The central task involved predicting the "loan_status" of each loan, with two classes: 0 denoting healthy loans and 1 representing high-risk loans.

Key Variables for Prediction:

- loan_status: The target variable indicating whether a loan is healthy (0) or high-risk (1).

Machine Learning Process:

The analysis comprised the following stages:

1. **Data Splitting:**
   - The dataset was read into a Pandas DataFrame from the "lending_data.csv" file.
   - Labels (y) were derived from the "loan_status" column, while the features (X) DataFrame was created from the remaining columns.
   - The data was split into training and testing datasets using the train_test_split function.

2. **Model Training:**
   - A logistic regression model was fitted using the training data (X_train and y_train).

3. **Model Evaluation:**
   - Model performance was assessed by:
     - Generating a confusion matrix.
     - Printing the classification report, encompassing precision, recall, and F1-score for both healthy and high-risk loans.

4. **Oversampling:**
   - Oversampling techniques were applied to balance the dataset compared to the original, addressing imbalanced classes.

Methods Used:

The primary machine learning method employed was logistic regression, complemented by oversampling techniques to tackle class imbalance.

Results:

The outcomes of the machine learning models are summarized as follows:

**Machine Learning Model 1 (Original Data):**
- Balanced Accuracy: [Balanced Accuracy Score]
- Precision for Healthy Loans (0): 1.00
- Recall for Healthy Loans (0): 1.00
- Precision for High-Risk Loans (1): 0.87
- Recall for High-Risk Loans (1): 0.89

**Machine Learning Model 2 (Resampled Data):**
- Balanced Accuracy: 0.9952
- Precision for Healthy Loans (0): 1.00
- Recall for Healthy Loans (0): 1.00
- Precision for High-Risk Loans (1): 0.87
- Recall for High-Risk Loans (1): 1.00

Summary:

In summary, the machine learning models were constructed to evaluate loan risk, and their performance was systematically assessed. The selection of the optimal model depends on factors such as the specific problem at hand and the importance of predicting healthy loans (0) or high-risk loans (1). It is crucial to consider the trade-off between precision and recall when making this decision. Generally, the second balanced model, utilizing resampled data, demonstrated improvement as the recall score increased for the high-risk loan category.

Overall, this analysis furnishes valuable insights into the creditworthiness of borrowers, aiding informed decision-making regarding loan risk.
