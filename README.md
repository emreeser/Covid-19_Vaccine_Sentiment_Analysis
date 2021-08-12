# Covid-19 Vaccine Sentiment Analysis with Tweets

The development of information technology is increasing. The development of information technology is characterized by the emergence of increasingly social media such as Youtube, Facebook, Instagram, Line, Twitter and others. One of the most widely used social media is Twitter. Twitter is one of the social networking services where users can send and read text-based messages with a limit of 140 characters, known as tweets. Tweet data on Twitter can be a form of perception and opinion. The opinions posted on Twitter can contain many things, one of which is about Covid-19 pandemic. In this article we wanted to develop a model for opinions of people about covid -19 vaccines. 

##Proposed Method

In this project we used SVM classifier. Like Naive Bayes classifiers, support vector classifiers also work well for text classification and require relative few training examples. Support vector machine analyzes the data, define the decision boundaries and uses the kernels for computation which are performed in input space. The input data are two sets of vectors of size m each. Then every data which represented as a vector is classified into a class. Nextly we find a margin between the two classes that is far from any document. The distance defines the margin of the classifier, maximizing the margin reduces indecisive decisions. SVM also supports classification and regression which are useful for statistical learning theory and it also helps recognizing the factors precisely, that needs to be taken into account, to understand it successfully.
We used TF-IDF method for vectorization of words. A Term frequency (TF) is a simple measurement in the weighing method. This method, every term assumed to have a proportion of interests according to the number of occurrences (emergence) in the text (document). Term frequency can improve the recall value of retrieval information, but not always fix the precision value.  The Inverse document frequency, commonly abbreviated IDF, is a term for a more focused method of paying attention to the term occurrence of the whole text set. On IDF, a rare term that appears in the entire collection of text is judged to be more valuable. The value of each term interest is assumed inversely with the amount of text containing the term .

As shown in the figure 3 below we used a prepared tweet dataset from kaggle. First of all  we drop out columns except tweet_text and sentiment. We converted the tweet text to lower case and then we removed unnecessary tweet words such as username, retweets, hashtags, links, punctuations, digits etc.And then we fixed contractions. (e.g we converted “i’m”  to “i am” ) Then we removed stop words and single characters such as ‘i’ and ‘a’.  Because any of these don’t help us to identifying sentiment of tweet. After all of this we completed our cleaning stage. For testing our model we pulled tweet data from twitter and we drop out columns except tweet_text . We implemented cleaning process on this tweet data and we send this data to our model for prediction and we recieved realistic results.
