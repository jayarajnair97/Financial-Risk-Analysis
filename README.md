#<h1>Financial Risk Analysis<h1/>
<h2>Overview<h2/>
This GitHub repository hosts code for a comprehensive Financial Risk Analysis project. The analysis involves merging application data with previous application data to predict the likelihood of loan default. Various machine learning models, including Random Forest, Decision Tree, Logistic Regression, and Support Vector Machine (SVM), are employed for this task.

<h2>Datasets<h2/>
Application Data: Contains essential information about loan applicants.
Previous Application Data: Encompasses historical data on previous loan applications.
The datasets are merged based on the 'SK_ID_CURR' column to create a consolidated dataset for analysis.

<h3>Data Preprocessing<h3/>
Handling Missing Values
Missing values for numeric columns are imputed with the mean, while non-numeric columns are imputed with the mode (most frequent value).

Data Type Handling
The 'TARGET' column is checked for data type. If it is 'object', an attempt is made to convert it to a numeric type.

<h3>Exploratory Data Analysis (EDA)<h3/>
Financial Analysis
A scatter plot illustrates the relationship between income, credit amount, and the probability of loan default.
Count plots showcase the distribution of client family status, loan type, education, and employment status.
Loan Purpose Distribution
A bar plot visualizes the distribution of the top 10 loan purposes.

<h3>Feature Selection<h3/>
Selected features for model training include 'NAME_EDUCATION_TYPE', 'NAME_INCOME_TYPE', 'AMT_DOWN_PAYMENT', 'AMT_APPLICATION', and 'NAME_PAYMENT_TYPE'.

<h3>Model Building and Evaluation<h3/>
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

# Power Point Presentation link
https://docs.google.com/presentation/d/1xliygkI-Z8-aEULsfIbaejwP_KgPXOHe/edit?usp=drive_link&ouid=110042194959097886731&rtpof=true&sd=true
