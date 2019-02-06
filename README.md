## Introduction
The project was part of the data wrangling part of the Udacity Data Analyst Nanodegree program. The dataset that you will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as WeRateDogs. This Twitter account that rates people's dogs with a humorous comment about the dog. Ratings almost always have a denominator of 10, however the numerators are usually greater than 10. 11/10, 12/10, 13/10, etc. This unique rating system is a big part of the popularity of WeRateDogs and does not need to be cleaned.


## Project Details

The tasks for this project were:
- Data wrangling, which consisted of:
  - Gathering data
  - Assessing data
  - Cleaning data
- Storing, analyzing, and visualizing the wrangled data
- Reporting on my data analyses and visualizations (act_report.pdf)

__Important note:__
The project requires only original ratings (no retweets) that have images. Not all of the original tweets in the dataset are dog ratings and some are retweets.

#### Gathering Data
For this project we will be using data from three sources:
 1. The WeRateDogs Twitter archive. Which we need to download manually by clicking the following link: [twitter_archive_enhanced.csv](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv)
 2. The tweet image predictions, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file  [image_predictions.tsv](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv) should be downloaded programmatically using the Requests library. 
 3. Using the tweet IDs in the WeRateDogs Twitter archive, we need to query the Twitter API for each tweet's JSON data using Python's Tweepy library and store each tweet's entire set of JSON data in a file called tweet_json.txt file. We should gather each tweet's retweet count and favorite ("like") count at minimum, and any additional data you find interesting.

#### Assessing Data
After gathering each of the above pieces of data, assess them visually and programmatically for quality and tidiness issues. Detect and document at least eight __(8) quality issues__ and __two (2) tidiness issues__ in your `wrangle_act.ipynb` Jupyter Notebook.

#### Cleaning Data 
Clean each of the issues you documented while assessing. Perform this cleaning in `wrangle_act.ipynb` as well. The result should be a high quality and tidy master pandas DataFrame (or DataFrames, if appropriate).

#### Storing, Analyzing, and Visualizing Data
Store the clean DataFrame(s) in a CSV file with the main one named `twitter_archive_master.csv`. If additional files exist because multiple tables are required for tidiness, name these files appropriately. Additionally, you may store the cleaned data in a SQLite database (which is to be submitted as well if you do).

Analyze and visualize your wrangled data in your `wrangle_act.ipynb` Jupyter Notebook. __At least three (3) insights__ and __one (1) visualization__ must be produced.

#### Reporting
Create a __300-600 word written report__ called `wrangle_report.pdf` or `wrangle_report.html` that briefly describes your wrangling efforts. This is to be framed as an internal document.

Create a __250-word-minimum written report__ called `act_report.pdf` or `act_report.html` that communicates the insights and displays the visualization(s) produced from your wrangled data. This is to be framed as an external document, like a blog post or magazine article, for example.

## Author
This project was completed by Mateusz Zajac.
