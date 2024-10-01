
# Loan Approval Prediction

This project uses a dataset to predict the approval status of loans based on various applicant and loan attributes. The dataset includes information such as the applicant's age, income, employment length, home ownership status, loan intent, and credit history.

## Table of Contents
- [Dataset Description](#dataset-description)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [How to Use](#how-to-use)
- [Conclusions](#conclusions)

## Dataset Description

The dataset contains 58,645 rows and 13 columns, including:

- **person_age**: Age of the loan applicant.
- **person_income**: Annual income of the loan applicant.
- **person_home_ownership**: Whether the applicant owns or rents a home.
- **person_emp_length**: Length of employment in years.
- **loan_intent**: The intended use of the loan (e.g., education, medical, personal).
- **loan_grade**: The loan’s grade (e.g., A, B, C).
- **loan_amnt**: Loan amount.
- **loan_int_rate**: Interest rate on the loan.
- **loan_percent_income**: The percentage of the applicant's income that will be used to repay the loan.
- **cb_person_default_on_file**: Whether the applicant has a history of defaults (Y/N).
- **cb_person_cred_hist_length**: Length of the applicant’s credit history.
- **loan_status**: The target variable (0 for not approved, 1 for approved).

## Data Preprocessing

The data preprocessing steps include:

- Handling missing values.
- Encoding categorical variables (e.g., home ownership, loan intent, loan grade).
- Feature scaling and normalization where necessary.
- Splitting the data into training and testing sets.

## Exploratory Data Analysis (EDA)

EDA includes:

- Visualizations of the distribution of numerical features such as income and loan amounts.
- Correlation analysis to identify relationships between variables and the target.
- Analysis of categorical features and their impact on loan approval.

## Modeling

Various machine learning models were explored, including:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting

The models were trained on the preprocessed dataset and evaluated using metrics such as accuracy, precision, recall, and F1-score.

## Evaluation

Model performance was evaluated using the following metrics:

- **Accuracy**: Percentage of correct predictions.
- **Precision**: The proportion of positive identifications that were correct.
- **Recall**: The proportion of actual positives that were identified correctly.
- **F1 Score**: The harmonic mean of precision and recall.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/loan-approval-prediction.git
   ```
2. Install the necessary libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook to train models and make predictions:
   ```bash
   jupyter notebook Loan_approval_playground.ipynb
   ```

## Conclusions

This project demonstrates how machine learning models can be applied to predict loan approval using features related to an applicant's personal and financial background. The Random Forest and Gradient Boosting models showed promising results in terms of accuracy and interpretability.
