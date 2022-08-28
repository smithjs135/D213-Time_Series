# D213-Time_Series of the Hospital Dataset

## Overview
Created a tool that performs time-series analysis on the medical data set ('medical_time_series.csv') which contains a day and revenue component for one year. The expected goal of this analysis is to gain the ability to make predictions on revenue for the following year.

The data set consists of 731 rows (days) and two columns or variables: 
  * Day: Day during first two years of operation 
  * Revenue: Revenue in million dollar

## Research Question
What is the projected revenue for next year?

Time-Series analysis will be performed on the medical data set ('medical_time_series.csv') which contains a day and revenue component for one year. The expected goal of this analysis is to gain the ability to make predictions on revenue for the following year.

## Method Justification
We typically make some assumptions when performing a time-series analysis. First of which is we assume the data is stationary. This means the mean, standard deviation, and autocorrelation do not change over time. If the data is not initially stationary, it can typically be transformed into stationary data.

Another assumption we make for time-series analysis is there little to no autocorrelation in the data. Autocorrelation typically occurs when residuals are not dependent of each other.

**Evaluation of Dickey Fuller Test:** 
The p-value returned if 0.200 and the test statistic is -2.22. We fail to reject the hypothesis because the p-value is not below the 0.05 threshold. Furthermore, the test statistic is not less than the critical values. We do not have the 95% confidence level to reject the null hypothesis, so this series is non-stationary.

## Visualizations
![image](https://user-images.githubusercontent.com/46407407/187098886-59ed69e8-7314-428d-80e0-7e7a2e67417e.png)

![image](https://user-images.githubusercontent.com/46407407/187099010-9ddd42eb-8bf8-4044-81b8-4ea615bac6cf.png)

![image](https://user-images.githubusercontent.com/46407407/187099050-e242b2c0-e4be-4fe0-8bc3-e52f8622723d.png)

![image](https://user-images.githubusercontent.com/46407407/187099071-510ddded-34f1-409d-bda4-4693b54a4340.png)

![image](https://user-images.githubusercontent.com/46407407/187099106-ced05962-9cd1-4120-aa86-cf72c9e8f2e1.png)

![image](https://user-images.githubusercontent.com/46407407/187099165-6d39e62c-bbff-44a6-9957-62ecd5205606.png)

![image](https://user-images.githubusercontent.com/46407407/187099177-d90f25ef-da0a-4fe0-99d1-9546a1096a0e.png)

![image](https://user-images.githubusercontent.com/46407407/187099209-df389b6a-b6ad-467d-b9b0-1615a4bd91eb.png)

**Forecast Model**
![image](https://user-images.githubusercontent.com/46407407/187099299-1f19363d-2176-4db6-92ae-dbf81c48873f.png)

## Recommendations
Recommendations
This timeseries analysis demonstrates a repeating pattern of variance in hospital revenues. Overall the mean revenue stays fairly consitant throughout this 2 year study. The forecast suggests future revenue will not deviate much from the mean. My recommendation to the stakeholders is to determine the primary influencers of the revenue fluctuations to see if this can lead to a better understanding of revenue fluctuations and insight on how to increase future revenue.



## Libraries
* pandas
* numpy
* seaborn
* matplotlib
* statsmodel
* sklearn


