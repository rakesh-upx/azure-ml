# Crime data for cluster analysis in Azure ML Studio
Please click [here](https://gallery.azure.ai/Experiment/Cluster-Analysis-on-Crime-Data) to view the project


<p align="center">
  <img src="Images/cuchillo-con-sangre.jpg",alt="neofetch" align="middle" height="200px">
  </p>


## Objective
The objective of the project is to assign the cases of different sorts of crime across fifty states of the USA in 1973 to groups based on similarity each case exhibits among themselves & take appropriate action for each group based on behaviour shown by them

## Dataset description
Please click [here](Dataset/crime_data1.csv) to view the dataset.The dataset contains 50 instances of violent crime across 50 states of the USA in 1973.

### Attribute Description:

* _Murder_ : (Numeric) Murder arrests (per 100,000)

*  _Assault_ : (Numeric) Assault arrests (per 100,000)

* _Urban Population_ : (Numeric) Percent urban population

* _Rape_ : (Numeric) Rape arrests (per 100,000)

## Tools & algorithm used
The entire experiment was performed in Azure ML Studio using KMeans algorithm of both R & Azure ML module

## Code Snippets
Picture below is the entire experiment conducted in Azure ML workspace
![alt-txt](Images/Experiment.PNG)

### Loading the data
The dataset was collected from an online source and uploaded on Azure ML dataset component

### Summary of the data
Desriptive Statistics of the dataset was found using `Summarize module` of Azure ML Studio
<img src="Images/Capture.PNG">
### Data Wrangling
Data attributes were studied well before proceeding further analysis & found to have some missing cells.Missing cells were replaced with proper method, scatter plots were drawn to visualize relationships among the variables.
Missing cells were noticed using Summary of the data set shown above.
#### Missing Value Replacement
Missing cells were replaced using MICE technique which is very useful perhaps very appropriate method for replacing missing cells as far as the data set is concerned

![alt-txt](Images/mv%20scrubber.PNG)
          
#### Quick recheck of missing cells if any after replacement with MICE
![alt-txt](Images/summary%20after%20replacing%20mv.PNG)   

#### Visualization for finding relation between the variables
![alt-txt](Images/scatter%20plot1.PNG)
##### Output
![alt-txt](Images/scatter%20plot2.PNG)
![alt-txt](Images/scatter%20plot3.PNG)
##### Output
![alt-txt](Images/scatter%20plots.PNG)
![alt-txt](Images/scatter%20plot4.PNG)
![alt-txt](Images/scatterplot5.PNG)
![alt-txt](Images/scatter%20plot%206.PNG)
![alt-txt](Images/scatter%20plot7.PNG)

### Core Analysis
After data wrangling the prepared dataset was used for applying KMeans algorithm from both Azure ML library & R library

#### Execute R Script to find optimal K(Number of clusters)
![alt-txt](Images/R%20script%20for%20elbow%20method.PNG)
#### Output
![alt-txt](Images/elbow%20plot.PNG)


Elbow was noticed at cluster 3 i.e. when K=3, so we'll proceed with K=3 for modeling the data.
#### Let start with KMeans from library of R
![alt-txt](Images/Kmeans%20with%20R.PNG)
#### Output
The test result shows centroids of each cluster,cluster vector,cluster size,SSW & SSB
![alt-txt](Images/Output%20of%20KMeans%20with%20R.PNG)
#### Applying KMeans algorithm using Azure ML module
Parameters used to model the data using Azure ML Kmeans module

![alt-txt](Images/parameters%20for%20Kmeans%20in%20Azure.PNG)

Please click [here](Dataset/Cluster%20Analysis%20Results%20dataset.csv) to view the output of Kmeans test.


## Future Scope
Clustering is one of the essential Machine Learning techniques used widely in Data Science.The experiment conducted on the crime data holds good scope of refurbishing security in the states belonging to different clusters as per requirement. Thus we can use cluster algorithm to predict crime cases in other places & essentially on other data. 

























