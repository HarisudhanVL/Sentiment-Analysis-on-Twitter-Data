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

The sentiment of the tweet can be found using **polarity** and **subjectivity**. Polarity is float which lies in the range of [-1,1] where 1 means positive statement and -1 means a negative statement. Subjectivity quantifies the amount of personal opinion and factual information contained in the text. The polarity and subjective score for a tweet can be found using a python library named ***[textblob](https://textblob.readthedocs.io)***. When calculating a sentiment for a single word, TextBlob uses the “averaging” technique that is applied on values of polarity to compute a polarity score for a single word and hence similar operation applies to every single word and we get a combined polarity for longer texts.

The sentiment of the tweets were found using textblob which looks like,

![image](https://user-images.githubusercontent.com/68286374/178974121-9999c29d-2ad3-4eb9-99ad-0bf6fdcef335.png)

Reaction of people all in twitter was analyzed when Elon Musk Announces that he is going to buy the shares of Twitter. Most of the people around the world tweeted neutrally and positively.
![image](https://user-images.githubusercontent.com/68286374/178974669-b355100a-68ed-4893-a4f0-b703ea4a3624.png)













