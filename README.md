# Social Media Sentiment Analysis

This project leverages Natural Language Processing (NLP) techniques to analyze customer feedback, reviews, and social media interactions to gauge public sentiment towards a brand. By processing and classifying user-generated content, the project provides insights into customer sentiment, helping businesses understand their audience better.

### Project Overview

The goal of this project is to analyze sentiment from social media posts and categorize it into meaningful sentiment classes such as Positive, Negative, Neutral, and Other. The analysis includes:

- Cleaning and preprocessing social media data.
- Simplifying complex sentiment labels into actionable categories.
- Building and evaluating machine learning models to classify sentiment.
- Exploring sentiment trends across time and hashtags.
- Visualizing sentiment insights using plots and word clouds.

### Dataset

The dataset, sentimentdataset.csv, contains user-generated content from various social media platforms. The dataset includes the following features:

- Text: Social media posts and reviews.
- Sentiment:	Original sentiment labels assigned to the posts.
- Timestamp:	Date and time when the post was created.
- Hashtags	Hashtags used in the post.
- Likes:	Number of likes the post received.
- Retweets:	Number of retweets/shares the post received.
- Platform:	Social media platform where the post originated.
- Country:	Country of origin for the post.
- Year, Month, Day, Hour:	Date components extracted from Timestamp.

The dataset consists of social media posts that have been labeled for sentiment as one of three categories:

- Positive
- Neutral
- Negative

### Problem Statement

Understanding customer sentiment about a brand is critical for product and marketing decisions. This project aimed to analyze customer reviews and social media posts to gauge public opinion and sentiment trends.

### Solution Approach

1. Data Preprocessing
- Text Cleaning: Removed URLs, mentions, hashtags, punctuation, and stopwords.
- Feature Engineering: Simplified sentiment labels into four categories (Positive, Negative, Neutral, Other) for easier analysis.

2. Exploratory Data Analysis
- Visualized the distribution of sentiment labels.
- Generated word clouds for hashtags to understand trending topics.
- Analyzed sentiment trends over time.

3. Machine Learning Model
- Used TF-IDF Vectorization to convert text into numerical features.
- Trained a Logistic Regression model and a Random Forest Classifier to classify sentiments.
- Classification report (Precision, Recall, F1-Score)
- Confusion matrix
- Cross-validation accuracy

### Results

After training the Logistic Regression model, the following results were obtained on the test set:

Classification Report:
- Negative: Precision = 0.85, Recall = 0.82, F1-Score = 0.83
- Neutral: Precision = 0.64, Recall = 0.54, F1-Score = 0.59
- Positive: Precision = 0.62, Recall = 0.75, F1-Score = 0.68

Accuracy: 0.70

Confusion Matrix: The confusion matrix has been visualized to show the model's predictions vs actual labels for each sentiment category.

Class Distribution Before and After SMOTE:
- Class distribution was highly imbalanced in the original training set:
    - Negative: 153 instances
    - Neutral: 201 instances
    - Positive: 231 instances

After applying SMOTE, the training data was balanced with an equal number of samples across all classes:
    - Negative: 231 instances
    - Neutral: 231 instances
    - Positive: 231 instances

### Future Work

1. Hyperparameter Tuning:
- Further tune the Logistic Regression model using grid search or random search for optimal hyperparameters.

2. Model Comparison:
- Try other machine learning models such as Random Forest, Support Vector Machine (SVM), or XGBoost and compare performance.

3. Further Text Preprocessing:
- Experiment with more advanced text preprocessing steps, such as using Word2Vec or BERT embeddings for feature extraction.

### Source

https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset?resource=download
