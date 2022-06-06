# Public Perception of Misinformation on Twitter
## A Temporal Analysis of Sentiment Towards Ivermectin, 2021

Allison M. Towey
The University of Chicago, Masters in Computational Social Science
Advised by: Professor Sabrina Nardin
June 3, 2022

The code and data in this repository are for Allison Towey's Perspectives on Computational Research Project.

Please note that due to the size of the CSV file of tweets, the data cannot all be found on the repository link; you can contact the author to receive the list of tweet IDs scraped and rehydrate the tweets to complete the analysis.


## Requirements:

## Scraping:
### Run tweet_scraping.ipynb.
This Jupyter Notebook scrapes tweets mentioning "ivermectin" from August 3, 2021 to September 30, 2021.

The resulting data placed in tweets.csv

*Note, due to some unexpecting bugs in the Twint API, there are only around 4,300 tweets scraped. Further investigation is needed to understand why such a small number of tweets were found.

## Sentiment Analysis:
### Run sentiment_analysis.ipynb
This Jupyter Notebook cleans the tweets and uses TextBlob sentiment analyzer to create polarity scores for each tweet. Each day worth of tweets is then averaged into one resulting polarity score. Finally, the notebook plots these averages across the month, which leads to the finding below.

![image](https://user-images.githubusercontent.com/89881145/165219720-8a0a0472-34ec-477e-8d75-be7ce89c6432.png)

## Preliminary Findings
While there is a significant amount of variation, there appears to be sharp dip around August 23, 2021 in sentiment. This is relevant to my research, as it is two days following the CDC's tweet informing US citizens not to use ivermectin.
https://twitter.com/US_FDA/status/1429050070243192839?s=20&t=fHNQHn8OFKigT775wYA1ag

## Citation information
Towey, Allison. Sentiment Analysis of Tweets Mentioning "Ivermectin", (2022), GitHub repository, https://github.com/macs30200-s22/replication-materials-atowey-uchi/.
