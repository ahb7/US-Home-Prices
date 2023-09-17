# The key factors influencing US Home Prices.

S&P Case-Schiller Home Price Index is used as a proxy for home prices: fred.stlouisfed.org/series/CSUSHPISA.

In this project, first, I looked for data. And collected the following datasets.

## Data Collection:
All most all the data is collected from the Fred Economic Data website https://fred.stlouisfed.org/

### The dataset are:
Case-Schiller Home Price Index (CSUSHPISA) is our target variable.
Download link: https://fred.stlouisfed.org/series/CSUSHPISA

Consumer Price Index (CPILFESL)
Download link: https://fred.stlouisfed.org/series/CPILFESL

Construction Materials Price Index (WPUSI012011)
Download link: https://fred.stlouisfed.org/series/WPUSI012011

New Housing Units completed (COMPUTSA)
Download link: https://fred.stlouisfed.org/series/COMPUTSA

Real Interest Rate (REAINTRATREARAT10Y)
Download link: https://fred.stlouisfed.org/series/REAINTRATREARAT10Y

Unemployment Rate (UNRATE)
Download link: https://fred.stlouisfed.org/series/UNRATE

GDP Per Capita (GDPPC)
Download link: https://fred.stlouisfed.org/series/A939RX0Q048SBEA

The datasets were considered from 01-Jan-2000 to 01-June-2023
All data were merged into a single file inputFile.csv

## Exploratory data analysis:
Summary, scatter plot and correlation among the variables were done as part of exploratory data analysis.

## ML Model:
I tried with Linear Regression and xgboost. Xgboost gave better result, hence this is the final choice.

## Results:
The xgboost model gave the following evaluation metrics values.
```
R^2: 0.9943268764763544
MAE: 2.4089355755974258
MSE: 13.096733896525008
RMSE: 3.6189409910255526
```
The scatterplot plots the actual Case-Shiller U.S. National Home Price Index (HPI) vs Predicted HPI.
![ModelEvaluationImage](https://github.com/ahb7/US-Home-Prices/assets/17172345/e06cfccd-c789-4134-9955-7c549b2bcb89)

<strong>In the above plot, the Actual Home Prices Index(HPI) vs Predicted HPI line is at almost 45 degree angle.   
This is an indication of the very high accuracy of the model. This demonstrates that the chosen factors   
strongly influence the US Home Prices Index.

Please see the inputFile.csv and the jupyter notebook for the actual code.</strong>


