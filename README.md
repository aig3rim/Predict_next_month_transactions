# Predict next month transactions using RFM features and linear regression

## Introduction

This is a source code for a [Medium](https://aigerimshopenova.medium.com/) blog post Predict Next Month Transactions with RFM Features.

### Motivation
As a data scientist working in marketing, I was curious about data engineering part, which combines business understanding and hard skills. Therefore, I decided to create and test RFM features for a machine learning model. I believe it's quite important to have a good businees understanding before engineering featueres and know what kind of business question is needed to be answered.

### RFM
Recency, frequency, monetary (RFM) is a marketing analysis tool used to identify a company's best customers by using the following measures:
* Recency: How recently a customer has made a purchase
* Frequency: How often a customer makes a purchase
* Monetary Value: How much money a customer spends on purchases

### Dataset
For this analysis I am using a public dataset from UCI Machine Learning Repositiry, which can found [here](http://archive.ics.uci.edu/ml/index.php). This dataset contains information on transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

## Getting started
You need an installation of Python, plus the following libraries:

* numpy
* pandas
* matplotlib.pyplot
* seaborn
* sklearn
* statsmodels.api

## Summary and key findings
* We predicted next month transactions based on engineered RFM features using linear regression
* Looking at p-values, we can say that Frequency and IsEIRE features are statistically significant to predict the number of transactions for the next month
* R-squared = 0.649, which means that the model explains about 64.9% of the variation, which is relatively good. However, we could create more features and/or fit other models such as polynomial, Ridge or Lasso models to improve the metric or try other models.
