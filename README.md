This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and superstition based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and checking some data features
    
2.	Assigning categories: this is semi-manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a manual time-consuming process but will generate higher precision the end
        
        Approval             | 181  | %7.65 
        Business             | 35   | %1.48 
        Health               | 71   | %3.00 
        Junk Knowledge       | 108  | %4.56 
        Other                | 66   | %2.79 
        Politics             | 88   | %3.72 
        Shipment             | 113  | %4.78 
        Unique vaccination   | 311  | %13.14 
        Vaccination campaign | 124  | %5.24 
        Vaccine              | 135  | %5.71 
        Side effects         | 70   | %2.96 

        Unclassified         | 1134 | %47.93 
    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
