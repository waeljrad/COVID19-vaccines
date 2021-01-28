This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and junk knowledge based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and check some data features
    
2.	Assigning categories: this is manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a time-consuming process but will generate higher precision the end
        
        Approval                   | 185 | % 6.21 
        Business                   | 47  | % 1.58 
        Health                     | 97  | % 3.26 
        Junk Knowledge             | 154 | % 5.17 
        Other                      | 128 | % 4.30 
        Politics                   | 111 | % 3.73 
        Procurement and Logistics  | 189 | % 6.35 
        Unique vaccination         | 574 | % 19.27 
        Vaccination campaign       | 265 | % 8.90 
        Vaccine                    | 236 | % 7.92 
        Side effects               | 99  | % 3.32 

        Unclassified               | 893 | % 29.99 

    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
