# Sentiment Analysis of Ivermectin Tweets (August 2021)
The code and data in this repository are for Allison Towey's Perspectives on Computational Ressearch project.

The code is written in Python 3.9.7. The following packages are required to run the code:
#### Utilities
import re
import numpy as np
import pandas as pd
#### Scraping
import twint
import nest_asyncio
#### Plotting
import seaborn as sns
from wordcloud import WordCloud
import matplotlib.pyplot as plt
#### nltk and sentiment analysis
from nltk.stem import WordNetLemmatizer
import nltk
from textblob import TextBlob

## Scraping:
### Run tweet_scraping.ipynb.
This Jupyter Notebook scrapes tweets mentioning "ivermectin" from August 3, 2021 to September 30, 2021.

The resulting data placed in tweets.csv

*Note, due to some unexpecting bugs in the Twint API, there are only around 4,300 tweets scraped. Further investigation is needed to understand why such a small number of tweets were found.

## Sentiment Analysis:
### Run sentiment_analysis.ipynb
This Jupyter Notebook cleans the tweets and uses TextBlob sentiment analyzer to create polarity scores for each tweet. Each day worth of tweets is then averaged into one resulting polarity score. Finally, the notebook plots these averages across the month, which leads to the finding below.

![image](https://user-images.githubusercontent.com/89881145/165219720-8a0a0472-34ec-477e-8d75-be7ce89c6432.png)
