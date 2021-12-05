# King County House Sales Data Analysis Project
![KC](https://user-images.githubusercontent.com/74560236/112411481-9a0d6a00-8ce2-11eb-95a3-9f3aa482e987.jpg)

*Created by Andres Ramirez*

*Flatiron Data Science 011121 Cohort*

*March 26, 2021*

## Overview
* This project uses the King County House Sales dataset, which can be found in kc_house_data.csv in the data folder in this repo. The description of the column names can be found in column_names.md. For this project, I will use regression modeling to analyze house sales in a northwestern county.

## Business Problem
## Stakeholders
* The stakeholders in this project is Ramtuck Realty Group
## Consumer Use
* Ramtuck Realty group will use the results obtained from this project to help their clients who have made specific requests about the home they are looking for within King County.
## Data Understanding
* We will be focusing on price as our target variable since it is dependent on various features present on our dataset. Presented below is the outline and description of the columns present in our dataset.

### Column Names and descriptions for Kings County Data Set
* **id** - unique identifier for a house
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

## For our purposes we will be disregarding the following columns in the data

* **date**
* **id**


## Methods:
* This project utilizes descriptive statistics that help inform predictive modeling. The data is prepared through scrubbing and cleaning in order to prepare it for feature engineering and modeling. The data also underwent various tests to align with the assumptions of Linear Regression including identifying or rectifying instances of multicollinearity, normality, linearity heteroscedastiticty, homoescedasticity, skewness, kurtosis, and outliers. In order to accomplish this it was important to incorporate the concepts of ordinary least Squares, single linear regression, multiple linear regression, train-test-splits, correlation coefficients, mean absolute error, mean squared error, root mean squared error, cross validation, r squared, and log transformations.

## Results:
#### The biggest features affecting price when all other features held constant are:
* Grade of the home
* Square footage of the home not including the basement
* Square footage of the living space of the nearest 15 neighbors.

<img width="901" alt="Grade vs Price" src="https://user-images.githubusercontent.com/74560236/112909681-25a24480-90af-11eb-81c8-002a1a7c40de.png">

* This image is a density map that illustrates the effect of Grade vs Price. While there are of course outliers in our data we can state with confidence that as the grade of the home increases, the price increases, as evidenced by the darker orange and red areas. The reverse is also true and lower grade and price are reflected by lighter green areas.

## Conclusions:

* With a R-squared of 0.87, an MAE of 75,000 USD, and a RMSE averaging around 136,000 USD, our model seems to have significant predictive power. There is always additional room for model iteration and closer analysis of factors that may be limiting the quality of the model, its current levels promote an acceptable model when compared to our first model's values. The assumptions made in each test proved to be insightful regarding what features would positively or negatively impact the validity of our model. We are able to see with our final model some of the impacts that various features have on our target variable 'y' in order to better inform our stakeholders.

* For grade vs. price we were able to determine a coefficient of 0.0957, which leads to a change of 10.04% in price for every increment, while all other variables are held constant. For sqft above vs. price we were able to determine a coefficient of 0.1113, which leads to a change of 11.77% in price for every increment, while all other variables are held constant. For log of sqft_living15 vs. price we were able to determine a coefficient of 0.1579, which leads to a change of 17.10% in price for every increment, while all other variables are held constant. These were calculated by computing e^(coefficient).

* From our visualizations we can note that there are also price increases around economic hubs and city centers. As assumed, prices also increase with proximity to the waterfront as well. As we move further away from main cities such as Bellevue and Seattle, prices tend to decrease, while it is also important to note that there are outliers in the data regarding this point. High prices outside of the city can be accounted for by grade and lot size as they can be assumed to be large homes (i.e. mansions) with sizable land associated with them.

## Future Work:
* Future work that could be done would include optimizing our model with feature engineering, namely adding a feature that could help measure home prices based on their distance from major economic hubs or major locations of employment. Future work could also include optimizing the model to determine home cost based on its approximate location to main interstate and highways, since this can be an advantageous feature for some home buyers who wish to be far from the bustle of living within a major city, but relatively easy to access should they need to travel in.

* Another important consideration to make to future work can involve the impact that homes can be in a reliably modernized neighborhood. Features such as the presence or option for fiber optic internet connection, reliable satellite services and other modern amenities may play a great role in cost and attractiveness. This is an important feature as potential home buyers may already be or are considering working remotely from home, but may be limited by currently existing connection limits.


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
- Numpy

## Data Used:
- kc_house_data.csv 



## Featured Notebooks and Analysis
* [Presentation](https://docs.google.com/presentation/d/1ep6QVmJze2U1TrFiimT-Det1YxSy9ZiZHv4t833gqoA/edit?usp=sharing)
* [Jupyter Notebook](https://github.com/6cats1dog/KingCountyHomes/blob/main/King%20County%20House%20Sale%20Data%20Analysis.ipynb)
* [Jupyter Notebok PDF](https://github.com/6cats1dog/KingCountyHomes/blob/main/King%20County%20House%20Sale%20Data%20Analysis.pdf)
* [ReadMe](https://github.com/6cats1dog/KingCountyHomes/blob/main/README.md)
* [Presentation PDF](https://github.com/6cats1dog/KingCountyHomes/blob/main/Presentation%20for%20King%20County%20Home%20Sales%20by%20Andres%20Ramirez.pdf)
* [Data](https://github.com/6cats1dog/KingCountyHomes/blob/main/kc_house_data.csv)
