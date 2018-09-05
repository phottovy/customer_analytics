# Looking Back to (Predict) the Future
## Part Two - Exploring Customer Analytics

Galvanize Data Science Immersive | Capstone #3 | September 2018

This is part two of my capstone project using this dataset. Part one can be found [here][1].

### Pat Hottovy
#### Data Scientist
Email: p.hottovy@gmail.com  
Linkedin: [in/patrick-hottovy](https://www.linkedin.com/in/patrick-hottovy/)


## Table of Contents
* [Background](#background)
* [Data](#data)
* [Objectives](#objectives)
* [Approach](#approach)
* [Measures](#measures)
* [Results](#results)
* [References](#references)
<!-- * [About Me](#about-me) -->

<a id='background'></a>
## Background
![ClickFox_logo][3]  
<!-- <img style="float: right;" src="images/CF_logo.png"> -->
In today’s business world, anticipating the needs and wants of your customers is vital to the success of your business. Partnering with [ClickFox][2], the leader in “Customer Journey Analytics,” I was able to gain valuable real-world experience using advanced analytics working with customer data on a current business use case.  

For a particular client, ClickFox provides forecasts for daily, aggregated KPI’s related to key segments of the customer journey. The goal of this project is to both analyze the current process and look for ways to optimize the flow of information going forward.



<a id='data'></a>
## Data
The datasets consist of a number of separate daily feeds containing different customer metrics. For each feed, six different predictions using various time series methods are included. In addition, each daily forecast contains predictions for 14 days into the future. I was provided 10 months of raw data and actuals for these feeds to use for my analysis.

![data_example][4]

**Fig 1: Example Raw Data for one of the feeds**  
**Fig 2: Actuals compared to best forecast for that day**  
**Fig 3: Composite of the best predictor per day by color**


<a id='objectives'></a>
## Objectives
* Evaluate the six predictions methods currently being provided to the client
* Analyze the time series data and identify the trends and features that are most indicative of future activity
* Create a workflow from the current process to provide a single daily forecast using either one or a combination of the current predictors


<a id='approach'></a>
## Approach
* Evaluate current predictors using root mean squared error (RMSE)
* Perform time series decomposition and stationarity tests
* Create my own forecasts for comparison to the current predictors
* Create a pipeline with a variety of statistical modeling techniques to find the optimal results
 * Build a workflow using the best model to provide one daily feed


<a id='measures'></a>
## Measures
Even though the daily KPI is a continuous variable, the focus of this project was to determine which of the current predictors or combination of predictors provided the best results.

This ultimately turned the project into a multiclass classification problem. I created models and tested the data using the following techniques:
* Logistic Regression
* k Nearest Neighbors
* Ensemble methods
 * Random Forests
 * Gradient Boosting
* Multilayer Perceptron Neural Network


<a id='Results'></a>
## Results
After building a pipeline to test the data, I discovered with this data, all of the classification models provided reasonably similar results. Below are the models that provided the best scores for the different feeds:

![model_pie][5]

<a id='references'></a>
## References
* ClickFox has proven customer journeys “to be over 30% more predictive than individual events.” Using advanced analytics, ClickFox provides its clients with insights to get the most value out of each interaction with its customers. [clickfox.com/expert-opinions](www.clickfox.com/expert-opinions)




[1]: https://github.com/phottovy/time_series_forecasting
[2]: https://www.clickfox.com
[3]: images/CF_logo.png
[4]: images/git_data_example.svg
[5]: images/git_model_pie.svg
[3]: images/
[3]: images/
[3]: images/
