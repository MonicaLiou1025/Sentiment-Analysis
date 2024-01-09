# Sentiment-Analysis-On-Reddit

![image](https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/03c9c743-459f-4da1-bb3b-4f8b60de6706)

## Project Overview
Am I the asshole? People often post their story in the AITA community to 
Ever since I heard of it, I’ve wanted to explore a dataset of Reddit posts from a well known subreddit called “Am I the Asshole?” (AITA), in which users post stories of conflicts in which they weren’t sure if they did the right thing or were instead the, um, asshole. Other users comment and vote with their judgment: You’re the Asshole (YTA), Not the Asshole (NTA), Everyone Sucks Here (ESH), No Assholes Here (NAH), or Not Enough Info (INFO).

## Scrapping
We uses PRAW (Python Reddit API Wrapper) to interact with Reddit. The script collects posts from various categories (controversial, hot, new, rising, top of all time, top of the year...) and saves them into different CSV files.

<div align="center">
  <img width="605" alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/3c855f37-1d32-4a2a-9011-87d2c4f52959">
</div>

## Word Frequency
We use Word Tokenization and Part-of-Speech Tagging to find out the main characters or nouns. As you see in the below, the results are all about people and mostly showed pairs: For example, we got husband and wife here, sister and brother, daughter and son, girlfriend and boyfriend. But, hold on a second. We've got 'mom' on the list, but where's 'dad'? It seems like dads are often overlooked or not mentioned as much in the AITA tales, or perhaps, the less problematic ones in the AITA community. That's our little aha moment! So Good job, dad!

![output](https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/88dd92c2-e303-4f37-abd4-521e24fbda67)
