This project is still in progress

The data source is the following:
https://www.kaggle.com/gpreda/pfizer-vaccine-tweets

The countries has been normalised manually as a new feature.
The following columns have been added using code:
 - Country_freq
- text_length
- link

The 'text' column has been modfied to remove the link, now in a seperate column.

The next steps will be (1) normalising the hashtags (manually) (2) predict the main topic based on the hashtags based on NLP predictions.
