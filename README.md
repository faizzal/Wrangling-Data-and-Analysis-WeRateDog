# Wrangling-Data-and-Analysis-WeRateDog
this project is about wrangling [gather-assest-clean] data and do some investigation and analysing using matplot library

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>
1. To install the application you need to install python - v3 on your own PC in addition to anaconda tool, then use git and clone the work from this repository and run the program and find the results.
2. You also need to create a developers account on the Twitter platform so you can get Key to use the API and get data of the partecular user to analyze the data, below you will find instructions to git key for twitter API.

First, if you do not already have one, you need to sign up for a Twitter account.
Next, to set up a developer account, follow the directions on Twitter’s Developer Portal, in the “How to Apply” section.
You will be guided through the steps, and asked to describe in your own words what you are building. Here is some suggested language you can use: "As a Udacity student, I need to access the Twitter API in order to complete a Data Wrangling student project. In this project, I'll be using Tweepy to query Twitter's API for data included in the WeRateDogs Twitter archive. This data will include retweet count and favorite count. Before I can run my API querying code, I need to set up my own Twitter application. Once I have this set up, I will develop some code to create an API object that I'll use to gather Twitter data. After querying each tweet ID, I will write its JSON data to a tweet_json.txt file with each tweet's JSON data on its own line. I will then read this file, line by line, to create a pandas DataFrame that I will assess and clean. I may post this completed project on my GitHub account, where it will get viewers. Otherwise there will be no other readers or users of my Twitter data or project analysis beyond the Udacity instructors and reviewers."
Once you submit your application, you should soon receive an email from Twitter letting you know they have approved your new Twitter developer account. Follow the link in the email from Twitter to a page of directions to get started creating your app.
If you are asked for an app name, it can be anything appropriate, and if you’re asked for a Website URL, it can be anything in a standard URL format. You can do the same with other requested URLs, or perhaps leave them blank.
If you’re asked to explain how your app will be used, you could say something like "I'm creating this for a student Data Wrangling project with Udacity, where we need to query and analyze Twitter data from WeRateDogs."
You should then be given a Success message, and a new developer page displayed to you where you can manage your app.
You can then go to the Keys and Tokens tab on this page to find or generate the Consumer API keys, and the Access Token and Access Token Secret that you will need.
after you have key apply it in folowen code

import tweepy

consumer_key = 'YOUR CONSUMER KEY'
consumer_secret = 'YOUR CONSUMER SECRET'
access_token = 'YOUR ACCESS TOKEN'
access_secret = 'YOUR ACCESS SECRET'

auth = tweepy.OAuthHandler(consumer_key, consumer_secret)
auth.set_access_token(access_token, access_secret)

api = tweepy.API(auth)


## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using Stack Overflow data from 2017 to better understand:

1. How other developers suggested breaking into the field (what education to pursue)?
2. What factors about an individual contributed to salary?
3. How bias played a role in the suggestions of developers for how to break into the field?
4. What was the state of bootcamps for assisting individuals with breaking into developer roles?
5. How were bootcamps assisting with increasing diversity in tech careers?

The full set of files related to this course are owned by Udacity, so they are not publicly available here.  However, you can see pieces of the analysis here.  This README also serves as a template for students to follow in creating their own project README files.


## File Descriptions <a name="files"></a>

There are 3 notebooks available here to showcase work related to the above questions.  Each of the notebooks is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps.  

There is an additional `.py` file that runs the necessary code to obtain the final model used to predict salary.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@josh_2774/how-do-you-become-a-developer-5ef1c1c68711).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to Stack Overflow for the data.  You can find the Licensing for the data and other descriptive information at the Kaggle link available [here](https://www.kaggle.com/stackoverflow/so-survey-2017/data).  Otherwise, feel free to use the code here as you would like! 
