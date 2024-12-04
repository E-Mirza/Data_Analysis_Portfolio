# Data_Analysis_Portfolio
## Projects
1. [Home Credit Default Risk](https://github.com/E-Mirza/Data_Analysis_Portfolio/tree/main/Home%20Credit%20Default%20Risk)
   ### Overview:
   #### Default Risk:
   When borrowers cannot make contractual payments, default risk can occur.
   Many people face challenges securing loans due to limited or no credit history, often falling prey to untrustworthy lenders. Home Credit Group aims to enhance financial 
   inclusion by offering safe, positive borrowing experiences for the unbanked, using alternative data like telco and transactional information to assess repayment ability.
   Doing so will ensure that clients capable of repayment are not rejected and that loans are given with a principal, maturity, and repayment calendar that will empower 
   their clients to be successful. The main objective of this project is to predict the binary outcome of the TARGET variable, which indicates loan default.
   ### Business Problem
   Lenders need to assess the likelihood of borrowers defaulting on loans to mitigate financial losses. Ineffective risk evaluation can lead to approving loans for high-risk 
   borrowers or rejecting low-risk applicants. This project aims to leverage data-driven insights and machine learning models to improve default predictions.
   ### Project Objective
   The objective of this project is to analyze the **Home Credit Default Risk** dataset and:
   1. Perform exploratory data analysis (EDA) to uncover key trends, patterns, and relationships influencing loan defaults.
   2. Identify critical predictors for credit risk assessment.
   3. Build predictive models using machine learning techniques, including **XGBoost**, **logistic regression**, and **random forest**, to forecast default probabilities.
   4. Evaluate model performance to ensure accurate and actionable insights, enabling lenders to make informed decisions and minimize financial risk.
   ### Data Sources:
   The data is provided by Home Credit, a service dedicated to provided lines of credit (loans) to the unbanked population. Predicting whether or not a client will repay a 
   loan or have difficulty is a critical business need, and Home Credit wants to unlock the full potential of their data to see what sort of machine learning/deep learning      models can be develop to help them in this task.
   ### Data Exploration:
   Data Exploration is a process where we analyze data to find trends, patterns, anomalies, or relationships. The goal is to understand what the data can reveal. It usually 
   starts with a broad overview and then focuses on specific details as we find interesting areas. The insights gained can be valuable on their own or help guide decisions 
   for modeling, such as selecting which features to use.
   Exploratory Data Analysis (EDA)
      ### Key findings from EDA include:
   #### Target Distribution:
   91.9% of loans are non-defaults (TARGET=0), and 8.1% are defaults (TARGET=1).
   #### Age and Defaults:
   Younger borrowers (20-30 years) show the highest default rates, while older borrowers (65+ years) have the lowest.
   #### Education Levels:
   Borrowers with higher education or academic degrees are less likely to default compared to those with lower secondary education.
   #### Loan Amounts:
   Higher average loan amounts are associated with defaulters in some education and income groups.
   #### Income Groups:
   Borrowers with very high incomes take larger loans, but default patterns do not vary significantly across income groups.
   #### Key Correlations:
   EXT_SOURCE_3, EXT_SOURCE_2, and EXT_SOURCE_1 have strong negative correlations with default risk.
   Demographic factors like DAYS_BIRTH also show moderate correlations.
   #### Late Payments:
   Defaults are slightly associated with a higher number of late payments, but extreme outliers exist.













   
