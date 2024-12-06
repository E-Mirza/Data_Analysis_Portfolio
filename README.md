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
   3. Build predictive models using machine learning techniques, including **XGBoost**, **logistic regression**, and 
   **random forest**, to forecast default probabilities.
   4. Evaluate model performance to ensure accurate and actionable insights, enabling lenders to make informed decisions and 
   minimize financial risk.
   ### Data Sources:
   The data is provided by Home Credit, a service dedicated to provided lines of credit (loans) to the unbanked population. 
   Predicting whether or not a client will repay a 
   loan or have difficulty is a critical business need, and Home Credit wants to unlock the full potential of their data to 
   see what sort of machine learning/deep learning      models can be develop to help them in this task.
   ### Data Exploration:
   Data Exploration is a process where we analyze data to find trends, patterns, anomalies, or relationships. The goal is to 
   understand what the data can reveal. It usually 
   starts with a broad overview and then focuses on specific details as we find interesting areas. The insights gained can 
   be valuable on their own or help guide decisions 
   for modeling, such as selecting which features to use.
   Exploratory Data Analysis (EDA)
      ### Key findings from EDA include:
   #### Target Distribution:
   91.9% of loans are non-defaults (TARGET=0), and 8.1% are defaults (TARGET=1).
   #### Age and Defaults:
   Younger borrowers (20-30 years) show the highest default rates, while older borrowers (65+ years) have the lowest.
   #### Education Levels:
   Borrowers with higher education or academic degrees are less likely to default compared to those with lower secondary 
   education.
   #### Loan Amounts:
   Higher average loan amounts are associated with defaulters in some education and income groups.
   #### Income Groups:
   Borrowers with very high incomes take larger loans, but default patterns do not vary significantly across income groups.
   #### Key Correlations:
   EXT_SOURCE_3, EXT_SOURCE_2, and EXT_SOURCE_1 have strong negative correlations with default risk.
   Demographic factors like DAYS_BIRTH also show moderate correlations.
   #### Late Payments:
   Defaults are slightly associated with a higher number of late payments, but extreme outliers exist.

   ### My Contribution to the Project
   As part of a four-member team, I contributed to various aspects of the **Home Credit Default Risk** project. While all 
   group members worked collaboratively, one member achieved a particularly strong Kaggle score with their model, which we 
   collectively decided to use as our final submission. My specific contributions included: 
   - I analyzed the performance of all models created by the group, including **Logistic Regression**, **Random Forest**, 
   and **XGBoost**, to identify strengths and weaknesses.
   - I documented the evaluation metrics (e.g., accuracy, AUC, precision, recall) for each model to provide a clear 
   comparison.
   - I summarized the final results, explaining why the selected model (XGBoost) performed best, and highlighting its key 
   advantages.
   My role was integral in synthesizing insights and providing a clear narrative that tied together the team's efforts, 
   ensuring a cohesive and impactful final submission.

   ## Data Modelling:{https://github.com/E-    Mirza/Data_Analysis_Portfolio/blob/main/Home%20Credit%20Default%20Risk/Modeling.Rmd}
   Implemented and evaluated the following models:
   ### Logistic Regression
   ### Random Forest
   ### XGBoost

   ### Results:
   #### Logistic Regression
   AUC-ROC Score: 0.7365
   Logistic Regression demonstrated reliable performance, making it a strong baseline model for the dataset.
   #### Random Forest
   AUC-ROC Score: 0.6913
   Random Forest provided reasonable performance, although it fell short compared to Logistic Regression.
   #### XGBoost
   Training AUC-ROC: 1.0000
   Validation AUC-ROC: 0.4999
   XGBoost significantly overfit the training set and failed to generalize to the validation set, highlighting the need for 
   further tuning

   ### Challenges
   Class Imbalance:
   Required extensive preprocessing to balance the dataset.
   Overfitting in XGBoost:
   Despite tuning, the XGBoost model overfit the training data but performed poorly on the validation set.
   ### Solution to the Business Problem
   The goal of the project was to predict the likelihood of a client defaulting on their loan using machine learning 
   models. Based on the analysis:
   Logistic Regression emerged as the most effective model with an AUC-ROC of 0.7365, providing a reliable baseline for 
   identifying potential defaulters.
   This solution can be used by lenders to assess credit risk, enabling better decision-making for loan approvals and 
   reducing financial losses caused by defaults.
   ### Business Value of the Solution
   #### Improved Risk Assessment:
   The model allows lenders to flag high-risk applicants, minimizing loan defaults and improving profitability.
   #### Efficient Resource Allocation:
   Helps prioritize resources for collections or additional investigations into flagged applications.
   #### Compliance with Financial Regulations:
   Ensures responsible lending practices by evaluating the creditworthiness of applicants.
   
   ### Difficulties Encountered
   #### Class Imbalance:
   The dataset had significantly more non-default cases than default cases, requiring techniques like SMOTE and careful 
   metric selection (e.g., ROC instead of accuracy).
   #### Overfitting in XGBoost:
   XGBoost overfit the training data due to insufficient tuning and complexity of the model. Extensive trial-and-error 
   tuning was needed, but it still failed to generalize well.
   #### Large Dataset Processing:
   Handling the large dataset required optimizing preprocessing and leveraging parallel computing to reduce runtime.
   #### Group Coordination:
   Balancing tasks among group members and ensuring consistent approaches in preprocessing and evaluation posed challenges.

   ## What I Learned
   #### Importance of Preprocessing:
   Handling missing values, class imbalances, and feature scaling are critical to building reliable models.
   #### Model Evaluation:
   Using metrics like AUC-ROC is more insightful than accuracy, especially with imbalanced datasets.
   #### Strengths and Limitations of Algorithms:
   Logistic Regression is simple yet effective for baseline performance.
   Complex models like XGBoost require careful tuning to avoid overfitting.
   #### Team Collaboration:
   Dividing roles (e.g., preprocessing, modeling, and evaluation) and combining efforts led to a well-rounded solution.
   #### Iterative Approach:
   Modeling involves continuous testing, refinement, and validation to achieve optimal results.

   ## Summary
   The project provided valuable insights into predicting loan defaults using machine learning. Logistic Regression emerged 
   as the most suitable model, striking a balance between interpretability and performance. The solution offers significant 
   business value by aiding lenders in better credit risk management. Despite challenges like class imbalance and 
   overfitting, the team successfully implemented a robust process and gained practical experience in data science 
   workflows.
  






   
