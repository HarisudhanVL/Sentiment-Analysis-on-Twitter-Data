# Sentiment-Analysis-on-Twitter-Data

### PROBLEM STATEMENT

Sentiment analysis on tweets ‘ Elon Musk buys Twitter ’ extracted from Twitter.

### PROJECT ABSTRACT

The tweets extracted from Twitter were preprocessed and the sentiment i.e, positive, negative, and neutral of the tweet is found using polarity and subjectivity. The Dataframe is framed. The created data frame is stored in the MySql database. Then the data is retrieved from SQL database to build a ML model to predict the sentiment of a new tweet. The distributed computing framework i.e, pyspark is used for implementing with the support of python. The performance of the model is evaluated. And also the analysis is made on the tweets of ElonMusk taking over Twitter.

### EXTRACTING TWEETS FROM TWITTER

The tweets can be extracted from twitter using **TWITTER API**. The API can be generated and found from [Twitter developer](https://developer.twitter.com) site. The twitter API can be accessed using a python library called ***[Tweepy](https://docs.tweepy.org/en/stable/)***. The keys authentication takes place with help of the tweepy library. Then define the hastag that has to be searched for, in this project **TwitterTakeover**. The tweets associated with this hashtag are extracted from twitter.

The extracted tweets of hashtag **TwitterTakeover** looks like,

![image](https://user-images.githubusercontent.com/68286374/178969100-ace51c0a-e796-4c81-9f4e-9277846d3dbf.png)

### PREPROCESSING THE TWEETS

The extracted tweets generally has text, numbers, emojies, multiple spaces, hyperlinks, punctuation, etc... Inorder to remove the unwanted entities preprocessing is done. General text preprocessing includes,
1) Removal of punctuation.
2) Removal of multiple white spaces.
3) Conversion of text from upper case to lower case.
4) Removal of numbers.
5) Removal of hyperlinks.

The tweet before preprocessing,
![image](https://user-images.githubusercontent.com/68286374/178970388-e812b087-e464-468d-9f1b-949723fd0944.png)

The tweet after preprocessing,
![image](https://user-images.githubusercontent.com/68286374/178970597-7b10ccb9-b33c-4a4c-b92c-8093f14556f4.png)

After preprocessing store the tweets in a list.

### SENTIMENT OF TWEETS

In general the sentiment of a tweets is categorized into three,
1) POSITIVE
2) NEGATIVE
3) NEUTRAL

The sentiment of the tweet can be found using **polarity** and **subjectivity**. 











