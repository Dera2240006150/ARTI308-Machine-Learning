# ARTI 308 – Lab 5: Feature Engineering (Classification) 🍔🛵

## Overview
This repository contains the completed tasks for **Lab 5: Feature Engineering** in the ARTI 308 course. The objective of this lab is to build a baseline classification model to predict `Order_Status` (e.g., Delivered, Cancelled) using a Talabat-style food delivery dataset. 

Since the dataset was already clean (no missing values or duplicates), the primary focus of this project is on **feature engineering**, evaluating model performance, and interpreting feature importances using a Random Forest Classifier.

## Dataset
* **File:** `talabat_enhanced_orders.csv`
* **Description:** Contains 100,000 records of food delivery orders with features including order time, delivery distance, items ordered, pricing, and precise geocoordinates for the customer, restaurant, and driver.

## Key Tasks & Implementations

* **Base Preprocessing:** Engineered initial time-based features (order hour, weekend indicator) and price-based features (price per item). Implemented a vectorized Haversine distance function to calculate geographical distances.

* **Task 1: Spatial Feature Engineering:** Created a new feature, `driver_to_rest_distance_km`, calculating the initial distance a driver must travel to reach the restaurant. This serves as a strong predictive signal for potential order delays or cancellations.

* **Task 2: Temporal Feature Engineering:** Redefined the `is_peak_hour` rule to strictly target the evening dinner rush (18:00 - 22:00) to better capture high-traffic delays.

* **Task 3: Categorical Dimensionality Reduction:** Experimented with the `top_k` threshold (10, 30, and 50) for the `Item_Name` feature. Replaced less frequent items with an "Other" category to reduce the cardinality of the dataset before applying One-Hot Encoding. Evaluated how this affected model accuracy and feature importance.

* **Task 4: Feature Selection:** Utilized Scikit-Learn's `SelectFromModel` with a median threshold to drop the bottom 50% of the least important features. Proved that dropping noisy/unimportant features maintains (or slightly improves) model accuracy while significantly reducing model complexity and training time.

## Technologies & Libraries Used
* **Python 3**
* **Pandas & NumPy:** Data manipulation and vectorized calculations.
* **Scikit-Learn:** Machine learning pipeline (`Pipeline`, `ColumnTransformer`, `OneHotEncoder`), classification (`RandomForestClassifier`), and evaluation metrics.
* **Matplotlib & Seaborn:** Data visualization.

## How to Run
1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed (`pip install pandas numpy scikit-learn matplotlib seaborn`).
3. Place the `talabat_enhanced_orders.csv` dataset in the same directory as the notebook.
4. Open `Lab_5.ipynb` in Jupyter Notebook or Google Colab and run all cells.
