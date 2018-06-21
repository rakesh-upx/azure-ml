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
<img src="Images/mv%20scrubber.PNG>
          
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
![alt-txt](Images/scatter%20plot4.PNG)











