# Yelp_Review___Text_Mining_Project
## Data Description: 
The dataset of this project is collected by Yelp engineers at 2017 and it contains more than 115 million reviews in total. There are five json files in the dataset, including the files of business, user, check-in, tip and review. In our project, we mainly focus on the review file. 

In the review file, there are 10 columns in total, which include review id, user id, business id, stars, date, useful, funny, cool, text and type. The three id columns contain unique id for each review, user and business. The stars column refers to the stars rating that customers labeled at Yelp, which ranges from 1 to 5. The date column refers to the date that customers wrote their review, which ranges from 2004 to 2017. The funny, cool and useful columns are customers’ label towards other customers'’ reviews or tips. The text column is the review that we are going to mainly focus on. The type column in the review file has only one value, which is review. 

## Project Objectives: 
This project is aiming at two main objectives achieved by topic modeling and sentiment analysis. 

-	Trend analysis: 
We would like to investigate the customers’ preference change in Yelp reviews over time by analyzing groups of top keywords in topics using LDA topic modeling. We divide the sample dataset into 3 time ranges from 2004 to 2017 and using unsupervised training to assign topics to groups of words. We plan to distinguish most popular topics in certain period and make recommendations both for Yelp and merchants to help them better understand and attract customers. Here is a potential outcome, 5 years ago, people write reviews revealing food and service of the restaurant, 5 years later, they may pay more attention to the decoration and environment. 

-	Sentiment Analyzer Training: 
We applied VADER Lexicon-Based Sentiment Analysis as unsupervised learning approach and Naive Bayes Classifier-Based Sentiment Analysis as supervised learning approach to train the analyzers and select the one with highest accuracy rate. Our objective is to use the most powerful model to predict other unlabeled reviews on other platforms for merchants. For example, some restaurants may have their own accounts on Facebook, they can receive many comments and reviews on that platform but have no idea what the attitude in reviews is without label. In this case, our model will be extremely useful in helping them interpret, understand and even build a closer relationship with customers. We believe our model can be a bridge between customers and merchants. 

## Conclusion:  
1. Recommendations  
- Restaurants should care more about the quality and the variety of food. Instead of only  having certain types of foods like American style, they should also pay attention to  decoration, service and environment of restaurants. 
- Hotels need to shift their attention from cost-efficient to high quality, which contains  convenience, good serving, parking, reservations and comfort. In recent years, hotels may  attract customers furthermore if they could provide facilities related with entertainment like  clubs or casinos.  
- After trying on several sentiment analysis. We found out that by using Naive Bayes  Classifier-Based Sentiment Analysis to train the model, we would get a higher accuracy. By  taking use of this method, restaurants can train their own model to predict reviews on social  media. The polarity they get is relatively precise. 

2. Possible shortcomings and ways to overcome them  
- For Naive Bayes Classifier-Based Sentiment Analysis, since it’s highly computationally  intensive, we were not able to train a large dataset. So the result at the first time is not very  accurate. Next time, if we still want to use the supervised learning techniques, we should get  a big-ram computer and train a bigger dataset.  
- Since we would like to apply our trained model based on Yelp to other platform like  Facebook, there can be selection bias. The reason is people who write reviews on Yelp may  not the same kind of customers on Facebook and their wording could be different. One  possible way to deal with this is to add labeled reviews on other platform into train dataset.  The model trained in this way could deliver a higher accuracy.  
