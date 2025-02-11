# IS597
Spring 2025-IS 597-Human Centered Data Science at UIUC

## Assignment 1: Reddit Data Collection & Visualization

Background

Reddit is a social network of communities (e.g., a humen-centered data community like UIUC student reddit) where people can dive into their interests, hobbies, and passions. Registered users can post content (e.g., links, text posts, images, and videos) to the site. The posts can then be voted up or down by other members. Posts are organized by subject into user-created boards called "communities" or "subreddits". According to Semrush, as of July 2022, Reddit ranks as the 10th most-visited website in the world and the 6th most-visited website in the U.S. The public Reddit data can be accessed by authorized applications on Reddit.

Objectives

Build a crawler that collects a list of Reddit posts in a given subreddit based on different post sorting criteria.
Perform frequency analysis on the collected text data.
Build a network analysis tool that measures and visualizes the network structure of the collected user comments.
Introduction to Open Authentication (OAuth)

Note: Please safely store all the key pairs and tokens the first time you generate them. The key pairs and tokens might not be accessed beyond the first time they are generated.

Open Authentication (OAuth) on Reddit. Here is the reference for more details about OAuth on Reddit. Most Reddit API functions can be accessed by registered applications (e.g., the crawlers you will develop in this assignment) through OAuth 2.0. To register your application, you first need to have a Reddit account. If you already have one, you can directly use it. Otherwise, you will need to create an account on Reddit. Then, you need to create an application and get the keys (i.e., a pair of Client ID and Client secret). The main steps for the above registration are summarized below: Go to https://www.reddit.com/prefs/apps/Links to an external site., and create a new Reddit application for this assignment by clicking "create an app" at the bottom. Select "web app" and fill in all required fields. You can pick a name of your choice for the application. For the URL and redirect URI, you can either use your own homepage or simply type the HTTP address of your machine. Submit the form, record the Client ID (next to your app icon under "developed applications") and Client secret (in the "secret" section) from the screen and use them in your application (i.e., crawlers).

Introduction to PRAW (The Python Reddit API Wrapper)

Python is a great programming language for fast text data processing. Active developer communities create many useful libraries that extend the language for various applications. In this assignment, we introduce PRAW (A Python Reddit API Wrapper), which is a Python API wrapper that we can easily access Reddit APIs. It is open-sourced and hosted on Github. Building upon our code skeleton, we aim to collect a JSON file of subreddits with given keywords and filters.

This programming assignment requires Python 3.8 or later and additional Python packages. You can download Python from Python Download and find more information about Python at www.python.orgLinks to an external site.. If you are new to Python, here is a tutorial to get started on Python: docs.python.org/3/

*If you use other versions of Python (i.e., 3.7 or earlier), please make sure your code runs correctly and specify the version number of your Python in the README file you turn in.

Assignment Running Environment

For this assignment, detailed instruction and skeletal code are provided as an iPython notebook. You may either download the .ipynb file provided and run the code locally or finish the code on the Google Colab environment. You can check more details of those running environments in Tutorial 0 slides. For all tasks, detailed instructions are provided in the iPython notebook, here we will have an overview of the assignment.

Note: Just for your information, Reddit has some rate limits on its Public API. You can get more information here: Reddit Data API Limit.

Exercises

Data Collection:

1.1 Fetch hot subreddits of a Reddit [5 pt]
1.2 Search subreddits based on keywords ordered by relevance [10 pt]
1.3 Search subreddits based on keywords ordered by time [5 pt]
1.4 (Filters) Add time filter to your keyword search [5 pt]
1.5 Collect Reddit data around a topic and examine the collected data [15 pt]
Data Exploration:

2.1 Basic Stats, Data exploration [5 pt]
2.2 Wordcloud visualization [10 pt]
2.3 Word Frequency Analysis [15 pt]
2.4 N-gram analysis [10 pt]
Network Visualization:

Construct a directed graph visualization using networkx and matplotlib [15 pt]
What to Turn In:

A zip file containing the following:

.ipynb file containing your code.
Run your iPython notebook and export the .ipynb file as a PDF file; submit the PDF file containing outputs of your code.
Collected data file.
Assignment File:

Download this Jupyter Notebook and finish the coding assignment by following instructions provided. Please use Google Colab to avoid any confusion in environment setting by uploading the provided Jupyter notebook here https://colab.research.google.com/Links to an external site..

Assignment1.ipynbDownload Assignment1.ipynb
Due Date:
This assignment is due 11:59 pm on March 3.
