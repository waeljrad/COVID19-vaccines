This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and superstition based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and checking some data features
    
2.	Assigning categories: this is semi-manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a manual time-consuming process but will generate higher precision the end
        
        Approval	1.48%
        Business	1.10%
        Health	1.56%
        Mass vaccination	0.17%
        Other	1.01%
        Politics	1.44%
        Shipment	3.80%
        Single vaccination	0.89%
        Superstition	1.48%
        Vaccination campaign	0.97%
        Vaccine	1.35%
        Unclassified	84.74%

3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
