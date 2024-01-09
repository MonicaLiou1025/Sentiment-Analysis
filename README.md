# Sentiment-Analysis-On-Reddit

![image](https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/03c9c743-459f-4da1-bb3b-4f8b60de6706)

## Project Overview
Am I the asshole? People often post their story in the AITA community to 
Ever since I heard of it, I’ve wanted to explore a dataset of Reddit posts from a well known subreddit called “Am I the Asshole?” (AITA), in which users post stories of conflicts in which they weren’t sure if they did the right thing or were instead the, um, asshole. Other users comment and vote with their judgment: You’re the Asshole (YTA), Not the Asshole (NTA), Everyone Sucks Here (ESH), No Assholes Here (NAH), or Not Enough Info (INFO).

## Scrapping
We uses PRAW (Python Reddit API Wrapper) to interact with Reddit. The script collects posts from various categories (controversial, hot, new, rising, top of all time, top of the year, top of the month) and saves them into different CSV files. Here's a breakdown of its functionality:
