This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and superstition based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and checking some data features
    
2.	Assigning categories: this is semi-manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a manual time-consuming process but will generate higher precision the end
        
    Approval                  | 190 | %6.38 
    Business                  | 41  | %1.38 
    Health                    | 86  | %2.89 
    Junk Knowledge            | 135 | %4.53 
    Other                     | 94  | %3.16 
    Politics                  | 101 | %3.39 
    Procurement and Logistics | 173 | %5.81 
    Unique vaccination        | 495 | %16.62 
    Vaccination campaign      | 193 | %6.48 
    Vaccine                   | 189 | %6.35 
    Side effects              | 90  | %3.02 

    Unclassified              | 1191 | %39.99 
    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
