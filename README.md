# ML-Capstone-Regression-Project-Seoul-Bike-Sharing-Demand-Prediction
## Objective:
I have Seoul Bike Sharing Demand Prediction dataset. The main objective of this project is to accurately predict the demand for rental bikes in urban areas to ensure a stable supply, thereby minimizing waiting times and enhancing overall mobility comfort for the public. This involves developing a model that forecasts the required bike count at different hours of the day.
## Dataset :
The given dataset have information of rented bike count. The dataset have 8760 rows and 14 columns. The columns from the dataset is as follows:

* **Date** : Date on which bike rented.
  
* **Rented Bike Count** : Count of Bike Rented.
  
* **Hour** : Hour of the day (0-23).
  
* **Temperature** : Temprature of the day in celcius.
  
* **Humidity** : Humidity of the day in percentage.
  
* **Wind Speed** : Speed of wind in m/s.
  
* **Visibility** : Visibility Measure 10m.
  
* **Dew Point Temprature** : Dew Point Temprature measure in degree celcius.
  
* **Solar radiation** : Solar radiation measure in MJ/m2.
  
* **Rainfall** : Rainfall in mm.
  
* **Snowfall** : Snowfall measure in cm.
  
* **Seasons** : Spring, Summer, Fall, Winter.
  
* **Holidays** : Whether a holiday or not.
  
* **Functional** : Whether a functional day or not.

## Data Cleaning and Manipulation:
## **Duplicate Values**
Dataset do not have any duplicate and null values.

## EDA:
The EDA and visualization is done by using scatterplot, barplot, histlpot, heatmap, pairplot etc.
In EDA I tried to find out answers of some question. The questions are as follows:
1. What is the distribution of the 'Rented Bike Count?
2. How does the distribution of 'Rented Bike Count' vary throughout the days in the dataset?
3. How does 'Temperature(°C)' affect 'Rented Bike Count'?
4. How do 'Seasons' affect 'Rented Bike Count'?
5. How does 'Wind speed (m/s)' affect 'Rented Bike Count'?
6. How do 'Holiday' affect 'Rented Bike Count'?
7. How does visibility ('Visibility (10m)') influence bike rental count?
8. Is there any noticeable relationship between dew point temperature ('Dew point temperature(°C)') and rented bike count?
9. How does the functioning day ('Functioning Day') affect bike rental demand?

## Hypothesis Testing:
Based on EDA charts, I defined three hypothetical statments from the dataset. Performed hypothetical testing and calculated P-Value using statistical tests. I this project I used following statistical tests :
1. T-Statistical test
2. F_statistical test

## Feature Engineering and Data Pre-processing:
Here I did following steps:
1. Handling Missing Values
2. Handling Outliers
3. Removing Outliers
4. Categorical Encoding
5. Checking and Removing Multicollinearity
6. Check correlation between independent and dependent variables
7. Feature Transformation
8. Apply test and train split
9. Feature Scalling:

## ML Model Implementation:
In this project I implemented following regression models:

Linear Regression
Ridge Regression
Lasso Regression
Elastic Net Regression

# Model Explainability:
Here I used SHAP library.

# Conclusion
1. EDA insights:

* There's a rise in bike rentals during 2018 compared to 2017, with noticeable drops in rentals during 2017, suggesting increased popularity or intensified marketing efforts from early 2018 onwards.

* Bike rental demand is high in warm weather condition and low in mild condition.

* The rented bike count is highest in the summer season, followed by autumn and then spring. The rented bike count is lowest in the winter season.

* when the wind speed is low then the rented bike count is hight and when wind speed is maximum then the bike count is less.

* When there is a holiday then the bike count is very less and when there is no holiday then the rent bike count is very high.

* Better visibility conditions are associated with higher bike rental counts.

* When dew point temperature is maximum then the count of the rented bike is maximum and when temperature is minimum then count is also minimum.

* On a functioning day the rent bike count is high and when there is no functioning day then the rented bike count is zero.

* Rented bike count has a strong positive correlation with temperature (0.54), meaning higher temperatures are associated with more bike rentals.

2. Machine Learning Model:

* Based on these metrics:

* Linear Regression, Ridge Regression, and Lasso Regression have very similar performance across all metrics.

* Elastic Net Regression performs slightly worse compared to the other models, with a higher MAE, MSE, and lower R2 Score.

* Considering the similarity in performance between Linear Regression, Ridge Regression, and Lasso Regression, either of these models can be considered the best choice for this dataset. However, Elastic Net Regression may not be the preferred choice in this case due to slightly poorer performance.

* All 4 models have been explained with the help of SHAP library.

* Temperature and Hour are the two most important factors according to all the models.

3. Challenges:

* Handling outliers to avoid their impact on predictions.
* Converting categorical variables into numerical representations.
* Managing multicollinearity among predictor variables.
* Choosing an easy-to-understand technique to explain model predictions.
