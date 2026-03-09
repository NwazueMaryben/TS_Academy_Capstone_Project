# TS Academy Capstone Project | Group 9: Telco Customer Churn Prediction


## Table Of Contents <br>
* Project Overview <br>
* Dataset <br>
* Methodolgy <br>
* Key Notebook Sections <br>
* Model Performance & Comparison <br>
* Key Findings <br>
* Model Limitations <br>
* Business Justification & Recommendations <br>
Author <br>

## Project Overview <br>
This project focuses on building an end-to-end classification pipeline to predict customer churn for a telecommunnications provider.  The primary goal is identify customers at risk of churning using supervised learning techniques.  Retaining existing customers is often more cost-effective than acquiring new ones, whhcih makes churn prediction an importance business problem.<br>
* **Chosen Track**: Classification <br>
* **Problem Statement**:* Predict whether a telecom customer will churn (Yes/No) <br>

## Dataset<br>
**Telco Customer Churn Dataset (IBM)** <br>
The dataset contains 7,043 customer records with 21 features covering demographic information, service subscriptions and billing details. <br>

## Methodology <br>
The project follows a standard machine learning workflow: <br>
1. **Data Preprocessing:** Type conversion (specially TotalCharges to float), handling missing values and features selection. <br>
2. **Eploratory Data Analysis (EDA):** Analysis of churn distribution and relationship between features like Contract and Monthly Charges with the target. <br>
3. **Modeling:** Implementation of a **Baseline Logistic Regression** and an **Advanced Random Forest Classifier**. <br>
4. **Evaluation:** Assessment using Accuracy, Precision, Recall and FI-score. <br>
5. **Interpretation:** Analyzing features importance to understand what drives customer decisions. <br>

## Key Notebook Sections <br>
1. **Problem Framinf and Tracking Justification** <br>
Identified the project as a Supervised Learning (Classificiation) task aimed at binary outcomes. <br>
2. **Data Understanding & Preprocessing** <br>
Handles the conversion of string data to numeric format (Float64) to allow for mathematical modeling. <br>
3.**Exploratory Data Analysis (EDA)** <br>
Visualizes data patterns, showing that month-to-month contracts and high charges are significant churn indicators. <br>
4. **Baseline Model:** **Logistics Regression** <br>
The initial model used to set a performance benchmark, achieving approximately 80% accuracy. <br>
5. **Advanced Model:** **Random Forest** <br>
A robust ensemble model used to capture non-linear relationships and provide Feature Imortance insights. <br>


## Key Findings:
Logistic Regression performed best for overall accuracy.
Random Forest helped identify the most important features. <br>

## **Model Limitations** 
While the models achieve, there are key limitations to consider:

* **Class Imbalance:** The dataset contains significantly more "Non-Churners" (74%) than "Churners" (26%). This can cause the model to be baised toward predicting that a customer will stay.
* * **Feature Scope:** The data focuses on billing and contract types but lacks "Sentiment Data" (like customer service call logs or satisfaction surveys) which are strong predictors of churn.
  * **Static Snapshot:** This is a "Point-in-Time" analysis. it does not account for seasonla changes or new competitor offer that might happen after the was collected. <br>

  ## Business Justification & Recommendations <br>
  Based on the **"Feature Importance"** analysis, the following strategic actions are recommended: <br>
  1. **Contract Migration** Incentise customers on month-to-month plans to move to one-year or two-year contracts. <br>
  2. **Price Sentivity:** Offer loyalty discounts to high-paying customers who show early signs of churn (high monthly charges). <br>
  3. **Proactive Retention:** Use the 80% accuracy model to flag at-risk customers before they terminate their service. <br>

  ## Author
  * **Name:** Nwazue Maryben Ngozi
  * **Role:** Data Scientist
  * **Email:** nwazueblessing5@gmail.com
  * **Github Respository:** https://github.com/NwazueMaryben/TS_Academy_Capstone_Project
