# Fake-news-detection-Task-1
This repository implements a machine learning model using Python's scikit-learn library to detect fake news articles. It utilizes the Passive Aggressive Classifier algorithm and TF-IDF vectorization to analyze text data and classify news articles as real or fake.

Getting Started

Prerequisites:

Python 3.x
Required libraries: numpy, pandas, scikit-learn
Install them using pip install numpy pandas scikit-learn

Running the Script:

Clone or download this repository.
Open a terminal or command prompt and navigate to the repository directory.
Run the script using python main.py (assuming your script is named main.py).
Data

This project expects a CSV file named fake_or_real_news.csv containing the following columns:

Unnamed: 0: (Optional) An index column (can be ignored)
title: Title of the news article
text: Body text of the news article
label: Label indicating whether the news is fake or real (e.g., "FAKE" or "REAL")
Model and Approach

Data Loading and Preprocessing:

The script loads the CSV data using pandas.
Text data is cleaned by removing stop words (common words like "the", "a", etc.) using TF-IDF vectorization.
The data is split into training and testing sets for model evaluation.

TF-IDF Vectorization:

TF-IDF (Term Frequency-Inverse Document Frequency) is a technique for converting text data into numerical features.
It considers both the frequency of a word within a document (TF) and its rarity across the entire dataset (IDF).
This helps to identify words that are discriminative for classifying fake news.

Passive Aggressive Classifier:

The model uses a Passive Aggressive Classifier, a linear learning algorithm suitable for large datasets and online learning.
It iterates through the training data, updating the model parameters only when necessary to maintain correct classification.
Evaluation:

The model is trained on the training data and evaluated on the held-out testing set.
Accuracy score is calculated to measure the model's performance in correctly classifying real and fake news articles.
A confusion matrix is also generated to visualize the model's classification breakdown.

Expected Output:

The script will output the accuracy score of the model on the testing data. Additionally, the confusion matrix will be printed, providing insights into the model's performance on each class (real and fake news).
