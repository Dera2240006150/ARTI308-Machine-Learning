# K-Nearest Neighbors (KNN) Project

## Description
This repository contains the laboratory solution for the K-Nearest Neighbors assignment for ARTI308 - Machine Learning. The objective of this project is to build and optimize a KNN classifier to predict target classes based on a set of anonymized feature data.

## Author
**Dera Aldosari** (ID: 2240006150)

## Repository Structure
* `KNN_AssignmentSolution.ipynb`: The main Jupyter Notebook containing the data exploration, model training, parameter tuning, and final evaluation.
* `KNN_Project_Data`: The dataset used to train and test the model.

## Workflow & Results
1.  **Exploratory Data Analysis (EDA):** Visualized the dataset using Seaborn pairplots to understand the relationships between the anonymized features and the target class.
2.  **Data Standardization:** (Standardized the features if applicable to the workflow).
3.  **Model Optimization:** The baseline model was evaluated, and the `n_neighbors` parameter was tuned to find the optimal K-value.
4.  **Final Performance:** By retraining the model with `K=23`, the classifier achieved a balanced **accuracy and F1-score of 0.87**, effectively minimizing false positives and false negatives.

## Technologies Used
* **Python 3**
* **Pandas & NumPy** (Data manipulation and analysis)
* **Matplotlib & Seaborn** (Data visualization)
* **Scikit-Learn** (Machine Learning modeling and evaluation)

## How to Run
To run this project locally:
1. Clone the repository.
2. Ensure you have the required libraries installed (`pip install pandas numpy matplotlib seaborn scikit-learn`).
3. Open `KNN_AssignmentSolution.ipynb` in Jupyter Notebook or JupyterLab.
4. Run all cells. Ensure `KNN_Project_Data` is in the same directory as the notebook.
