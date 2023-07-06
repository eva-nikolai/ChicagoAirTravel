# Chicago Airport Performance Predictions

**Summary**

Given the high volume of flights per day in Chicago and unique weather conditions that affect the “Windy City”, consumers should inform their ticket purchases with which airport is the most efficient given a certain time of year. Therefore, this project compares departure delays between Chicago O’Hare (ORD) and Chicago Midway (MDW) to predict which Chicago airport is the most likely to get customers to their final destination on-time.

Objectives:

* Utilize web scraping in Python to produce datasets of departure delays from ORD and MDW
* Analyze most recent 10 years of of delays using various statistical regression and smoothing methods
* Develop accurate and validated forecasts of departure delays using R and Python

**Methodology**

This project uses two datasets produced from scraping the Bureau of Transportation Statistics Websites to forecast future departure delays at both Chicago O'Hare and Midway. It first prepares the data, then checks for random walks in the data, and finally compares multiple forecasting methods including regression, smoothing, ARIMA, and LTST models, to identify the most accurate prediction method as well as which airport has the stronger on-time departure performance.

**Check for Random Walk**

Before beginning the models, we first checked for random walks in the data using r libraries "forecast" and "zoo", finding the data does not have a random walk.

**Regression** 

We then moved into our regression-based models, and compared their accuracies to identify the highest performing model.

**Smoothing**

Next, we evaluated the performance of the Holt-Winter Exponential Smoothing method at each airport and similarly compared their accuracies to identify the highest performing model. 

**ARIMA** 

The third models performance we tested on our data was our ARIMA model and its' accuracy against the regression methods, smoothing methods, and benchmark naive method.

**Long-term Short-term Memory Model**

The last model we evaluated on our dataset was the Long-term Short-term Memory Model (LTST). Using Python, we utilized the "pandas", "tensorflow", "numpy", and "matplotlib.pyplot" libraries to prepare the data for model usage, apply the method, and plot the findings. We then compared the results again against all other models.

**Results**

When comparing each model's performance on the Chicago Airport Departure Delay Data, we determine that the ETS(AAA) method performed best on the Chicago O'Hare dataset and that the ETS(ANA) method performed best on the Chicago Midway dataset. 

After comparing the airports using their most accurate methods, we find that Chicago O'Hare is predicted to be more reliable in delivering on-time flight departures than its competitor, Chicago Midway. 