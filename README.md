This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and junk knowledge based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and check some data features
    
2.	Assigning categories: this is manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a time-consuming process but will generate higher precision the end
        
        Approval                  | 207 | % 6.95 
        Business                  | 47  | % 1.58 
        Health                    | 108 | % 3.63 
        Junk Knowledge            | 194 | % 6.51 
        Other                     | 168 | % 5.64 
        Politics                  | 123 | % 4.13 
        Procurement and Logistics | 202 | % 6.78 
        Unique vaccination        | 619 | % 20.79 
        Vaccination campaign      | 312 | % 10.48 
        Vaccine                   | 287 | % 9.64 
        Side effects              | 117 | % 3.93 

        Unclassified              | 594 | %19.95 

        DISCLAIMER: these classifications are the result of a manual effort whithout medical proper knowledge. Medical professionals     may have a different opinion.

    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
