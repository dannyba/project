Aanlysis of Twitter Messages related to drugs:
Data from Twitter API and Drugs.com was analysed using NLP techniques
 
Motivation:
Tweets (twitter messages) sometimes express opinions about different topics. 
I propose to build an automatic sentiment (positive or negative) extractor from a tweet related to prescription and Over The Counter (OTC) drugs. 
Using this analyzer:
      See which drugs are more tweeted
      See which drugs have more positive tweets and which less
      Which Tweets have url in their message (and thus trying to sell the drug online)
      Location of users that tweet about drugs

Sentiment classifiers Analysis:
An essential part is to have a comprehensive dataset or corpus to learn from, as well as a test dataset to ensure that the accuracy of the algorithm meets the expected standards. 
I used a corpus of already classified tweets. This database is based on data from the following sources:
    University of Michigan sentiment analysis competition on Kaggle.
    Twitter Sentiment Corpus by Niek Sanders.

The dataset contains 1,578,627 classified tweets, each row is marked as 1 for positive sentiment and 0 for negative sentiment. 
I diluted (took 1/10 randomly) the dataset to get a more diverse set of Tweets. I trained a Naive Bayes Classifier model. 

Creating Python script for Twitter search:
I used Twitter API to search for ~1000 different drugs. 
The search results as JSON, and uploaded into a Python Panda DataFrame.
