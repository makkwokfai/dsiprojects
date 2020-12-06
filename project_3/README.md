# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & Classification

### Description

- To utilize the Reddit API to scape posts automatically from 2 Subreddits.
- To create and compare different classification models. The models predict which Subreddit a specific post came from.

### Data Collection

- The posts are scaped using the Reddit API.
- The posts are scaped from 2 subreddits i.e. Computing & Data Science - with 24.1k & 341k members respectively.
- These subreddits were created in 2011 & 2009, with 8,600+ & 45,000+ submissions respectively.
- The Reddit API extracts the posts in JSON format and the posts are stored as JSON files for further analysis.

### Data Cleaning

We have done data cleaning to the comments: 
- Duplicate message and null messages were dropped.
- Remove HTML and non-letters.
- Convert words to lower letters.
- List the stopwords and remove them.
- Combine "Selftext" & "Title" columns, and make them into a "New" column.

### Vectorizer & Modeling

Vectorizer from scikit-learn were used to convert the text data to numeric features. 2 different classifier - Naive Bayes & Logistic Regression were used to check which classifier give a better prediction on unseen datas.

### Conclusion & Recommendation

Vectorizer and Naive Bayes classifier achieved the best accuracy scores (train / test scores: 0.979 / 0.914).

Potential improvements for future: collect more training data, do more data cleaning and preprocessing (remove more stop words i.e. numbers, stem/lemmatize i.e. -ing verbs), more intensive gridsearching to optimize models, include n-gram parameter in gridsearch, try more models.