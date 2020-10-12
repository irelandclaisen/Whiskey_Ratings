# Whiskey Ratings

## Description
In this project, I scrape data from a whiskey rating site to develop a model that can predict whiskey ratings based on variables such as the whiskey's price, age, alcohol by volume, and descriptors, such as sweet, smoke, spice, etc.

## Featured Techniques
 * BeautifulSoup web scraping
 * Feature Engineering
 * Data Visualization
 * Linear Regression
 * Lasso regularized regression

## Data
Data was scraped from whiskeyadvocate.com.  To get the data, please run whiskey_pickling.ipynb.  This code will scrape the data, do some clean up, and generate a pickle file with all the data scraped from the website.

## Model Overview
The target variable is ratings.  Features included in the final model include ln(Price), Age, ABV, year review was made, reviewer, category (like scotch, bourbon, etc), and descriptors (like sweet, fruit, tobacco, etc.) A Lasso regularized regression was performed to help remove extraneous variables.  The linear regression model has an R2 of 0.4, RMSE of 3.7 and a MAE of 2.7.
