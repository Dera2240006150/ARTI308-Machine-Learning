# Lab 4: Data Quality Assessment & Preprocessing

## Overview
This repository contains the Jupyter Notebook for **Lab 4: Data Quality Assessment & Preprocessing**. In real-world machine learning projects, datasets are rarely perfect; they often contain missing values, noisy data (outliers), and inconsistent formats. This lab demonstrates a complete data preprocessing pipeline to clean and prepare a dataset before feeding it into a machine learning model.

## Dataset
* **File:** `Housing.csv`
* **Description:** A real estate dataset containing housing prices and various features such as area, number of bedrooms/bathrooms, and furnishing status. 

## Key Tasks & Concepts Covered
This lab systematically applies practical preprocessing techniques, including:

1. **Data Quality Assessment:** * Checking and correcting data types.
   * Mapping binary categorical string variables (e.g., 'yes'/'no') into machine-readable numeric formats (1/0).
2. **Handling Missing Values:** * Detecting `NaN` values.
   * Applying **Median Imputation** to handle missing data robustly, especially since real estate prices are heavily right-skewed and sensitive to extreme outliers.
3. **Outlier Detection & Handling:** * Visualizing data distribution using Boxplots.
   * Identifying outliers using the **Interquartile Range (IQR)** method.
   * Demonstrating strategies to either remove or cap extreme values (Percentile Method).
4. **Data Normalization & Scaling:** * Applying **Min-Max Normalization** to scale features between 0 and 1.
   * Applying **Z-Score Standardization** (using `StandardScaler`) to transform data to have a mean of 0 and a standard deviation of 1.
5. **Dimensionality Reduction (PCA):** * Checking feature correlation using heatmaps.
   * Applying **Principal Component Analysis (PCA)** to reduce highly correlated dimensions (like `price` and `area`) into a single principal component (PC1) while retaining the majority of the dataset's variance.

## Technologies Used
* **Python 3**
* **Pandas** (Data manipulation)
* **NumPy** (Numerical operations)
* **Matplotlib & Seaborn** (Data visualization)
* **Scikit-Learn** (Preprocessing and PCA)

## How to Run
1. Clone the repository to your local machine.
2. Ensure you have Jupyter Notebook installed, along with the required libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`).
3. Open `Lab4.ipynb` in Jupyter Notebook or Jupyter Lab.
4. Run the cells sequentially to observe the data transformation pipeline.
