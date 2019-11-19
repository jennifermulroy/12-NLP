# Natural Language Processing Techniques on Bitcoin and Ethereum

In this assignment, fundamental natural language processing techniques were applied to the latest news articles featuring Bitcoin and Ethereum to better understand sentiment and factors involved with the coin prices.  A number of factors were analyzed including, sentiment, common words, phrases, organizations and entities mentioned in aticles. 

in the latest news articles featuring Bitcoin and Ethereum. As well as fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

from nltk.sentiment.vader import SentimentIntensityAnalyzer
analyzer = SentimentIntensityAnalyzer()
from nltk.corpus import reuters, stopwords

### News Headlines Sentiment

Read your api key environment variable
Create a newsapi client
Fetch the Bitcoin news articles
Create the Bitcoin sentiment scores DataFrame

Use the news api to pull the latest news articles for bitcoin and ethereum and create a DataFrame of sentiment scores for each coin. 

Use descriptive statistics to answer the following questions:
1. Which coin had the highest mean positive score?
2. Which coin had the highest negative score?
3. Which coin had the highest positive score?

Why is sentiment analysis so important?
Businesses today are heavily dependent on data. Majority of this data however, is unstructured text coming from sources like emails, chats, social media, surveys, articles, and documents. The micro-blogging content coming from Twitter and Facebook poses serious challenges, not only because of the amount of data involved, but also because of the kind of language used in them to express sentiments, i.e., short forms, memes and emoticons.

Advantages of using VADER
VADER has a lot of advantages over traditional methods of Sentiment Analysis, including:
It works exceedingly well on social media type text, yet readily generalizes to multiple domains
It doesn’t require any training data but is constructed from a generalizable, valence-based, human-curated gold standard sentiment lexicon
It is fast enough to be used online with streaming data, and
It does not severely suffer from a speed-performance tradeoff.

### Tokenizer

from nltk.tokenize import word_tokenize, sent_tokenize
from nltk.corpus import stopwords
from nltk.stem import WordNetLemmatizer, PorterStemmer
from string import punctuation
import re


### NGrams and Frequency Analysis

from collections import Counter
from nltk import ngrams

In this section you will look at the ngrams and word frequency for each coin. 

1. Use NLTK to produce the n-grams for N = 2. 
2. List the top 10 words for each coin. 


# Word Clouds

In this section, you will generate word clouds for each coin to summarize the news for each coin


# Named Entity Recognition

In this section, you will build a named entity recognition model for both coins and visualize the tags using SpaCy.

import spacy
from spacy import displacy

SpaCy is an open-source library for advanced Natural Language Processing in Python.

PERSON, NORP (nationalities, religious and political groups), FAC (buildings, airports etc.), ORG (organizations), GPE (countries, cities etc.), LOC (mountain ranges, water bodies etc.), PRODUCT (products), EVENT (event names), WORK_OF_ART (books, song titles), LAW (legal document titles), LANGUAGE (named languages), DATE, TIME, PERCENT, MONEY, QUANTITY, ORDINAL and CARDINAL

