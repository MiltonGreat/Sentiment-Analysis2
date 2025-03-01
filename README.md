# Sentiment Analysis from Text Data

This project aims to automate sentiment classification from text data, such as social media interactions, customer reviews, and feedback, to help businesses gain insights into public opinion. By leveraging machine learning, we classify text into Positive, Neutral, and Negative sentiments, enabling companies to track customer emotions, identify trends, and improve engagement strategies.

### Objectives

- Gauge public sentiment towards a brand, product, or service.
- Identify trends in customer feedback, including recurring complaints or praise.
- Improve customer engagement by analyzing negative feedback and responding effectively.
- Visualize sentiment distribution over time to understand customer emotions.

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

### Project Workflow

1. Data Preprocessing
- Removing irrelevant columns (Unnamed: 0, duplicate index columns).
- Cleaning text data (lowercasing, removing stopwords, punctuation, and special characters).
- Tokenization & vectorization using TF-IDF or Word Embeddings.
- Balancing the dataset using SMOTE to handle class imbalances.

2. Modeling Approach
- Baseline Model: Logistic Regression
- Advanced Models: Random Forest
- Evaluation Metrics: Precision, Recall, F1-Score, and Accuracy.
- Confusion Matrix for analyzing misclassifications.

### Results

1. Sentiment Distribution:
- Positive: 279 occurrences
- Neutral: 251 occurrences
- Negative: 202 occurrences

2. Class Imbalance Handling:
- Original distribution: Class 2 (Positive) had the highest count, while Class 0 (Negative) was underrepresented.
- SMOTE was applied to balance the dataset before training.

3. Model Performance:
- Achieved an accuracy of 70% with Random Forest.
- Negative sentiments were classified with high precision, while Neutral sentiment posed challenges.

### Source

https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset?resource=download
