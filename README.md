# Project 3: Reddit Classification

## Problem Statement

This project aims to train a classifier to predict which subreddit a given post’s title came from.


## Executive Summary

### Methodology:

Using Reddit’s API, post titles were collected from the subreddits r/WritingPrompts and r/ShowerThoughts and collected into a combined dataframe.

The dataframe was then split up into a training set, on which various classification models were trained, and a test set, on which the trained models were tested for accuracy.

In order to work with the text data, various pre-processing techniques, including tokenization, stemming, CountVectorizer and TfidfVectorizer, were employed.

Additionally, various hyperparameters of the classification models were tuned using both GridSeachCV and direct substitution.

### Contents:
- [01_Data_Acquisition](https://git.generalassemb.ly/kevincrystal/DSI-labs-and-projects/blob/master/projects/project_3/01_Data_Acquisition.ipynb)
- [02_NLP_CountVectorizer_and_Modeling](https://git.generalassemb.ly/kevincrystal/DSI-labs-and-projects/blob/master/projects/project_3/02_NLP_CountVectorizer_and_Modeling.ipynb)
- [03_NLP_Tfidf_and_Modeling](https://git.generalassemb.ly/kevincrystal/DSI-labs-and-projects/blob/master/projects/project_3/03_NLP_Tfidf_and_Modeling.ipynb)


## Conclusion

The best classifiers trained were:
- Logistic Regression (default parameters, on CountVectorized data) which had accuracy scores of 96.7% on the training data and 85.37% on the test data. This test score improved by 4 percentage points after the titles were stemmed.
- Support Vector Machine (tuned parameters: kernel = ‘linear’, C=0.1; on CountVectorized data) which had accuracy scores of 91.5% on the training data and 84.17% on the test data.
# Subreddit_Classification
