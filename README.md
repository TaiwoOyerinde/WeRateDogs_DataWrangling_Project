# WeRateDogs_DataWrangling_Project
## Introduction:
In this project, my task was to wrangle, analyze and visualize data from three different sources on the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog.

## Gathering Data:
1. In gathering the first dataset, I manually downloaded a file,twitter-archive-enhanced.csv, from Udacity's project workspace and loaded it as a dataframetweets on my local jupyter notebook using pandas -read_cv.
2. For the second dataset gathering process, a link that contains tweet image predictions was provided in the Udacity's Classroom. I used the Requests library to programmatically download the tweets,image_predictions.tsv, locally on my desktop and loaded it as a dataframe image_tweets.
3. The last dataset used the Twitter API to gather data. I got my twitter developer account approved, retrieved all my access tokens and secrets, and ran codes for about 30 minutes using the 'tweet_id'in tweets( I used the guide given in the Udacity workspace,twitter-api.py) to gather additional data which downloaded on my desktop as tweet_json.txt . I initialized an empty list tweets_data , loaded the relevant data I needed(ids, retweets and favorite counts) and appended it to my empty list. Then, I converted the list tweets_data to a dataframe using pd.DataFrame and named it tweets_extra.
## Cleaning Data:
Before cleaning my data, I made copies of all 3 datasets. To clean my data, I took each of the issues documented from my assessing activity and ran them through the Define-Code-Test process. I carefully defined the problem, ran code(s) to solve the problem and then tested them to confirm the issue is resolved.

At the end of the cleaning process, I successfully combined all 3 datasets into 1,twitter, which I stored as twitter-archive-master.csv
## Analyzing Data:
I analyzed my final dataset for the following questions:

- Which top 5 tweets gained the most engagement using the retweet_count?
- Most tweets are from which source?
- What was the most favorite dog stage recorded?
- What rating level is most popular?
- Which dog breed has the strongest confidence level?
- Is there a correlation between retweet_count and favourite_count? If there is, what type of correlation is it?
- Most twitter handlers named their dogs?
- On which day of the week did tweets gather the most engagement based on the highest average retweet_count and favorite_count?
