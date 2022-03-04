# stock-prediction
stock prediction
# Potential Business Problem:
Apple is one of the biggest tech giants. Its sales figures also benefit from the release of innovative products or services. 
Prediction of stock price index movement is regarded as a challenging task of financial time series prediction due to volatile and non-linear nature.
An accurate prediction of stock price movement may yield profits for investors. Here, we used a Long Short Term Memory Network (LSTM) for building our model to
predict the stock prices of Apple. With the introduction of Machine Learning and programmed methods of prediction have proved to be more efficient in predicting stock prices.
# Why solve this problem?
Companies and equity traders to predict future revenues and changes in the economic and business sectors.
 We'll be using a dataset from Kaggle and for this particular project, I have used the data for 'Apple'. This dataset contains information about apple stock. 
 The columns in the given dataset are as follows: date, open, high, low, last, close, etc. The data consists of records of roughly 14 features.
 #1. Exploratory Data Analysis

In Data Analysis we will try to find out missing values in the dataset, All the Numerical variables and Distribution of the numerical variables, Categorical Variables, Outliers, Relationship between an independent and dependent feature.
# 2. Feature Engineering
After cleaning the data, we can visualize data and better understand the relationships between different variables. There are many more visualizations that you can do to learn more about your dataset, like scatterplots, histograms, boxplots, etc
# 3.Model Training:
In this situation, we split the data into training set and test set, then fit candidate models on the training set, evaluate and select them on the test set. we are taking 0.60 i.e. 60% total length of data as our training size and remaining 40% would be our test size. considering this, Train dataset(754) and Test dataset(503) is formed. 
In timeseries data ,next step always dependent on previous step of data foe that we consider timesteps. Suppose we have to compute next day output, for that 'how many previous day' we need to be dependent on is decided by timesteps .we are just converting data into independent and dependent feature based on this timesteps. For instance, 
to predict the 51st price, this function creates input vectors of 50 data points prior and uses the 51st price as the outcome value. Similarly, for the next record we have to 
just shift one position to the right.
Be careful about making generalizations to other stocks, because, unlike other stationary time series, stock market data is less-to-none seasonal and more chaotic.
Just checking the RMSE does not help us in understanding how the model performed. Let's visualize this to get a more intuitive understanding. So here is a plot of the
predicted values along with the actual values.
![image](https://user-images.githubusercontent.com/61880535/156760398-1ad5038d-0660-41b0-a7c4-5494dd56a9ff.png)
# credits
I want to thank krish sir for sharing this project . It was a great learning experience.
# For MEDIUM blog:
https://medium.com/@tejashree-nawale/a-machine-learning-model-for-stock-price-prediction-109c2a942519
