# Regression Analysis on Air Quality Data in Azure ML Studio

Please click [here](https://gallery.azure.ai/Experiment/Air-Quality-in-an-ItalianCity-2) to view the project.

![alt-txt](Air%20quality/AlfedPalmersmokestacks.jpg)

## Objective
If the air is at 100-percent relative humidity, sweat will not evaporate into the air. As a result, we feel much hotter than the actual temperature when the relative humidity is high. If the relative humidity is low, we can feel much cooler than the actual temperature because our sweat evaporates easily, cooling -us off.
`The objective of the experiment is to predict Relative Humidity(RH) in air based on other detrimental contents in air at a given point of time`

## Data Description
Click [here](https://github.com/rakesh-upx/azure-ml/blob/master/airquality-regression-analysis/Dataset/AirQualityUCI.csv) to find the dataset.
The dataset contains 9358 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an Air Quality Chemical Multisensor Device. The device was located on the field in a significantly polluted area, at road level, within an Italian city. Data were recorded from March 2004 to February 2005 (one year)representing the longest freely available recordings of on field deployed air quality chemical sensor devices responses. Ground Truth hourly averaged concentrations for CO, Non Metanic Hydrocarbons, Benzene, Total Nitrogen Oxides (NOx) and Nitrogen Dioxide (NO2) and were provided by a co-located reference certified analyzer. `Missing values are tagged with -200 value`.

![alt-txt](https://github.com/rakesh-upx/azure-ml/blob/master/airquality-regression-analysis/Air%20quality/Airquality%20data.PNG)

## Tool & Algorithms used
The entire analysis was performed in Azure ML studio using 
`Linear Regression`
`Decision Forest Regression`
`Boosted Decision Tree`
` Neural Network algorithms`

## Code snippets

### Loading the data
The data set was collected from UCI repository & uploaded on Azure. The noticeble part of the data set is the missing values were tagged with `-200` across all the variables.

### Summary of the data
![alt-txt](Air%20quality/Capture.PNG)

### Data Wrangling
All the attributes were well studied before performing Data Wrangling in which I did some feature transformations,missing value analysis,correlation analysis,feature selection & splitting data set into train& test set executing R Script , Python Script other Azure ML modules.
![alt-txt](Air%20quality/Data%20wrangling.PNG)

### Replacing -200 with NaN 
It'll help us to replace the missing cells of the data set at later stage with any appropriate method
![alt-txt](Air%20quality/Replacement%20-200%20with%20NaN.PNG)

### Finding number of missing cells per column
![alt-txt](Air%20quality/Execute%20R%20Script(Airquality).PNG)
![alt-txt](Air%20quality/mv(Airquality).PNG)

### Replacing Missing Values
![alt-txt](Air%20quality/cleaning%20mv(AirQuality).PNG)

### Quick recheck of missing cells if any after replacement with probabilistic PCA
![alt-txt](Air%20quality/rechecking%20missing%20cells.PNG)

### Pair plots for visualizing correlation between the vriables
#### Execute R script
![alt-txt](Air%20quality/correlation.PNG)
#### Output
![alt-txt](Air%20quality/correlation%20plot(airquality).PNG)

### Core Analysis
After data wrangling, the split data set was all ready for core analysis in which 4 above mentioned algorithms were used to model the train data & scoring was done with test data.
![alt-txt](Air%20quality/Core%20analysis.PNG)

### Outcome of the Experiment
The performance of each algorithm was tabulated in a meaningful & convenient manner keeping all the evaluation metrics alligned so that it gets easily accessible & understandable to the viewers
![alt-txt](Air%20quality/Outcome(Airquality%20Analysis).PNG)

## Future Scope of the experiment
Humidity drives most of the observable weather phenomena starting with clouds via fog, rain to storms and finally to such dramatic weather phenomena as hurricanes. It is not possible to forecast the weather exactly without precise knowledge of humidity in all the layers of the atmosphere. Correct relative humidity is important for our well-being and health.The experiment has attempted to forecast Relative Humidity(RH) based on given factors(Variables influencing).In the mould of this experiment, Relative Humidity can be predicted in other places to offer Meteorologists insights to forecast weather patterns.


















