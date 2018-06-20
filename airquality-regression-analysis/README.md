# Regression Analysis on Air Quality Data in Azure ML Studio

![alt-txt](Air%20quality/AlfedPalmersmokestacks.jpg)

## Objective
If the air is at 100-percent relative humidity, sweat will not evaporate into the air. As a result, we feel much hotter than the actual temperature when the relative humidity is high. If the relative humidity is low, we can feel much cooler than the actual temperature because our sweat evaporates easily, cooling -us off.
`The objective of the experiment is to predict Relative Humidity(RH) in air based on other detrimental contents in air at a given point of time`

## Data Description
Click [here](https://github.com/rakesh-upx/azure-ml/blob/master/airquality-regression-analysis/Dataset/AirQualityUCI.csv) to find the dataset
The dataset contains 9358 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an Air Quality Chemical Multisensor Device. The device was located on the field in a significantly polluted area, at road level, within an Italian city. Data were recorded from March 2004 to February 2005 (one year)representing the longest freely available recordings of on field deployed air quality chemical sensor devices responses. Ground Truth hourly averaged concentrations for CO, Non Metanic Hydrocarbons, Benzene, Total Nitrogen Oxides (NOx) and Nitrogen Dioxide (NO2) and were provided by a co-located reference certified analyzer. `Missing values are tagged with -200 value`.

![alt-txt](https://github.com/rakesh-upx/azure-ml/blob/master/airquality-regression-analysis/Air%20quality/Airquality%20data.PNG)

## Tool & Algorithms used
The entire analysis was performed in Azure ML studio using Linear Regression, Decision Forest Regression, Boosted Decision Tree & Neural Network algorithms

## Code snippets
### Summary of the data
![alt-txt](Air%20quality/Capture.PNG)
