# CapstoneProject_Suchismita
### Using Machine Learning Model to predict the Loan Category (Good / Bad)


#### Executive summary

**Project overview and goals:** The goal of this project is to identify more effective ways for detecting the possibility of loan turning bad and evaluating the best model to capture those. Loan approval prediction using machine learning will offer lenders many benefits. Lenders can improve the accuracy of creditworthiness assessments, reduce the risk of defaults, and improve overall portfolio quality.



**Findings:** The best model for predicting the loan category is the Random Forest Classifier Model having an accuracy score of 0.96, recall of 0.96 and F1-score of 0.95. The second best model was Logistic Regression having accuracy score of 0.9238 and followed by KNN Neighbors having an accuracy of 0.9178. Initially 11 features were selected and feature selection was run and it was identified that features - emp_length_int, annual_income, loan_amount, interest_rate, total_pymnt, dti, year have significant contribution towards model training and prediction.
 

#### Rationale
Predictive analytics has played a pivotal role in streamlining the lending process. It helps lending companies gather relevant data of customers, identify frauds early, application screening, study past data and identify trends and patterns from past happenings and use it to predict future outcomes.

#### Research Question
The model would predict the loan category whether the loan defaults (Bad Loan)  or loan repaid (Good Loan). 

#### Data Sources
The data source used from Lending Club Information > Loan_Test

#### Methodology
	
# Data Exploration
The dataset contains 887379 rows and 55 columns. This dataset also contains considerable missing values for the features - emp_length (44825), mths_since_last_delinq (454312), mths_since_last_record (750326),
last_pymnt_d (17659), final_d (17659) , next_pymnt_d  (252971), emp_length_int (44825).

# Data Pre-Processing
For the features (which have significant influence on building the model) and have NULL values, mean has been calculated from the non-null values for that feature and the mean has been substituted for the null values. The dummy variables are created and using map method categorical variables are converted into integars.

# Feature Selection
Feature selection, also known as variable selection, is the process of selecting a subset of relevant features (variables, predictors) to efficiently train a Machine Learning Model which would most accurately predict the loan status.
Calculated RMSE for the selected features to find the minimum error.


#Model building and comparing the accuracy score
Split the dataset into test and train data. Used Logistic Regression Classifier, Random Forest Classifier and KNN Classfier to get the accuracy score for each and evaluate the best model



#### Results
It is observed that as average interest rates for loans started to increaase over the years from 2012 to 2015, the number of Bad Loans also increased. This can be also supported by the claim that Debt-Income ratio of the customers increased.
Random Forest Classifier is the best model to predict the loan category.

#### Next steps
Monitor the model performance for new data.

#### Outline of project
Reduce the loan default for the banks.

##### Contact and Further Information
ssanyal2018@gmail.com







