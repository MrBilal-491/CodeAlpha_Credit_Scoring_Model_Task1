# CodeAlpha_Credit_Scoring_Model_Task1
The Credit Scoring Model is designed to predict the creditworthiness of individuals by analyzing their past financial and personal data. The purpose of this model is to assist financial institutions in making informed lending decisions by classifying customers into categories of "Good Credit" and "Bad Credit" risk.
2. Dataset Overview
The model utilizes the German Credit dataset obtained from the UCI Machine Learning Repository. This dataset includes 1,000 entries and 20 input features, consisting of both numerical and categorical data. Each entry represents a loan applicant with information such as:
•	Checking account status
•	Credit history
•	Loan purpose
•	Credit amount
•	Duration of the loan
•	Age, job, and housing
•	Employment status
•	Personal status and other financial indicators
The target variable is "credit_risk," which is binary: 0 (Good Credit), 1 (Bad Credit).
3. Objective
The primary goal is to create a predictive model that accurately classifies individuals based on their credit risk. By doing so, the model aims to:
•	Reduce default risk for lenders
•	Automate the credit approval process
•	Ensure fair and data-driven decision making
4. Algorithms Used
Three classification algorithms are employed to build and evaluate the model:
4.1 Logistic Regression
•	A statistical model used for binary classification.
•	Estimates the probability of a binary outcome using the logistic function.
•	Suitable for linearly separable data.
•	Outputs probabilities which can be thresholded to classify credit risk.
4.2 Decision Tree Classifier
•	A non-linear model that splits the data based on decision rules.
•	Builds a tree where internal nodes represent tests on features, and leaves represent the output label.
•	Easily interpretable and handles both numerical and categorical data.
4.3 Random Forest Classifier
•	An ensemble model consisting of multiple decision trees.
•	Each tree is trained on a random subset of the data and features.
•	Improves accuracy and reduces overfitting compared to a single decision tree.
•	Provides feature importance scores.
5. Key Features and Preprocessing
•	Feature Engineering: Separating numerical and categorical variables.
•	Scaling: Numerical features are standardized using StandardScaler.
•	Encoding: Categorical features are transformed using OneHotEncoder.
•	Handling Imbalance: Models use class_weight='balanced' to address class imbalance in credit risk.
6. Model Evaluation
Each model is evaluated using the following metrics:
•	Classification Report: Includes precision, recall, F1-score for both classes.
•	Confusion Matrix: Visual representation of correct and incorrect predictions.
•	ROC-AUC Score: Measures the model's ability to distinguish between good and bad credit.
•	ROC Curve: Graph showing the trade-off between true positive rate and false positive rate.
7. Results Visualization
The implementation displays:
•	Confusion matrices as heatmaps
•	ROC curves for all three models
•	AUC scores to compare model performance
