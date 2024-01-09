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

![image](https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/18f1354e-57b7-4784-9b24-7b9e1fb0530a)


## Lift Value
What attributes make a post in Reddit's AITA community lean towards 'Not the A-hole' (NTA) or 'Asshole' (YTA)? In this chart, the 'Lift Percentage' for YTA is calculated by taking its YTA lift value and dividing it by the sum of the lift values for both NTA and YTA. Let’s see the result, if you mention wife, girlfriend in your AITA post topic, dude, you have a high percentage of being an asshole. I will send this report to my boyfriend, if he wants to judge me on AITA community, he is probably the one who is having issue. Also, if you mention your child and kids, you are probable an asshole as well. However, if you mention husband or boyfriend, it seems that you are not asshole at all. That make sense to me. So if I want to complain my bf in the AITA community, I have low percentage of being an asshole.  And if you mention ‘mom’, okay you are not asshole too! 

<img width="613" alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/e8f02890-0cab-49ff-83f4-22f500982974">

## Sentiment Analysis
We use VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool to score the text from from -1 (most negative) to +1 (most positive).
As you see, AITA stories are extremely not neutral…

<img width="743" alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/736530d0-a33f-46c3-a097-930931976510">

## Modeling
Binary Labeling:'Asshole' tagged as 1. 'Not The A-hole' tagged as 0.
<img width="807" alt="image" src="https://github.com/MonicaLiou1025/Sentiment-Analysis/assets/140920765/c1b34547-be0b-47f0-bcc1-f741f154d484">


