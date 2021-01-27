This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

This data set from Kaggle contains tweets about COVID19 vaccines with lists of Hashtags. The goal of this project is classifying these tweets to distinguish health-oriented, political and junk knowledge based on NLP algorithms.

In order to achieve this, we follow three steps:

1.	Text processing and data preparation: in this step we format the data, delete GDPR related information, extract links from tweets and check some data features
    
2.	Assigning categories: this is manual process which plays a role in the prediction quality. We have to classify the tweets directly one-by-one, which is a time-consuming process but will generate higher precision the end
        
        Approval                  | 179  | %6.01 
        Business                  | 42   | %1.41 
        Health                    | 90   | %3.02 
        Junk Knowledge            | 140  | %4.70 
        Other                     | 95   | %3.19 
        Politics                  | 104  | %3.49 
        Procurement and Logistics | 174  | %5.84 
        Unique vaccination        | 512  | %17.19 
        Vaccination campaign      | 228  | %7.66 
        Vaccine                   | 194  | %6.51 
        Side effects              | 92   | %3.09 

        Unclassified              | 1128 | %37.88 
    
3.	Once categories are assigned, an NLP vectorizer is used to predict the tweets.

At the end we will have a classifier to predict whether the tweet has real informative value in regards to COVID19 and helps to eliminate all junk-science or any other irrelevant information.
