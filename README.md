# Sentiment-Analysis-using-Naive-Bayes
A Naive Bayes model that analyses the sentiments of the tweets: Positive Sentiment or Negative Sentiment

The model is trained on 4500 positive sentiment tweets and 4500 negative sentiment tweets.
The tweets are preprocessed before the actual task begins. Preprocessing includes removing all the stopwords(words like I,am,the which do not really have a significance on the sentence sentiment), hastags,hyperlinks ,case conversion.
Once this is complete, the tweets are tokenized.
The last step of preprocessing is stemming which means converting every word to it's root form as in learning and learnt will both be converted to learn.

The frequency of each word when occuring in a Positive Sentence and a Negative Sentence is counted and stored individually.
Using this we calculate how much impact each word has on the Positivity or Negativity of the sentence.
