# Wisconsin Breast Cancer Data for Classification Analysis


Please click [here](https://gallery.azure.ai/Experiment/Breast-Cancer-2) to view & download the experiment.


<p align="center">
  <img src="Breast_Cancer_Images/breast-cancer-thinkstock-759.jpg",alt="neofetch" align="middle" height="200px">
  </p>





## Objective
Early cancer detection and prognosis is one of the most important healthcare areas where machine learning techniques are being applied.
The second leading cause of death among women is breast cancer, as it comes directly after lung cancer. More than one million cases and nearly 600,000 deaths occurring worldwide annually.
`The experiment aims to predict instances of breast mass collected as Malignant or Benign`.

## Data Description
Please click [here](Dataset/BreastCancer.csv) to view the dataset. 

This dataset consists of 573 samples & 32 features describing the characteristics of a cell nuclei taken from a digitized image of a breast mass.
1) ID number 2) Diagnosis (M = malignant, B = benign)
 3-32)  Ten real-valued features are computed for each cell nucleus:
* Radius: (mean of distances from center to points on the perimeter)
* Texture (standard deviation of gray-scale values) 
* Perimeter
* Area 
* Smoothness (local variation in radius lengths) 
* Compactness (perimeter^2 / area - 1.0) 
* Concavity (severity of concave portions of the contour) 
* Concave points (number of concave portions of the contour) 
* Symmetry 
* Fractal dimension ("coastline approximation" - 1)
The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.
Missing attribute values: Yes
##### Class distribution: `357 benign, 212 malignant`

Please have a gimpse of the dataset
![alt-txt]("Breast_Cancer_Images/Capture.PNG")




