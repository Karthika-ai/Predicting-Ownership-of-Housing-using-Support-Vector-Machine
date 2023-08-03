# Predicting-Ownership-of-Housing-using-Support-Vector-Machine
The project uses Support Vector Machine to predict if a residence is occupied by owners or tenants based on information retrieved about the occupants and the property using the U.S census for social, economic and health research IPSUMS data

## Software
R Studio

## Packages
`library(tidyverse)`
`library(e1071)`
`library(dplyr)`
`library(caret)`
`library(ggplot2)`
`library(tictoc)`
`library(pROC)`

## Getting Started
Data Preprocessing
    - Converting data types
    - Imputing missing values
    - Feature Selection
    
## Methods
SVM with
    - Linear Kernel
    - Radial Kernel
    - Polynomial Kernel

## Key Findings
- The annual income of the individuals is one of the strong predictors used in determining the type of occupants residing in the house. From the plots we could infer that the individuals with annual income more than $700,000 own a house with more than three rooms in any local area. This analysis reveals that certain socioeconomic groups are less likely to own homes which can be less stable and more expensive.
- Policymakers could use this information to educate and start counseling programs related to homeownership. This is also done to target affordable housing programs, such as increasing funding for down payment assistance, providing tax incentives for developers to build affordable housing.

## Results
It was identified from the project that the annual income, density of local population and number of rooms are the strongly correlated variables to classify the type of occupants. The hyperplanes separated the feature space into two classes even though the data points were not well separated. Of the three models used, the tuned hyper parameter model using a polynomial kernel with a degree 3 and cost of 5 was able to predict the “renter” class at 85%, “owner” class at 69% and overall accuracy of 78%. The computational time for the model to train using the polynomial kernel was 40.8 sec. As a future proposition to obtain better results, the model should be trained on the equal number of observations for each class.

## Reference
James, G., Witten, D., Hastie, T., & Tibshirani, R. (n.d.).An Introduction to Statistical Learning. Retrieved April 26, 2023, from https://www.statlearning.com/

