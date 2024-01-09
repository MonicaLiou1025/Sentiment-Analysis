# Sentiment Analysis on Reddit's "Am I the Asshole?" Subreddit

![image](https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/03c9c743-459f-4da1-bb3b-4f8b60de6706)

## Project Overview
"Am I the Asshole?" (AITA) is a popular subreddit where users share personal stories and seek judgment from the community. This project aims to analyze sentiments and patterns within these narratives to understand common trends and perceptions.

## Data Scrapping
Utilizing PRAW (Python Reddit API Wrapper), our script collects posts from different categories (e.g., controversial, hot, new, rising, top of all time, top of the year) and compiles them into various CSV files.

<img alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/3c855f37-1d32-4a2a-9011-87d2c4f52959">


## Word Frequency
Through Word Tokenization and Part-of-Speech Tagging, we identified commonly occurring characters and nouns. Interestingly, the data showed frequent pairings like 'husband' and 'wife', 'sister' and 'brother', etc. Our analysis uncovered a curious trend: while 'mom' is a frequent mention in AITA narratives, 'dad' is notably less mentioned. This observation serves as a subtle compliment to dads, highlighting their potentially less controversial or more harmonious role in the family scenarios shared on Reddit's AITA community.

![image](https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/18f1354e-57b7-4784-9b24-7b9e1fb0530a)


## Lift Value Analysis
This section examines attributes that sway a post towards being judged as 'Not the Asshole' (NTA) or 'Asshole' (YTA). Our findings suggest mentioning a 'wife' or 'girlfriend' in posts correlates with a higher likelihood of being labeled YTA, while references to 'husband' or 'boyfriend' are less likely to receive such judgments. Interestingly, 'mom' mentions also tend to avoid the YTA tag.

<img alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/e8f02890-0cab-49ff-83f4-22f500982974">

## Sentiment Analysis
Using the VADER (Valence Aware Dictionary and sEntiment Reasoner) tool, we scored texts on a scale from -1 (most negative) to +1 (most positive). The analysis reveals a significant lean towards non-neutral sentiments in AITA stories.

<img alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/736530d0-a33f-46c3-a097-930931976510">

## Modeling
For classification, posts tagged as 'Asshole' are labeled as 1, and 'Not The Asshole' are labeled as 0.
The results will give the judgment of whether a post is classified as "Am I the Asshole" or not and provide Probability Scores of the classification. The BERT model is more accurate by a margin of 10.75% compared to the Random Forest model. This suggests that for this particular task, BERT is better at understanding the context and nuances of the language used in AITA posts.
<img alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/c1b34547-be0b-47f0-bcc1-f741f154d484">


