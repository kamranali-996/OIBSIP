📧 Task 4 — Email/SMS Spam Detection Using Machine Learning

AICTE Oasis Infobyte Internship (OIBSIP)

📌 Overview

This project is part of Task 4 under the AICTE Oasis Infobyte Internship Program.
The objective of this task is to build a Machine Learning model that detects spam emails/SMS messages.

Spam detection is an essential application of Natural Language Processing (NLP).
This project classifies messages into:

Spam (unwanted, phishing, promotional, scam)

Ham (normal/legitimate messages)

Using Python and Machine Learning, the model learns from labeled text messages and predicts whether a new message is spam or not.

📂 Dataset Description

The dataset contains two main columns:

Column	Description
label / status	Message category (spam / ham)
message	The email/SMS text content

Dataset provided by Oasis Infobyte.

There are no missing values.
The dataset is imbalanced, with more ham messages than spam.

🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

Google Colab

🧹 Data Preprocessing

Loaded dataset with correct encoding (latin-1)

Removed unnecessary columns

Renamed columns (optional: label → status)

Checked for null values

Added optional message length analysis for EDA

📊 Exploratory Data Analysis

Performed visual and statistical analysis:

✔️ Label Distribution

Count of spam vs ham messages.

✔️ Message Length Analysis

Compared average message length for spam & ham messages.
Visualized using:

Histogram

KDE distribution

🤖 Model Building
1. Train-Test Split
X = df['message']
y = df['label'] or df['status']


Used an 80-20 split with stratification.

2. TF-IDF Vectorization

Converted raw text into numerical features using:

TfidfVectorizer(stop_words='english', max_df=0.9, min_df=5)

3. Classifier Used

Logistic Regression
(max_iter = 1000)

This model works well for binary classification in NLP tasks.

4. ML Pipeline

Combined vectorizer + model using:

Pipeline()


This ensures clean and efficient training.

📈 Model Evaluation

Evaluated the model using:

Accuracy Score

Precision, Recall, F1-score (classification report)

Confusion Matrix (visualized using heatmap)

The model achieved high accuracy, showing strong performance in identifying spam messages.

🧪 Custom Message Testing

Tested the model on real-world examples:

Phishing-style spam messages

Normal messages

Output correctly classifies messages as:

spam / ham

📝 Conclusion

This project demonstrates how NLP and Machine Learning can be used to detect spam messages effectively.

Key achievements:

Preprocessed textual data

Converted text into TF-IDF vectors

Trained a Logistic Regression model

Achieved strong evaluation scores

Built a complete pipeline

Successfully predicted new spam messages

This task strengthened my knowledge of:

Text preprocessing

Vectorization

Binary classification

Evaluation metrics

NLP-based machine learning pipelines

📁 Files Included

Email_Spam_Detection.ipynb — Full Colab notebook

README.md — Project documentation

🙌 Submitted Under

AICTE x Oasis Infobyte Internship Program (OIBSIP)
Task 4 — Email Spam Detection Using Machine Learning
