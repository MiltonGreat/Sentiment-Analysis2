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

### Features and Techniques

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

4. Model Deployment
- Saved the trained model and vectorizer using pickle for future use.

### Visualizations
- Sentiment Distribution: Visualized the count of posts across different sentiment categories.
- Sentiment Trends Over Time: Line plots showing how sentiment varies with time.
- Hashtag WordCloud: A word cloud representing the most frequently used hashtags.

### Results

- The sentiment classification model achieved balanced performance on multiple classes, leveraging simplified sentiment categories.
- The model provides actionable insights into customer sentiment trends, enabling brands to better understand their audience.

### Key Insights

- Sentiment analysis provides valuable insights into customer behavior and brand perception.
- Simplified sentiment categories enable actionable insights, especially when dealing with complex datasets.
- Visualizations like word clouds and time-series plots help uncover trends and patterns in customer sentiment.

### Future Work

- Improve label diversity by balancing underrepresented classes in the dataset.
- Explore advanced NLP techniques like BERT or Transformers for better sentiment classification.
- Implement a dashboard for real-time sentiment analysis and trend tracking.
- Integrate additional features like user engagement metrics for enhanced predictions.

### Source

https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset?resource=download
