#Financial Risk Analysis
Overview
This GitHub repository hosts code for a comprehensive Financial Risk Analysis project. The analysis involves merging application data with previous application data to predict the likelihood of loan default. Various machine learning models, including Random Forest, Decision Tree, Logistic Regression, and Support Vector Machine (SVM), are employed for this task.

Datasets
Application Data: Contains essential information about loan applicants.
Previous Application Data: Encompasses historical data on previous loan applications.
The datasets are merged based on the 'SK_ID_CURR' column to create a consolidated dataset for analysis.

Data Preprocessing
Handling Missing Values
Missing values for numeric columns are imputed with the mean, while non-numeric columns are imputed with the mode (most frequent value).

Data Type Handling
The 'TARGET' column is checked for data type. If it is 'object', an attempt is made to convert it to a numeric type.

Exploratory Data Analysis (EDA)
Financial Analysis
A scatter plot illustrates the relationship between income, credit amount, and the probability of loan default.
Count plots showcase the distribution of client family status, loan type, education, and employment status.
Loan Purpose Distribution
A bar plot visualizes the distribution of the top 10 loan purposes.

Feature Selection
Selected features for model training include 'NAME_EDUCATION_TYPE', 'NAME_INCOME_TYPE', 'AMT_DOWN_PAYMENT', 'AMT_APPLICATION', and 'NAME_PAYMENT_TYPE'.

Model Building and Evaluation
Decision Tree Classifier
A Decision Tree Classifier is trained and evaluated using confusion matrix and classification report metrics.
Logistic Regression
Logistic Regression is applied, and model performance is evaluated.
Support Vector Machine (SVM)
A Support Vector Machine model is implemented, and its performance is assessed.# Financial-Risk-Analysis


The better acuracy score by DecisiontreeClassifier 
[[256129   5167]
 [ 23978    757]]
              precision    recall  f1-score   support

           0       0.91      0.98      0.95    261296
           1       0.13      0.03      0.05     24735

    accuracy                           0.90    286031
   macro avg       0.52      0.51      0.50    286031
weighted avg       0.85      0.90      0.87    286031
