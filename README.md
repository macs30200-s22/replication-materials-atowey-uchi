# Public Perception of Misinformation on Twitter
## A Temporal Analysis of Sentiment Towards Ivermectin, 2021

Allison M. Towey

The University of Chicago, Masters in Computational Social Science

Advised by: Professor Sabrina Nardin

June 3, 2022

The code and data in this repository are for Allison Towey's Perspectives on Computational Research Project.

In the summer of 2021, debate over the efficacy and safety of using ivermectin as a treatment for or preventative tool against COVID-19 became a polarized topic of discussion, with some media personalities and US health officials disagreeing about its effectiveness and safety. Discussion about the drug and its use spread to online social media, with a significant increase in keyword mentions about the drug peaking in late August 2021. There is a lack of literature about the effect of this debate on the opinions and acceptance of the drug by the general public. 

This paper seeks to understand the role of the media and government in shaping public perception of health information as witnessed on social media. To do so, we study whether four events, 1) Brian Kilmeade discussing the drug on the nightly Fox News program “Tucker Carlson Tonight”, 2) the FDA tweeting their disapproval for its use, 3) Seth Meyers’ “Late Night” segment about ivermectin, and 4) Podcaster and media personality Joe Rogan claiming he used the drug to heal from the illness, led to significant changes in positive and negative sentiment about ivermectin. This paper looks at changes in public sentiment as seen on Twitter over the months of August and September 2021 to study how concrete, polarizing events in the media shape public discourse about critical public health information.

In the course of the study, we find that though the amount of discussion about ivermectin on Twitter did significantly increase during the time period studied, the percent of positive, negative, and neutral sentiment detected in these tweets remained volatile during the time period, with no significant linear trends over the course weeks following these high-profile events. This paper describes the study and methods, and makes several key suggestions for further topic-based analysis of this time period and the role of political media and health officials in discussing unproven medical health claims of public health importance.


*Please note that due to the size of the CSV file of tweets, the data cannot all be found on the repository link; you can contact the author to receive the list of tweet IDs scraped and rehydrate the tweets to complete the analysis. I include a small sampling of tweets collection in tweets.csv that demonstrate the type of information scraped.*


## Overview of materials in repository:
* tweet_scraping.ipynb: A Jupyter notebook containing code to scrape the tweets in the analysis.
* sentiment_analysis.ipynb: A Jupyter notebook containing code to analyze the data, including the sentiment analysis classification.
* requirements.txt: The necessary requirements to recreate code on another machine.
* data.csv: the numerical data (number of tweets per day) used in analysis in a CSV format.
* tweets.csv: a small sampling (around 4,000 tweets) showing the type of information scraped. For the full CSV of tweets, please contact the repository owner.



## How to Replicate Code

### Requirements:
The code is written in Python 3.9.7 and all of its dependencies can be installed by running the following in the terminal (with the requirements.txt file included in this repository):

```
pip install -r requirements.txt
```

### Scraping:

#### Run tweet_scraping.ipynb.
This Jupyter Notebook scrapes tweets mentioning "ivermectin" from August 3, 2021 to September 30, 2021. As a result, we scrape a total of 128,587 tweets during the time period. Important information included is the text (content) and the date of each tweet.


### Sentiment Analysis:

#### Run sentiment_analysis.ipynb
This Jupyter Notebook cleans the tweets and uses the TextBlob sentiment analyzer to create polarity scores for each tweet. Each day worth of tweets is then averaged into one resulting polarity score. Finally, the notebook plots these averages across the month, which leads to the finding below.

![image](https://user-images.githubusercontent.com/89881145/165219720-8a0a0472-34ec-477e-8d75-be7ce89c6432.png)

## Key Findings
The data.csv file contains the numerial data used for the analysis. This includes the standard deviation and summing information used in the research.

### Increased Twitter Discourse During Media Scrutiny

An increase in social media discussion about ivermectin correlated with the FDA tweet and remained high throughout the period of study

<img width="506" alt="Screen Shot 2022-06-06 at 12 10 13 AM" src="https://user-images.githubusercontent.com/89881145/172098613-585b3de5-082e-4e0a-914b-d9df44c4b5f6.png">

Figure 1: Number of Tweets each day from August 1 to September 30, 2021. The middle third, the section with the highest number of tweets, from August 20 to September 9 is shaded.


### High Variance in Positive and Negative Sentiment Throughout Studied Period

Sentiment in the tweets collected about ivermectin was largely volatile, with no clear linear pattern of note.

<img width="506" alt="Screen Shot 2022-06-06 at 12 09 15 AM" src="https://user-images.githubusercontent.com/89881145/172098519-74326f6c-4d22-42c7-b413-5005caf6e9e3.png">

Figure 2: Positive, neutral and negative sentiment as expressed by ‘ivermectin’ Tweets over the period of analysis. 


## Citation information
Towey, Allison. Sentiment Analysis of Tweets Mentioning "Ivermectin", (2022), GitHub repository, https://github.com/macs30200-s22/replication-materials-atowey-uchi/.
