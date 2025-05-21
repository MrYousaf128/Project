🐦 Twitter Sentiment Analysis using Machine Learning
This project applies machine learning techniques to perform sentiment analysis on Twitter data using the Sentiment140 dataset. The goal is to classify tweets as positive or negative based on their textual content.


📌 Project Objectives
Build a sentiment analysis model to classify tweets as Positive or Negative.

Use preprocessing techniques like tokenization, stemming, and TF-IDF.

Train and evaluate a Logistic Regression model.

Deploy the model using a simple Gradio web interface.



🗃 Dataset
Name: Sentiment140

Source: Kaggle

Size: 1.6 million labeled tweets


Labels:

0: Negative

4: Positive (replaced with 1 in this project for binary classification)

🧪 Technologies & Libraries
Language: Python


Libraries:

pandas, numpy, re

nltk for text preprocessing

scikit-learn for ML model and evaluation

gradio for model deployment


🔍 Methodology
1. Data Preprocessing
Assign column names: ['target', 'id', 'date', 'flag', 'user', 'text']

Replace label 4 with 1 for consistency (1 = Positive, 0 = Negative)

Remove special characters, lowercase text, and remove stop words

Apply Porter Stemming


2. Feature Extraction
Use TF-IDF Vectorizer to convert text into numerical features

Limit to top 1000 features for performance


3. Model Training
Split data (80% train, 20% test)

Train Logistic Regression model on TF-IDF vectors


4. Evaluation
Evaluate accuracy on training and test data

Use confusion matrix to analyze results

Achieved approximate distribution:

🟩 Positive Tweets: ~56.21%

🟥 Negative Tweets: ~43.79%


🖥 Deployment
Used Gradio to build an interactive web app

Allows real-time tweet sentiment prediction via browser input
