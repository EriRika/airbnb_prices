## Airbnb price analysis, data visualisation, and feature handling

In this analysis I tried to answer 4 business questions
- How expensive is a night in Seattle?
- When should I visit Seattle?
- Can I find great places without paying too much money?
- What can I learn about the different districts and their vibes?
- 



## Table of contents

- [Data used](#data-used)
- [Libraries used](#libraries-used)
- [What's included](#whats-included)
- [Content of Notebook](#content_of_notebook)
- [Summary](#summary)


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
1. Business Problem
2. Data Understanding
3. Data Preparation
   1. Convert Columns to float or date
   2. Clean numerical columns
4. Data understanding after Data Preparation
   1. histogram of prices
   2. boxplot of prices
   3. Boxplot price per categorical variable
   4. Boxplots and histograms of price per binary variable
   5. Correlation of numericla variables
   6. Scatterplots between numerical columns and price
   7. Price per day
   2. Amount of listings over time
   3. Cost per weekday vs. listings per weekday
5. NLP analysis
   1. Find describing adjectives of listing
   2. Find describing adjectives of location
   3. Find describing nouns of location 
6. Modelling Linear Regression
7. Evaluating Linear Regression  
8. Modelling CatBoost
9. Evaluating CatBoost  

## Summary
- How expensive is a night in Seattle?
<br />Prices are around 100$, but there are many outliers
![alt text](https://github.com/EriRika/airbnb_prices/blob/master/pictures/Price%20boxplot.png)
![alt text](https://github.com/EriRika/airbnb_prices/blob/master/pictures/Price%20histogram.png)

- When should I visit Seattle?
 <br />Seattle is cheapest between October and May. On top od that one can save in average 8$, if you do not stay during the weekend
![alt text](https://github.com/EriRika/airbnb_prices/blob/master/pictures/Average%20Price%20per%20weekday.png)
![alt text](https://github.com/EriRika/airbnb_prices/blob/master/pictures/Average%20Price%20over%20time.png)

- Can I find great places without paying too much money?
 <br />Yes, looking at the rating, we can see that there is no correlation between a very good rating and the price
 ![alt text](https://github.com/EriRika/airbnb_prices/blob/master/pictures/scatter_review_scores_rating.png)

- What can I learn about the different districts and their vibes?
 ![alt text](https://github.com/EriRika/airbnb_prices/blob/master/pictures/Diverse%20District.PNG)
 <br />By extracing the top 10 adjectives and nouns per district, I was able to describe them

- Can I predict the price per listing?
 <br />I reached an R2 of 0.62, which is acceptable, but not particularly good. The model underpredicts especially very expensive listings. One reason could be that there is an higher order dependency with the price between some features.

   
[Medium Post - What Secrets does Airbnb data tell me about Seattle?](https://erikagintautas.medium.com/what-secrets-does-airbnb-data-tell-me-about-seattle-49fba69eb362)


