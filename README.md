# Data Science  Portfolio

This repository contains a series of projects I've used for learning Data Science and applying the technology and principles I've been studying.  Each project is in a separate folder.  Most of my data will be coming from `CSV` files downloaded from public sources (https://kaggle.com)

## Projects

#### 2021-12-02 - Weight Log Analysis

I record my weight in lbs and body fat percentage every day in a Google spreadsheet. I exported the data to CSV, cleaned it and created a couple of new metrics to explore the results.

I created scores for my weight and body fat percentage and compared them to days of the week to see their peformance. Generally, my weight and body fat is highest on Sundays and lowest on Wednesdays. I fluctuated toward heavier / fatter on several occasions. I also observed when I would hit a personal record for body fat, the subsequent weeks I would regress to a heavier and fatter state for a period (homeostasis).

In 2022, I plan to apply this knowledge by purposely attempting to lower my numbers on Sundays. I'm curious how that would effect the trend of swinging numbers.

#### 2021-11-05 - Genshin Data Analysis

The data is a collection of character statistics from the game Genshin Impact.  I explored the data with Pandas and Seaborn and cleaned the data in Pandas, translating terms from Portuguese to English and abbreviating some words to symbols to better read the data.

After exploring the data, I removed some outliers that I believe would have skewed the results of any predictive studies. My reasoning for these values being outliers was that they were nearly a full standard deviation larger than their adjacent, lower values (respectively).

I then created linear regression models with scikit-learn to compare how a couple of individual stats could predict a target. I chose `ATK -> HP` and `DEF -> HP` for testing. After creating the models. I graphed them on a scatterplot.

The result of the study showed that `DEF` was a better predictor than `ATK` for `HP`. I can improve on this study by:

- Experimenting with more features.
- Using different model families.
- Using Cross Validation to optimize different model families.

