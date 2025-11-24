📈 Task 5 — Sales Prediction using Python

AICTE Oasis Infobyte Internship (OIBSIP)

📌 Overview

This project is part of Task 5 under the AICTE Oasis Infobyte Internship Program.
The objective of this task is to build a Machine Learning model that predicts product sales based on advertising spending on different media channels.

Businesses frequently use sales prediction models to:

Decide where to invest their advertising budget

Understand the impact of marketing channels

Forecast future sales based on promotional activities

Using Python and Linear Regression, this project predicts sales using advertising expenditure on:

TV

Radio

Newspaper

📂 Dataset Description

The dataset used in this project is Advertising.csv, containing the following columns:

Column Name	Description
TV	Cost spent on TV advertising
Radio	Cost spent on Radio advertising
Newspaper	Cost spent on Newspaper advertising
Sales	Product sales (target variable)

The dataset initially contains an extra column (Unnamed: 0), which has been removed during preprocessing.

🛠️ Technologies Used

Python

Pandas

NumPy

Seaborn

Matplotlib

Scikit-Learn

Google Colab

🧹 Data Preprocessing

Loaded the dataset from Advertising.csv

Dropped unnecessary index column (Unnamed: 0)

Checked for missing values (none present)

Performed statistical analysis and summary

Identified correlations between features and target

📊 Exploratory Data Analysis (EDA)

EDA was performed using:

✔️ Pairplot

To observe relationships between all numerical features.

✔️ Correlation Heatmap

To understand how strongly each advertising medium influences sales.

Insights:

TV advertising has the highest impact on Sales

Radio also contributes positively

Newspaper has the weakest relationship with Sales

🤖 Model Used
Multiple Linear Regression

Why Linear Regression?

Simple and interpretable

Works well for continuous target variables

Effective when features show linear relationships with the target

Model workflow:

Selected features: TV, Radio, Newspaper

Target variable: Sales

Split data into training and testing sets (80/20)

Trained the model on the training data

Evaluated model performance on the testing data

📈 Model Evaluation

Evaluation metrics used:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score (Coefficient of Determination)

In this dataset, the model achieves a strong R² score (≈ 0.88 – 0.90), indicating good predictive accuracy.

Additionally, an Actual vs Predicted Sales scatter plot visually confirms strong alignment.

🔍 Feature Importance

The regression coefficients indicate the influence of each advertising channel:

TV has the highest impact

Radio has moderate influence

Newspaper has minimal effect

This aligns with real-world marketing insights.

🧪 Prediction on New Data

The model is capable of predicting future sales based on user-defined advertising budgets.

Example:

new_data = pd.DataFrame({
    'TV': [100],
    'Radio': [20],
    'Newspaper': [10]
})

prediction = model.predict(new_data)
print("Predicted Sales:", round(prediction[0], 2))

📝 Conclusion

This project demonstrates how Machine Learning can be used to:

Analyze advertising impact

Predict product sales

Assist businesses in making data-driven marketing decisions

Using the Advertising dataset and Linear Regression, the model successfully forecasts sales by understanding how advertising spending influences customer demand.

This task strengthened my understanding of regression modeling, feature importance, and data visualization.

📁 Files Included

Sales_Prediction.ipynb — Google Colab Notebook

README.md — Documentation for Task 5

Advertising.csv — Dataset used

🙌 Submitted Under

AICTE x Oasis Infobyte Internship Program (OIBSIP)
Task 5 — Sales Prediction Using Python
