This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

Objective:

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and superstition based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and checking some data features
    
2.	Assigning categories: this is semi-manual process which plays a role in the prediction quality. Categories are assigning via two ways:
 a. By extracting hashtags, classifying them one by one and set an algorithm to elect a category for each tweet based to the highest category occurrences
 b. However, hashtags appearing many times may incur errors for some outliers: in that case a hard-coded classification for the tweet overrides the tweet category
 Note: This classification effort is still in progress in step a.

3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets
At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
