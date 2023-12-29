# YouTube Comments Analysis using Bigdata

This GitHub repository contains a Python script for sentiment analysis on YouTube comments. The process involves fetching comments from a YouTube video using the YouTube Data API, preprocessing the comments by removing emojis, special characters, and other irrelevant elements, and performing sentiment analysis using PySpark.

## Key Components:

### YouTube Data API Integration:

Utilizes the Google API client library to interact with the YouTube Data API for fetching comments from a specific video using its unique video ID.

### Data Preprocessing:

Cleans the fetched comments by removing emojis, special characters, and unnecessary spaces using regular expressions.
Converts all comments to lowercase for uniformity.

### Data Storage:

Saves the preprocessed comments to a CSV file named 'youtube dynamic.csv' for further analysis.

### Sentiment Analysis with PySpark:

Implements sentiment analysis using PySpark, a fast and general-purpose cluster computing system.
Utilizes a logistic regression model trained on a labeled dataset for sentiment prediction.

###Training and Testing:

Reads a labeled dataset for training the sentiment analysis model.
Splits the dataset into training and testing sets (70-30 ratio).

### Feature Extraction:

Tokenizes comments into individual words and removes stop words.
Converts each token into a numerical feature using HashingTF.

### Model Training:

Trains a logistic regression model on the numeric features of the training dataset.

### Model Testing:

Tests the trained model on the testing dataset and evaluates its accuracy.

### Application on YouTube Comments:

Reads the preprocessed YouTube comments from 'youtube dynamic.csv.'
Applies the trained model to predict sentiment on the YouTube comments.

The code is designed for robust sentiment analysis on YouTube comments and provides a clear demonstration of data fetching, preprocessing, and machine learning-based sentiment analysis using PySpark. Feel free to clone the repository and adapt the code for your specific use case.
