🚗 Task 3 — Car Price Prediction with Machine Learning

AICTE Oasis Infobyte Internship (OIBSIP)

📌 Overview

This project is part of Task 3 under the AICTE Oasis Infobyte Internship Program.
The objective of this project is to build a Machine Learning model that predicts the selling price of a used car based on multiple factors.

Car price depends on various attributes such as:

Present price of the car

Fuel type

Transmission

Selling type (Dealer/Individual)

Car age

Owner history

Kilometers driven

Using these features, I trained a regression model that predicts the selling price of a car.

📂 Dataset Description

The dataset contains the following columns:

Column Name	Description
Car_Name	Name of the car
Year	Year of purchase
Selling_Price	Target variable (price in lakhs)
Present_Price	Current ex-showroom price
Driven_kms	Kilometers driven
Fuel_Type	Petrol / Diesel / CNG
Selling_type	Dealer / Individual
Transmission	Manual / Automatic
Owner	Number of previous owners
✔️ Target Variable:

Selling_Price

✔️ Features Used:

After feature engineering:

Present_Price

Driven_kms

Fuel_Type

Selling_type

Transmission

Owner

Car_Age (created from Year)

🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Google Colab

🧹 Data Preprocessing Performed

Loaded dataset into Pandas

Checked for missing values

Renamed and cleaned columns

Converted Year → Car_Age

Dropped irrelevant columns like Car_Name

One-Hot Encoded categorical features

Split dataset into training and testing sets

Feature engineering made the model more accurate by replacing raw year with actual car age.

🤖 Model Used

I used RandomForestRegressor, which is ideal for regression tasks due to:

Ability to handle non-linear relationships

Robustness to outliers

Higher prediction accuracy

Low overfitting compared to single decision trees

The complete model was built using a Scikit-Learn Pipeline combining:

Preprocessing (OneHotEncoding + numeric passthrough)

Random Forest Regressor

📊 Model Evaluation

The trained model was evaluated using:

MAE (Mean Absolute Error)

R² Score

These metrics help measure how close predicted values are to actual selling prices.

The model also includes a scatter plot comparing Actual vs Predicted Prices, which helps visualize prediction accuracy.

🔍 Prediction on New Car Data

The model can take inputs such as:

Present Price

Driven Kilometers

Fuel Type

Transmission

Owner Count

Car Age

Example output:

Predicted Selling Price (in lakhs): 4.67


This means the model correctly predicts a car’s selling price based on its attributes.

📈 Project Flow Summary

Import Libraries

Load Dataset

Clean & Analyze Data

Feature Engineering (Car_Age)

One-Hot Encode categorical features

Train-Test Split

Build Pipeline (Preprocessing + Model)

Train Random Forest Model

Evaluate performance

Predict new car price

Visualize results

📝 Conclusion

This Car Price Prediction project demonstrates how Machine Learning can be applied to real-world regression problems.

Key learnings include:

Feature engineering

Handling categorical/numerical data

Building ML pipelines

Using Random Forest for regression

Model evaluation

Making predictions on new data

This task strengthened my understanding of regression algorithms and practical ML workflows.

📁 Files Included

Car_Price_Prediction.ipynb — Google Colab notebook

README.md — Project documentation

🙌 Submitted Under

AICTE x Oasis Infobyte Internship Program (OIBSIP)
Task 3 — Car Price Prediction with Machine Learning
