
## Overview
This repository contains a Jupyter Notebook (`02-SVM Assignment_filled.ipynb`) demonstrating the implementation, evaluation, and tuning of a Support Vector Machine (SVM) classifier. The model is trained to classify the species of Iris flowers using the famous [Iris flower data set](http://en.wikipedia.org/wiki/Iris_flower_data_set).

## Dataset
The Iris dataset consists of 150 samples from three species of Iris (*Iris setosa*, *Iris virginica*, and *Iris versicolor*). Four features are measured from each sample:
* Sepal length (cm)
* Sepal width (cm)
* Petal length (cm)
* Petal width (cm)

## Dependencies
Ensure you have the following Python libraries installed to run the notebook:
* `pandas`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `IPython`

## Project Workflow
1. **Data Loading & Formatting:** * Loaded the built-in Iris dataset using `sklearn.datasets` and formatted it into a pandas DataFrame for easier handling.
2. **Exploratory Data Analysis (EDA):**
   * Generated a pairplot using `seaborn` to visualize feature relationships and species separability (noting that *Iris setosa* is highly separable).
   * Created a KDE (Kernel Density Estimation) plot of sepal length versus sepal width specifically for the *setosa* species.
3. **Data Preprocessing:**
   * Separated the dataset into features (`X`) and target labels (`y`).
   * Performed a Train-Test split (70% training, 30% testing) using `train_test_split`.
4. **Model Training:**
   * Instantiated and trained a default Support Vector Classifier (`SVC`) from `scikit-learn`.
5. **Model Evaluation:**
   * Evaluated the base model using a Confusion Matrix and Classification Report.
   * Achieved high initial performance metrics (approx. 98% overall accuracy and f1-score).
6. **Hyperparameter Tuning:**
   * Utilized `GridSearchCV` to find the optimal combination of `C` and `gamma` parameters using a 3-fold cross-validation approach.
   * Parameter grid searched: `{'C': [0.1, 1, 10, 100], 'gamma': [1, 0.1, 0.01, 0.001]}`.
   * Retrained and evaluated the tuned model to ensure robust classification.

