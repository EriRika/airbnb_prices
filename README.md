## Airbnb price analysis, data visualisation, and feature handling

In this analysis I tried to answer 4 business questions
- How expensive is a night in Seattle?
- When should I visit Seattle?
- Can I find great places without paying too much money?
- What can I learn about the different districts and their vibes?



## Table of contents

- [Data used](#data-used)
- [Libraries used](#libraries-used)
- [What's included](#whats-included)
- [Content of Notebook](#content_of_notebook)


## Data used
The data contains air bnb listings, reviews and calendar entries

- [Data can be downloaded from here](https://www.kaggle.com/airbnb/seattle)

## Libraries used
- seaborn
- pandas
- numpy
- datetime
- sklearn
- nltk
- matplotlib
- warnings

## What's included
Within the download you'll find the following directories and files

```text
airbnb_prices/
├── AirBnB Seattle data Data cleaning, prediction and NLP.ipynb
├── airbnb data Seattle/
│   ├── listings.csv
│   ├── calendar.csv
│   ├── reviews.csv
└── pictures/
    ├── Price boxplot.png
    ├── Price histogram.png
   
```


## Content of Notebook
1. Import data and libraries
2. Understand the data and do some first checks
3. Data Cleaning
   1. Convert Columns to float or date
   2. Clean numerical columns
4. Gather some visual informaion
   1. histogram of prices
   2. boxplot of prices
   3. Boxplot price per categorical variable
   4. Boxplots and histograms of price per binary variable
   5. Correlation of numericla variables
   6. Scatterplots between numerical columns and price
5. Plot price development over time
   1. Price per day
   2. Amount of listings over time
   3. Cost per weekday vs. listings per weekday
6. NLP Analysis
   1. Find describing adjectives of listing
   2. Find describing adjectives of location
   3. Find describing nouns of location 
7. Predict Price
   1. Linear Regression
   2. CatBoost
   



