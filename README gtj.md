# Project 3 - Web APIs & Classification

## Table of Contents

- Problem Statement
- Data Collection
- Data Cleaning and EDA
- Preprocessing and Modeling
- Evaluation and Conceptual Understanding 
- Conclusion and Recommendations 

Identify the Problem Statement:**

The goal of this project is to use API to extract posts from two different subreddits and analyze the text from each. Natural Language Processing (NLP) - CountVectorizer and TF-IDF Vectorizer - and various classification methods will be used in order to determine if my models can predict the subreddit source a cerratin post is taken from. This is a binary classification problem. Logistic regression models (considered KNN and SVM), decision trees, and naive bayes (required) will also be applied in this project to test if the baseline score can maybe be outperformed. 

The question is whether machine learning can determine the approval ratings using NLP, by classifying if a given reddit post originates from r/Republican or r/Democratic. (source: https://observer.com/2016/02/these-9-reddit-communities-will-help-you-decipher-and-discuss-the-presidential-race/)

My targeted users are data scientists who are in the employment of potential presidential candidates running for in the 2020 campaign . 

Executive Summary:**

As part of data wrangling and acquisition, information is requested from an API, scraped. 

To convert into standard text data, ie titles and comments, NLP is utilised that can allow analysis and modeling to be conducted. 

Given the classification problem, classification modeling is done as a means of assessment and classification preprocessing. 

Data Collection:**

Data gathering, through an API, shows r/Democrats with 1834 posts and r/Republican with 1856 posts of various stuff for instance policy, impeachment and candidates. A function in my .ipynb notebook to pull each subreddit. A CSV file is created where the 2 subreddits are merged together. 

Data Cleaning and EDA:**

Firstly, there are some missing data (null values), duplicate posts, whitepaces and HTML formatting that needs to be rectified. A target variable is created - Republican as 1 and Democrat as 0 - for mapping purposes. 

Combined selftexts and titles to just create a title column. (Many posts had no selftexts, drop selftexts column.) A forloop is crucial when the subreddits are being scrapped while I run the API multiple times API caps the data at 1000 posts for each subreddit.

Another function created to convert raw text to a string (of words). BeautifulSoup will be used to remove any HTML. Any Upper texts will be converted to lowercase using the .lower(). Function will be used to combine any overlaps of two sets of words from the two subreddits so as to create stopwords for the modeling process. The stop_words('english) will be used to converted stopwords to a set and remove any stopwords followed by using WordNetLemmatizer(). CountVectorizer will also be applied. After data cleaning, a new clean version will be saved as a csv.

Preprocessing and Modeling:**

First and foremost, the train data has the columns that will be used for the generation and refinement of the models. The test data will have the same columns, except the target that I set to predict in my Regression model. A regression model will be generate based on the train data, where I will validated it through train-test-split, cross-validation/ gridsearch for hyperparameters, analysis to see if there are any relationship (correlation) between predictive variables,  feature transformation (preprocessing)

*<u>****Pro Tip 2: Reddit will give you 25 posts per request. To get enough data, you'll need to hit Reddit's API repeatedly (most likely in a `for` loop). Be sure to use the `time.sleep()` function at the end of your loop to allow for a break in between requests. THIS IS CRUCIAL**</u>***

***<u>**Pro tip 4: At the end of each loop, be sure to save the results from your scrape as a `csv`: JSON from Reddit > Pandas DataFrame > CSV. That way, if something goes wrong in your loop, you won't lose all your data.</u>*****

Evaluation and Conceptual Understanding:**



Conclusion and Recommendation:**


