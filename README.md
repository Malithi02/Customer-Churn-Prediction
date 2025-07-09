# Customer-Churn-Prediction📌 Project Overview
A beginner-friendly machine learning project to predict customer churn using classification models based on usage data.

📌 Project Features
•	Exploratory Data Analysis (EDA)

•	Data cleaning and label encoding

•	Handling class imbalance using SMOTE

•	Model training using:

    o	Decision Tree

    o	Random Forest

    o	XGBoost

•	Evaluation metrics: Accuracy, Precision, Recall, F1-Score

•	Model saved using Pickle for reuse




📁 Files Included

•	Customer_Churn_Prediction_using_ML.ipynb – Main Jupyter Notebook

•	WA_Fn-UseC_-Telco-Customer-Churn.csv – Sample dataset

•	customer_churn_model.pkl – Trained Random Forest model

________________________________________


🚀 How to Use

1.	Clone this repo or download the files
2.	Open the .ipynb notebook in Google Colab or Jupyter Notebook
3.	Run all cells to retrain the model or load the saved one
4.	Use the trained model to make predictions on new customer data
________________________________________



🧪 Sample Prediction Code

import pickle

model = pickle.load(open("customer_churn_model.pkl", "rb"))
sample_input = [[1, 0, 1, 0, 5, 1, 0, 1, 0, 0, 1, 0, 0, 1, 1, 2, 1, 35.0, 180.5]]
prediction = model.predict(sample_input)

print("Will the customer churn?", "Yes" if prediction[0] == 1 else "No")


