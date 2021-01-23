This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and superstition based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and checking some data features
    
2.	Assigning categories: this is semi-manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a manual time-consuming process but will generate higher precision the end
        
        Approval             |  51   | %2.16 
        Business             |  29   | %1.23 
        Health               |  81   | %3.42 
        Junk Knowledge       |  76   | %3.21 
        Other                |  48   | %2.03 
        Politics             |  52   | %2.20 
        Shipment             |  103  | %4.35 
        Unique vaccination   |  90   | %3.80 
        Vaccination campaign |  74   | %3.13 
        Vaccine              |  108  | %4.56 
    
        Unclassified         | 1.654 | %69.91 
    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
