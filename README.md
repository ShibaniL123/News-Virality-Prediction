# News-Virality-Prediction

In this project , I have used Twitter API, Tweepy to extract tweets from Twitter handle of popular news websites.
I have considered Retweet count as a paramameter of virality.
Used the following attributes from tweepy object: retweet count, favourite count, full text, created date,mined date.
Extracted URL of news article from the tweet. Used Newspaper3k to scrape the article, extract information and summarize it.
Here I have used number of words in the article as a parameter to determine it's virality.
Performed Sentiment Analysis on Summary of article to find polarity of sentiment. Removed outliers to improve accuracy.
Used following parameters to train regression model: Word count, Polarity, Sentiment class(positive or negative), difference in minutes between tweet mining and tweet creation,favourite count.
This model is used to predict number of retweets.  Random Forest Regressor, Ridge Regressor,KNN Regressor,Bayesian regression and Decision tree have been implemented. Bayesian Regression gave the best accuracy of 70.2%
 	    
	  Algorithm                Accuracy
    random forest regressor  0.689495
   	Ridge Regressor          0.70042
    Knn                      0.515772
    Bayesian Regression 	   0.702854
    Decision Tree 	         0.384234

I've included visualizations of data,as well as heatmaps of correlation between parameters.
