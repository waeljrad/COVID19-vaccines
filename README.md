This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and junk knowledge based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and check some data features
    
2.	Assigning categories: this is manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a time-consuming process but will generate higher precision the end
        
        Approval                  | 225 | % 7.56 
        Business                  | 48  | % 1.61 
        Health                    | 117 | % 3.93 
        Junk Knowledge            | 212 | % 7.12 
        Other                     | 180 | % 6.04 
        Politics                  | 144 | % 4.84 
        Procurement and Logistics | 211 | % 7.09 
        Unique vaccination        | 699 | % 23.47 
        Vaccination campaign      | 360 | % 12.09 
        Vaccine                   | 352 | % 11.82 
        Side effects              | 134 | % 4.50 

        Unclassified              | 296 | % 9.94 

        DISCLAIMER: these classifications are the result of a manual effort whithout medical proper knowledge. Medical professionals may have a different opinion.

    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
