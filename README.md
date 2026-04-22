# Lab 9: Decision Trees and Random Forests

## Project Overview
This project explores publicly available financial data from LendingClub.com, a platform that connects borrowers with investors. The goal of this lab is to build and compare machine learning models (Decision Trees and Random Forests) to predict whether or not a borrower will pay back their loan in full.

## Dataset
The dataset consists of lending data from 2007–2010. 
Key features include:
* `credit.policy`: Whether the customer meets the credit underwriting criteria.
* `purpose`: The purpose of the loan (e.g., credit card, debt consolidation, small business).
* `int.rate`: The interest rate of the loan.
* `fico`: The FICO credit score of the borrower.
* `not.fully.paid`: The target variable (1 if the loan was not fully paid, 0 if it was).

## Libraries Used
* **Pandas & NumPy:** Data manipulation and analysis
* **Matplotlib & Seaborn:** Data visualization and exploratory data analysis (EDA)
* **Scikit-Learn:** Model building, training, and evaluation (`DecisionTreeClassifier`, `RandomForestClassifier`, `classification_report`, `confusion_matrix`)

## Key Findings
The dataset is highly imbalanced, which impacts the models' ability to identify the minority class (defaulters). While the Random Forest model performs better in overall accuracy compared to a single Decision Tree, its recall for the minority class highlights the standard trade-offs encountered when using ensemble methods on imbalanced data.
