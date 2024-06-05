# TWITTER SENTIMENT ANALYSIS

## Aim
The project aims to classify the sentiment of tweets using Natural Language Processing (NLP) techniques. In simpler terms, the project aims to build a model that can tell you whether a tweet is expressing a positive, negative, neutral or irrelevant opinion.

## Dataset
The dataset for Twitter Sentiment Analysis contains 74682 records for training and 1000 records for testing or validation.

Features:

1. Tweet ID 
2. Entity
3. Sentiment (Positive, Negative, Neutral or Irrelevant)	
4. Tweet Content	


## Model
1. Text Preprocessing: Tweets undergo a series of transformations to prepare them for machine learning models. This includes:

  - Emoji Handling: Emojis can be converted to text representations (e.g., ":)" to "happy") or encoded numerically based on sentiment.
  - Punctuation Handling: Punctuation may be removed or converted to a standard representation (e.g., "?" to "question mark").
  - Stopword Removal: Common words with little meaning (e.g., "the", "a") are removed to focus on sentiment-bearing words.
  - Stemming: Words are reduced to their base form (e.g., "running" to "run") to capture variations and improve model performance.

2. Data Labeling: Tweets are manually assigned sentiment labels according to a predefined scheme:

  - Positive (1): Expresses a positive sentiment or opinion.
  - Negative (0): Expresses a negative sentiment or opinion.
  - Neutral (2): Does not express a clear positive or negative sentiment.
  - Irrelevant (3): Not related to the sentiment analysis task (e.g., retweets, advertisements).

3. Machine Learning Pipelines: Two pipelines are created to explore different feature extraction and classification techniques:

     Pipeline 1 (TF-IDF Vectorizer + Random Forest):
    - TF-IDF Vectorizer: This vectorizer captures the importance of words relative to the entire corpus, potentially highlighting sentiment-specific terms.
    - Random Forest: This ensemble method combines multiple decision trees, offering robustness and good performance on text classification tasks.

     Pipeline 2 (CountVectorizer + Logistic Regression):
    - CountVectorizer: This vectorizer represents text as word counts, providing a simpler feature representation.
    - Logistic Regression: This linear model offers interpretability and can be effective for sentiment classification.
