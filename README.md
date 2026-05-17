# Credit Card Customer Segmentation

This project applies unsupervised machine learning techniques to segment credit card customers based on their usage behavior. By identifying distinct customer groups, businesses can design better, more targeted marketing strategies.

## Project Overview
This project was developed for the **ARTI308 - Machine Learning** course. It uses **K-Means Clustering** to analyze customer-level credit card usage data, grouping individuals with similar financial behaviors together. 

## Dataset
The project uses the **Credit Card Dataset** (`CC_GENERAL.csv`), which contains behavioral variables for various credit card holders.
* **Source:** [Kaggle - Credit Card Dataset](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata/data)
* **Features:** The dataset includes features such as balance, purchases, cash advance, payments, and account tenure.

## Objectives
* Apply K-Means clustering to identify distinct customer segments without pre-existing target labels.
* Analyze the behavioral traits of each cluster.
* Provide actionable marketing strategies tailored to each segment.

## Key Customer Segments Identified
Through clustering, the following customer profiles were identified:
1. **Premium Spenders:** High-volume spenders. Strategy: Offer luxury rewards, travel points, and premium perks to maintain loyalty.
2. **Cash Advance Users:** Users who frequently carry debt. Strategy: Offer balance transfer promotions and debt consolidation options, while monitoring credit risk.
3. **Installment Shoppers:** Users who prefer paying over time. Strategy: Offer cash-back on daily spending and promote "buy now, pay later" features.
4. **Low Activity Users:** Rarely use their cards. Strategy: Send targeted activation campaigns and spending bonuses to encourage usage.

## Tech Stack
* **Language:** Python 3
* **Environment:** Jupyter Notebook
* **Libraries:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn` (standard data science stack)

## How to Run
1. Clone the repository.
2. Ensure you have the required libraries installed (`pip install pandas numpy scikit-learn matplotlib seaborn`).
3. Download the `CC_GENERAL.csv` dataset from Kaggle and place it in the same directory as the notebook.
4. Open and run `02_Credit_Card_Customer_Segmentation.ipynb` in Jupyter Notebook or Jupyter Lab.
