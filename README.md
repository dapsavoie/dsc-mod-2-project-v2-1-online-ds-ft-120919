
# Module 2 Final Project


## Introduction

    1. EDA + Model1: This contains all the data scrubbing performed for the first model as well as handling outliers and checking assumptions of regression. 

    2. Model2: This model predicts using only numerical values that are logged to standardize distribution. Distributions were not equal and i wanted to test the impact of this on results.

    3. Model3: This model predicts using numerical values that have been scrubbed like previous files but does not have log functions. 


## Data Cleaning and Preparation

    Outliers are dropped
    NaN are imputed or dropped
    
    
# What is the Best Performing Model ?

Model 1 performs with the highest r squared score but has significantly high kurtosis and has a high MSE. Model 3 has a low r squared score but a very low mean squared error. 

# What features matter the most?

This was done through inference of trial and error performing OLS on numerous selections of variables and checking the results. While much more work can be done on this, it seems that 'bedrooms', 'bathrooms', 'sqft_living', 'floors','yr_built','sqft_living15', 'sqft_lot15' are important factors in calculating this relationship. 

# What variables were colinear?

Some of the sqft variables were highly collinear and therefore sqft living is the most important of this. Grade is also a very important categorical variable that seems to capture quality that requires further investigation. 


# Conclusion

We started with a lot of features and ended with very few indicating that high correlation between features. I attempted to simplify this into a model that requires only a few variables but produces a quality r2 scored. 