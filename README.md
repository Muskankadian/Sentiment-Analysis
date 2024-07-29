# Sentiment-Analysis

## Overview
This project performs sentiment analysis on text data using machine learning techniques. It aims to classify the sentiment of textual data into positive, negative, or neutral categories.

## Features
- **Preprocessing**: Includes text cleaning, tokenization, and vectorization.
- **Machine Learning Models**: Implements various models such as Support Vector Machines (SVM), Naive Bayes, and LSTM Neural Networks for sentiment classification.
- **Evaluation**: Metrics like accuracy, precision, recall, and F1-score are used to evaluate model performance.
- **Deployment**: Provides options for deployment, such as REST API using Flask or integration into a web application.

## Technologies Used
- Python
- Libraries: NLTK, Scikit-learn, pandas, numpy, seaborn, matplotlib

## Database Schema
Here's a brief description of each attribute:

- **ProductId**: A unique identifier for the product being reviewed. This attribute helps distinguish between different products in the dataset.
-UserId: A unique identifier for the user who wrote the review. Each user is identified by their UserId.

- **ProfileName**: The profile name or username of the user who wrote the review. This attribute may provide additional context about the reviewer.

- **HelpfulnessNumerator**: The number of users who found the review helpful. This can be used as a measure of the review's perceived usefulness.

- **HelpfulnessDenominator**: The total number of users who indicated whether they found the review helpful or not. This attribute, along with HelpfulnessNumerator, provides a ratio of helpfulness.

- **Score**: The rating or score given to the product in the review, typically ranging from 1 to 5. This represents the user's overall satisfaction with the product.

- **Time**: The timestamp or date/time when the review was posted. This attribute can be used for temporal analysis or to track review trends over time.

- **Summary**: A brief summary or headline of the review. This provides a concise overview of the main points or sentiment expressed in the review.

- **Text**: The full text of the review, providing detailed feedback, opinions, and experiences shared by the reviewer

## Setup
1. **Clone the repository:**

2. **Install dependencies:**

3. **Run the project:**

## Usage
-Step 0.  Read in Data and NLTK Basics

-Step 1.  VADER Sentiment Scoring : 
      We will use NLTK's SentimentIntensityAnalyzer to get the neg/neu/pos scores    
      of the text. This uses a "bag of words" approach:
      1) Stop words are removed
      2) each word is scored and combined to a total score.

-Step 2.  Roberta Pretrained Model
      1)Use a model trained of a large corpus of data.
      2)Transformer model accounts for the words but also the context related to      
          other words.

-Step 3.  Combine and compare

-Extra:  The Transformers Pipeline
     Quick & easy way to run sentiment predictions


## Contact
- If you have any questions, feel free to contact me at muskankadian02@gmail.com
