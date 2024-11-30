The COVID-19 pandemic has posed unprecedented challenges to public health systems globally. Predicting the spread and severity of the virus is critical for informed decision-making, effective resource allocation, and timely policy interventions. 
This project leverages data science methodologies to build predictive models and provide actionable insights into COVID-19 trends.

The goals of this project are:

1. To analyze historical COVID-19 data and identify trends.
2. To provide visualizations and insights to support public health planning and classify countries based on confirmed, active cases and death rate.
3. To develop predictive models for forecasting case trends and classifying countries based on mortality rates.

**DATA PREPARATION AND CLEANING**
Data was extracted from kaggle. 
The full grouped data includes Date, Country/Region, Confirmed, Deaths, Recovered. 
The date column has type object which was changed to datetime type and other required columns like the recovery rate and death rate were created for proper visualisation. 
While other irrelevant columns were dropped 
After data processing the final data set used for visualization and modeling has 187 indexes and 6 columns 

**Explodatory Data Analysis**
The growth trend for the covid_19 cases and death followed an exponential growth trend in many nations. I used an heat map, two bar plots and a line plot to see nations that were mostly affected by Covid_19 
From the heat map, the US had the highest number of confirmed cases during the period, with brazil coming second, Russia third and India fifth. 
The bar plot was used to visualize the number of active cases and the US topped the list with Brazil and United kingdom following. 
Finally a line plot was used to visualize the trend in the top five nations. 
There was significant correlation between confirmed cases and death but the correlation with mortality rate was weak. 

**Classification Model Development**
Below is a summary of my Classification model 
Model: Random Forest Classifier.
Objective: Classify countries into "High" or "Low" mortality groups based on:
Confirmed, Deaths, Recovered, Active.
Evaluation Metrics:
1. Accuracy: 0.89
2. Precision: low (1), High(0.83)
3. Recall:  low (0.78) and High (1)
4. F1-score: low (0.88) and High (0.91)

 **Key Insights**
Based on the analysis and models:

Case and Mortality Trends:
Countries like US, brazil and Russia consistently exhibit higher mortality rates, driven by factors such as healthcare capacity or demographic profiles.
Recovery Rates:
High recovery rates were observed in regions with robust healthcare systems and early intervention strategies.
Model Accuracy:
The classification model achieved an accuracy of 0.89, making it reliable for identifying high-risk regions.


