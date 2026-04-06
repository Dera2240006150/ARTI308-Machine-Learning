# E-Commerce Customers Spend Prediction

## Project Overview
This project applies Machine Learning to predict the **Yearly Amount Spent** by customers of an E-commerce company. The company sells clothing online but also offers in-store style and clothing advice sessions. Customers can order through a mobile app or a web platform. 

The goal of this project is to build a **Linear Regression** model to help the company decide whether they should focus their efforts on improving their mobile app experience or their website.

## Dataset
The dataset contains customer information with the following numerical features:
* **Avg. Session Length:** Average session of in-store style advice sessions.
* **Time on App:** Average time spent on the company's mobile app in minutes.
* **Time on Website:** Average time spent on the company's website in minutes.
* **Length of Membership:** How many years the customer has been a member.
* **Yearly Amount Spent:** The total amount the customer spent in a year (Target Variable).

## Technologies & Libraries Used
* **Python 3**
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-Learn** (Machine Learning & Modeling)

## Workflow & Methodology
1. **Exploratory Data Analysis (EDA):** Checking dataset structure, data types, and summary statistics.
2. **Data Cleaning & Feature Engineering:** Dropping non-numerical identifiers (Email, Address, Avatar) to prepare the data for the regression model.
3. **Train/Test Split:** Splitting the data into 70% training data and 30% testing data.
4. **Model Training:** Fitting a Multiple Linear Regression model using `scikit-learn`.
5. **Model Evaluation:** Predicting the test set results and calculating error metrics (MAE, MSE, RMSE).

## Results & Insights
The model performed exceptionally well with the following error metrics:
* **Mean Absolute Error (MAE):** 7.23
* **Root Mean Squared Error (RMSE):** 8.93

**Model Coefficients:**
* Avg. Session Length: **~25.98**
* Time on App: **~38.59**
* Time on Website: **~0.19**
* Length of Membership: **~61.28**

**Conclusion:** The model reveals that **Length of Membership** is the strongest driver of yearly spending. Between the two digital platforms, the **Mobile App** (Coefficient: 38.59) is vastly outperforming the **Website** (Coefficient: 0.19). The company should either focus on optimizing the mobile app further to maximize current success, or drastically overhaul the website to catch up to the app's performance.
