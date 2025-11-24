🌼 Task 1 — Iris Flower Classification

AICTE Oasis Infobyte Internship (OIBSIP)

📌 Project Overview

This project is part of my AICTE Oasis Infobyte Internship – Task 1, where the objective is to build a machine learning model that can classify Iris flower species based on their physical measurements.

The Iris dataset contains measurements of:

Sepal Length

Sepal Width

Petal Length

Petal Width

The model predicts one of the three species:

Iris-setosa

Iris-versicolor

Iris-virginica

📂 Dataset Used

The dataset used in this project is the Iris.csv file provided in the internship resources.
It contains 150 rows and 6 columns:

Id

SepalLengthCm

SepalWidthCm

PetalLengthCm

PetalWidthCm

Species

The Id column was removed because it does not contribute to prediction.

🛠️ Technologies & Libraries

Python

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

📊 Steps Performed
1. Data Loading & Cleaning

Loaded Iris.csv into a pandas DataFrame

Checked shape, info, summary statistics

Dropped the unnecessary Id column

2. Exploratory Data Analysis (EDA)

Pairplot to visualize relationships between features

Correlation heatmap

Species distribution count

Boxplots (optional)

3. Data Preparation

Split dataset into Features (X) and Target (y)

Performed train-test split (80% training, 20% testing)

4. Model Building

Two algorithms were trained:

✔️ K-Nearest Neighbors (KNN)

n_neighbors = 3

Trained using X_train and y_train

✔️ Support Vector Machine (SVM)

Linear kernel

Performed exceptionally well

Achieved 100% accuracy on test data

5. Model Evaluation

Accuracy Score

Classification Report

Confusion Matrix Heatmap

6. Prediction on New Input

A new sample [5.0, 3.4, 1.5, 0.2] was given to the trained model, and the predicted species was Iris-setosa.

📈 Results
✔️ KNN Model Accuracy:

Varies depending on n_neighbors (typically between 95–100%)

✔️ SVM Model Accuracy:

1.0 (100% accuracy)

SVM performed best for this dataset because the classes are well-separated.

🤖 Conclusion

This project helped me understand the complete machine learning workflow:

Data loading

Cleaning

Visualization

Splitting

Training

Testing

Predicting

The Iris dataset is simple and balanced, making it ideal for learning classification.
Both KNN and SVM performed very well, with SVM achieving perfect accuracy.

🔗 Files Included

Iris_Flower_Classification.ipynb

📝 Credits

This project is submitted as Task 1 for the
AICTE Oasis Infobyte Internship (OIBSIP).
