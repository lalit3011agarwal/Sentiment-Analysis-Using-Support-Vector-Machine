# Sentiment Analysis Using Support Vector Machine

## Dataset Exploration
- Two datasets were used in this project, both obtained from [Kaggle](https://www.kaggle.com/):
  1. IMDb dataset: Contains over 50,000 movie reviews with ratings.
  2. Twitter sentiment analysis dataset: Contains over 190,000 tweets labeled as positive, negative, or neutral.
- The IMDb dataset was pre-processed to include only movies with a minimum of 1000 user ratings and to remove duplicates or missing values.
- The Twitter dataset contains tweets from various topics and hashtags, collected over several months.

## Preprocessing
Below are the preprocessing steps performed on the datasets:
- Removal of punctuation and numbers
- Conversion to lowercase
- Removal of stop words
- Two experiments were conducted:
  1. Stemming vs Lemmatization (on IMDb dataset)
  2. Inclusion vs Exclusion of Neutral Sentiment (on Twitter dataset)

## Model Architecture
- Employed Support Vector Machine (SVM) with LinearSVC
- Model was trained and tested on both datasets

## Performance Metrics
- Precision
- Recall
- F1-score
- Support
- Accuracy

## Experimental Results

### Experiment 1: Stemming vs Lemmatization (IMDb)
- Both techniques achieved 86% accuracy
- Comparable precision, recall, and F1-scores for both positive and negative sentiments

### Experiment 2: Neutral Sentiment (Twitter)
- With neutral sentiment: 89% accuracy
- Without neutral sentiment: 90% accuracy
- Including neutral sentiment improved classification of neutral tweets
- Excluding neutral sentiment improved classification of positive and negative tweets

## Challenges and Limitations
- Choice between stemming and lemmatization depends on specific dataset and problem
- Including or excluding neutral sentiment affects model performance differently

## Conclusion
- Both stemming and lemmatization are effective preprocessing techniques for sentiment analysis
- The decision to include or exclude neutral sentiment should be based on the specific goals of the analysis
- Careful experimentation and analysis are crucial when selecting preprocessing techniques and deciding on sentiment categories

## Future Directions
- Explore other machine learning algorithms for sentiment analysis
- Investigate the impact of different preprocessing techniques on model performance
- Analyze the effect of dataset size and quality on sentiment analysis accuracy
- Explore domain-specific sentiment analysis and its challenges
