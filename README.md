
# Module 2 Final Project


## Introduction

1. EDA + Model1: This contains all the data scrubbing performed for the first model as well as handling outliers and checking assumptions of regression. 

2. Model 2: This model predicts using only numerical values that are logged to standardize distribution. Distributions were not equal and i wanted to test the impact of this on results.

3. Model 3: This model predicts using numerical values that have been scrubbed like previous files but does not have log functions. 

4. Model 5: The final and best performing model combines years binned with encoded grade variables


## Data Cleaning and Preparation

    Outliers are dropped
    NaN are imputed or dropped
    The final model has binned ages
    
# What is the Best Performing Model ?

Model 5 performs with the highest r squared score but has significantly high kurtosis and has a high MSE. Model 3 has a low r squared score but a very low mean squared error. I noticed that the noise of too many data points was likely impacting the model so i approached key variables with strategically thought out manipulations that would enable them to be part of the model but have their contribution to the result be realistic. 

# What features matter the most?

This was done through inference of trial and error performing OLS on numerous selections of variables and checking the results. While much more work can be done on this, it seems that 'bedrooms', 'bathrooms', 'sqft_living', 'floors','yr_built','sqft_living15', 'sqft_lot15' are important factors in calculating this relationship. 

# What variables were colinear?

Some of the sqft variables were highly collinear and therefore sqft living is the most important of this. Grade is also a very important categorical variable that seems to capture quality that requires further investigation. 


# Conclusion

We started with a lot of features and ended with very few indicating that high correlation between features. I attempted to simplify this into a model that requires only a few variables but produces a quality r2 scored. The final model is not production ready and will not predict with an accuracy level deemed safe. However, knowing the variables that influence score can better inform agents at what drives price and help guide them in their future pricing decisions on homes that are selling!
