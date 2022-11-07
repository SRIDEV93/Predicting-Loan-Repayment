# Predicting-Loan-Repayment

# Understanding the Data
Before we start cleaning data for a machine learning project, it is vital to understand what the data is, and what we want to achieve. Without that understanding, we have no basis from which to make decisions about what data is relevant as we clean and prepare our data. We'll be working with some data from Lending Club, a marketplace for personal loans that matches borrowers who are seeking a loan with investors looking to lend money and make a return. Each borrower fills out a comprehensive application, providing their past financial history, the reason for the loan, and more. Lending Club evaluates each borrower's credit score using past historical data (and their own data science processs!) and assigns an interest rate to the borrower. Approved loans are listed on the Lending Club website, where qualified investors can browse recently approved loans, the borrower's credit score, the purpose for the loan, and other information from the application.Once an investor decided to fund a loan, the borrower then makes monthly payments back to Lending Club. Lending Club redistributes these payments to investors. This means that investors don't have to wait until the full amount is paid off to start to see returns. If a loan is fully paid off on time, the investors make a return which corresponds to the interest rate the borrower had to pay in addition to the requested amount. Many loans aren't completely paid off on time, however, and some borrowers default on the loan. That's the problem we'll be trying to address as we clean some data from lending club for machine learning. Let's imagine we've been tasked with building a model to predict whether borrowers are likely to pay or default on their loans.

# Dataset
The dataset is taken from lending_club_loans.csv.

# Data Preprocessing
* Initially the size of the dataset is large i.e., it has 42538 rows and 115 columns. It has more unncessary columns. So we have to remove them. Removing all the columns with morethan 50% missing values: This allows us to work faster.
* Remove the 'desc' column: It contains a long text explanation for the loan that we don't need. Remove the 'url' column: It contains a link to each on Lending Club which can only be accessed with an investor account.

# Further Cleaning
Here, Iam taking data dictionary from LendingClub provides to help us become familiar with the columns and what each column represents in the dataset. To make the process easier, we'll create a DataFrame that contains the names of the columns, datatype, first row values, and description from the data dictionary.

** Here I spilt the dataset into 3 group to better understand and for better cleaning. And then The cleaned dataset is named into a variable called Dataset. The final size of the dataset is (38123, 39)

# Exploratory Data Analysis

Here I started by analysing the distribution of loan_status and found that 85% of the loans were paid on time. And then I performed data analysis for each of the feature with the loan status. 

# Making predictions

For this classification problem, The models I used are Logistic Regression, Decision Tree, KNearest Neighbours, Random Forest and Support Vector Classification. Among these models which model is giving the best prediction is concluded with its accuracy score.

The Accuracy score 
      *   Logistic Regression is 85.95%
      *   Decision Tree is 76.15%
      *   Random Forest is 85.86%
      *   KNNeighbour is 85.94%
      *   Support vector Classification is 85.96%

# Conclusion

Here I am concluding that based on accuracy scores, support vector classification and Logistic Regression are giving almost similar accuracy among all other models to predict whether the applicant will repay their loan or not before issuing them. 




