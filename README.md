# King County House Sales Data Analysis Project
*Andres Ramirez*

# Overview

This project uses the King County House Sales dataset, which can be found in kc_house_data.csv in the data folder in this repo. The description of the column names can be found in column_names.md. For this project, I will use regression modeling to analyze house sales in a northwestern county.

# Business Problem
## Stakeholders
* The stakeholders in this project is Ramtuck Realty Group
## Consumer Use
* Ramtuck Realty group will use the results obtained from this project to help their clients who have made specific requests about the home they are looking for within King County.
** Data Understanding
We will be focusing on price as our target variable since it is dependent on various features present on our dataset. Presented below is the outline and description of the columns present in our dataset.

** Column Names and descriptions for Kings County Data Set
* **id** - unique identified for a house
* **date** - house was sold
* **price** - is prediction target
* **bedrooms** Number of Bedrooms/House
* **bathrooms** Number of bathrooms/bedrooms
* **sqft_living** square - footage of the home
* **sqft_lotsquare** - footage of the lot
* **floors** Total - floors (levels) in house
* **waterfront** - House which has a view to a waterfront
* **view** - Has been viewed
* **condition** - How good the condition is ( Overall )
* **grade** - overall grade given to the housing unit, based on King County grading system
* **sqft_above** - square footage of house apart from basement
* **sqft_basement** - square footage of the basement
* **yr_built** - Built Year
* **yr_renovated** - Year when house was renovated
* **zipcode** - zip
* **lat** - Latitude coordinate
* **long** - Longitude coordinate
* **sqft_living15** - The square footage of interior housing living space for the nearest 15 neighbors
* **sqft_lot15** - The square footage of the land lots of the nearest 15 neighbors

## For our purposes we will be disregarging the following columns in the data

* **date**
* **id**


## Methods:
* This project utlizises decriptive statistics that haelp inform predicitive modeling. The data is prepared through srubbing cleaningnin order to prepare it for feature engineering and modeling. The data also underwent various tests to align with the assumptions of Linear Regression including identifying or rectifying instances of multicollinearity, normality, linearity heterscedastiticty, homoescedasticity, skewness, kurtosis, and outliers.  In order to accomplish this it was important to incorporate the concepts of orinary least Squares, single linear regression, multiple linear regression, train-test-splits, correlation coefficients, mean absolute error, mean squared error, root mean squared error, cross validation, r squared, and log transformations

## Technologies:
- Python
- Matplotlib
- Seaborn
- Scikit Learn
- Scipy-stats
- Statsmodels
- Pandas
- Jupyter Notebook
- Google Slides
-Numpy

## Data Used:
-kc_house_data.csv 



## Featured Notebooks and Analysis
