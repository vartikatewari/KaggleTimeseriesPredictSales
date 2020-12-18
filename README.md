# KaggleTimeseriesPredictSales
Time-series forecasting of retail products sales using MachineLearning


Accurate Time series prediction has various real applications. In this project we tackle a similar problem provided by Kaggle, as part of their ongoing ”Predict Future sales” competition [4]. We handle challenging time series data of daily sales from the largest Russian software firms- 1C Company. Given past data the goal is to predict monthly sales for every possible shop item pair, and make the model robust to the seasonal changes and trends. We employ and compare three models, Prophet, random forest and xgboost for prediction, and evaluate them on Root Mean Squared Error(RMSE). We obtain the best peformance with xgboost as 0.85 RMSE on the test set where the target range is [0-20].

### Dataset Description
The data-set consists of daily sales data. There are about 3 million such records in the training set, collected over 60 shops selling 20,000 unique items.
Training data consists of records with information that a particular item had been sold in a particular shop, in a particular day, in the training period. The training period is about one and a half year. Testing period is the month that falls on training period. The data-set also has missing data as not every item is sold in the above time period.

### Data Cleaning and pre-processing
We removed the negatively priced items from the dataset. We also dropped the text features completely as they were in Russian.
We replaced missing product count with 0 We removed outliers by clipping item count to be less than or equal to 20.

## Pre-requisites
Python Packages
*scikit
*pandas
*numpy
*matplotlib
*seaborn
*statsmodels
*fbprophet
*xgboost

## How to explore the project
The project is divided into folders

Code : has notebooks for data processing, time series analyis and running models

Visualizations: contains the plots 

Data: contains the data files given as well as the features generated

Resources: contain related papers and reports



