This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and junk knowledge based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and check some data features
    
2.	Assigning categories: this is manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a time-consuming process but will generate higher precision the end
        
        Approval                  | 230 | % 7.72 
        Business                  | 50  | % 1.68 
        Health                    | 127 | % 4.26 
        Junk Knowledge            | 224 | % 7.52 
        Other                     | 204 | % 6.85 
        Politics                  | 154 | % 5.17 
        Procurement and Logistics | 231 | % 7.76 
        Unique vaccination        | 780 | % 26.19 
        Vaccination campaign      | 418 | % 14.04 
        Vaccine                   | 400 | % 13.43 
        Side effects              | 160 | % 5.37 

        DISCLAIMER: these classifications are the result of a manual effort whithout medical proper knowledge. Medical professionals may have a different opinion.

    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
