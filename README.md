
Complete project report 

Worked on going threw various location House Price Data and extract data relevant data based on master list . Worked in target Driven environment . Ensured that the data extracted is accurate and does not contain any error. 


	
	




HOUSE PRICE PREDICTION USING VARIOUS REGRESSION:
A COMPARATIVE STUDY



AJAY SHUKLA   |  Applied  DATA SCIENCE   |   22/August/2021
       aksamiliya@gmail.com
	 
		Introduction

There are a number of factors which determine property prices, some are logical, based on economic theories and population density and some are based on more intangible factors, like availability of amenities & necessities, neighborhood, etc.

Objective: Build a linear regression model to predict the price of the property from the dataset having attributes such as sale type, sale condition etc. Use Linear Regression and RandomForest algorithm & compare the performance

Dataset:Source (https://www.kaggle.com/anmolkumar/house-price-prediction-challenge)

The real estate sector is an important industry with many stakeholders ranging from regulatory bodies to private companies and investors. Among these stakeholders, there is a high demand for a better understanding of the industry operational mechanism and driving factors.
Today there is a large amount of data available on relevant statistics as well as on additional contextual factors, and it is natural to try to make use of these in order to improve our understanding of the industry. Notably, this has been done in PROJECT work  on housing prices 
In some cases, non-traditional variables have proved to be useful predictors of real estate trends. For example, in  it is observed that Seattle apartments close to specialty food stores such as Whole Foods experienced a higher increase in value than average.
This project can be considered as a further step towards more evidence-based decision making for the benefit of these stakeholders. The project focused on assessment value for residential properties in Calgary between 2017-2020 based on data from . The aim of our project was to build a predictive model for change in house prices in the year 2021 based on certain time and geography dependent variables. The main steps in our research were the following.
Data Description:
   Train.csv - 29451 rows x 12 columns
   Test.csv - 68720 rows x 11 columns
   Sample Submission - Acceptable submission format. (.csv/.xlsx file with 68720 rows)






Feature Selection/Attributes Description:
Column	Description
POSTED_BY	Category marking who has listed the property
UNDER_CONSTRUCTION	Under Construction or Not
RERA	Rera approved or Not
BHK_NO	Number of Rooms
BHKORRK	Type of property
SQUARE_FT	Total area of the house in square feet
READYTOMOVE	Category marking Ready to move or Not
RESALE	Category marking Resale or not
ADDRESS	Address of the property
LONGITUDE	Longitude of the property
LATITUDE	Latitude of the property



•	Modeling 
prediction using X_train with trained model so as to compare true price and predicted price made by our Linear regression , RandomForest model for prediction of the percentage change of the housing prices.
1
•	Exploration of reasons for misclassification in model
We then go back to the original data to find out why some samples are misclassified by our model.
In this report, we describe our approach to these steps and the results that we obtained.
Exploratory Data Analysis

By conducting explanatory data analysis, we obtain a better understanding of our data. This yields insights that can be helpful later when building a model, as well as insights that are independently interesting.

In order to understand our data, we first perform exploratory data analysis. This will provide us with insights that will be useful in building prediction models, as well as insights that may be of interest to stakeholders. As part of the Exploratory Data Analysis we aim to:
•	Look into the relationship between each variables and annual house price percentage change, and identify any patterns. For example, between the year of construction of a house and its annual percent price change.
•	We will also analyse relationships between the features. This may reveal that certain features are redundant and this would help the subsequent analysis.

Methodology

3.1. Feature selection. Our data has 11 features in total. If we use all of them in our prediction model, the model will have a risk of overfitting. Therefore, we decide to remove some unimportant features. We choose a LinearRegression, RandomForest algorithm called Supervise learning as the method to estimate how many components are needed to describe the data. The optimal number of features for the prediction can be determined by looking at the cumulative explained variance ratio as a function of the number of components.
This curve quantifies how much of the total, 8-dimensional variance is contained within the first n components. For example, we see that with the digits the first 5 components contain approximately 90% of the variance, while you need around 3 components to describe close to 100% of the variance.

	

Summary

By analysing historical data for house prices in Calgary along with various relevant features, we established some interesting patterns and trends. Using machine learning techniques, we were then able to identify a subset of the original features that are in a sense sufficient to describe our data.
Having selected the most important features, we then trained an Linear regression , RandomForest model for change in house price prediction, which classified samples into one of four categories. This model gave an accuracy rate of LR-72.53258347996879 , RF-0.9478940508689822
 on a test set that we had kept separate during development. This model can therefore be used to predict, for example, which type of house within Calgary is likely to increase and decrease in price in the year 2021 based on various scenarios.
                              Acknowledgements

We would like to express our deep and sincere gratitude to EICT-IIT Roorkee for giving us the opportunity to do this project. As a great bridge between academic and industry, this program educated us how to perform theoretical methodology in real life.
We would like to express our sincere thankfulness to Sanjay Agrawal and Abhishek Mishra for the continuous support of our research, for their patience, enthusiasm, motivation and immense knowledge. As our academic mentor, Sanjay Agrawal gave a lot active feedback on every step of the research. As industrial mentor, Sanjay Agrawal was dedicated to instructing us to get a realistic meaningful model. Both of them kept reminding us of the importance of collaboration, which ensured that the whole project proceeded smoothly.
Additionally, we would also like to thank all our friends who offered us some help, such as Stephen Styles who helped us build the misclassific 
