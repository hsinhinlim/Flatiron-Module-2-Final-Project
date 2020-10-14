# Flatiron Module 2 Final Project

## Objective
We attempt to apply multivariate linear regression on a dataset of residential properties located in King County, Washington in order to predict their sale price. Our business case assumes we are providing advice to a firm of real estate agents who wish to break into the residential property market in King County. Because they have no idea where to start negotiations between buyers and sellers on properties in King County they may be instructed to sell, the **primary objective** of this project is to build a simple 3 feature model which will generate a benchmark price around which negotiations can happen. 

As a **secondary objective**, the project attempts to harness the data for intelligence about the residential landscape which may be useful to these real estate agents (who, remember, have never been to King County). For instance, where the old neighbourhoods are and where the high quality housing is located in King County.

## Approach
We will attempt to achieve the **primary objective** in 3 steps:

1) **Exploratory Data Analysis** - In this step we will look at the entire data set, remove null values, convert data into numerical datatypes, investigate correlations between the data and (crucially) come to a view as to whether certain data is continuous or categorical. Looking at the correlations between the data (and between each independent variable and the dependent variable **price**) will provide initial clues as to which of the independent variables will be good predictors. We will also focus on the distribution of the dependent variable **price** and on the distribution of the independent variables in the dataset. This focus is designed to remove outlier values (of both the dependent and independent variables) which may interfere in the interpretation of any model.

2) **Feature Selection** - Having investigated and cleaned the data in the prior step, we will use a forward selection method to test multiple models to find the 3 features that will give rise to a 3 feature model with the highest **r-squared**. In this step we also take a closer at the features selected and analyse, crucially, whether their residuals are normally distributed.

3) **Assessing model accuracy** - Once we have ascertained that our 3 feature model meets the assumptions of linear regression, we can test the degree of accuracy of the model by analysing the mean error between the price predicted by the model and the actual price data. This will give a sense of the limitations of the model, where the limitations occur and the range of values the actual price of the property can take on away from the benchmark predictions made by the model.

Finally, after having identified 3 relevant features - we will attempt to achieve the **secondary objective** by using each feature as the basis for asking meaningful questions about the data from the perspective of a firm of real estate agents who are new to King County.

## Contents
This repository contains:
1) a Jupyter Notebook (student.ipynb) which contains the EDA and actual analysis undertaken to reach certain conclusions and recommendations;
2) a pdf of a slide presentation (presentation.pdf), setting out the conclusions and recommendations to a non-technical audience;
3) the dataset of King County housing data (kc_house_data.csv); and
4) a geojson file (zip_codes.geojson) setting out the polygon shapes of various King County zipcodes which are in the dataset. This is used to draw the choropleth map in the Jupyter notebook

## Usage
Clone the repository and run the Jupyter Notebook

## Other materials
I blogged about this project here: https://medium.com/@hsinhinlim/the-map-is-not-the-territory-5024531c9556
There is a YouTube video of a non-technical walkthrough of the slide presentation here: https://www.youtube.com/watch?v=IK5ThKrqTtg
