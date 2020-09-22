# Sentiment-Analysis-using-Naive-Bayes
A Naive Bayes model that analyses the sentiments of the tweets: Positive Sentiment or Negative Sentiment.

The model is trained on 4500 positive sentiment tweets and 4500 negative sentiment tweets. The tweets are preprocessed before the actual task begins. Preprocessing includes removing all the stopwords(words like I, am, the, etc which do not really have a significance on the sentence sentiment), removing hashtags, hyperlinks followed by case conversion. Once this is complete, the tweets are tokenized. The last step of preprocessing is stemming which means converting every word to its root form as in learning and learned will both be converted to learn.
Here the pre-processing is over.

The frequency of each word when occurring in a Positive Sentence and a Negative Sentence is counted and stored individually. Using this we calculate how much impact each word has on the Positivity or Negativity of the sentence.

When a new statement is encountered, the log probability of each word is added. Log probability of a word is the log of a fraction which is the number of times the word has appeared in a positive sentence to the number of times it has appeared in a negative sentence: log probability = log(n (+ve)/n(-ve)).
This value is calculated for all the words in the sentence and added together. If the final value is > 0, the sentence has a Positive Sentiment, and Negative Sentiment otherwise.
