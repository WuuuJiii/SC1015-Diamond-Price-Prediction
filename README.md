# SC1015 Data Science and Artificial Intelligence Project : Diamond Price Prediction

<p align="center">
  <img src="Dataset/diamonds.jpg" alt="Diamond Picture" width="800"/>
</p>


## About This Project ##
This is a course project for the SC1015 (Introduction to Data Science and Artificial Intelligence) offered by the Nanyang Technological University, Singapore  during the AY22/23 Semester 2.
 
We will be focusing on a diamond price predictor in this project.

Here is the walkthrough of our project.

1. Data Collection, Data Cleaning, Exploratory Data Analysis and Visualization : [Mini Project - Sample Collection, Data Cleaning + EDA](https://github.com/jjiunnbeh/SC1015/blob/6a172eebf5bf4492a97442129cdae6ba3c1eedca/Mini%20Project%20-%20Sample%20Collection,%20Data%20Cleaning%20+%20EDA.ipynb)
2. Model Building and Machine Learning: [Mini Project - Machine Learning](https://github.com/jjiunnbeh/SC1015/blob/6a172eebf5bf4492a97442129cdae6ba3c1eedca/Mini%20Project%20-%20Machine%20Learning.ipynb)

This project includes 2 notebooks, which cover all the walkthrough mentioned above.
## Problem Formulation ##

#### Practical Motivation ####

Nowadays, people have limited knowledge about the prices of diamonds and diamond sellers capitalise on this by selling diamonds with unfair and unreasonable prices.

Thus, this project can help diamond buyers to estimate the price of the diamond using the attributes that best predict the price of a diamond.The diamond industry is highly competitive and relies on accurate and timely pricing information. The prices of diamonds depend on various factors such as carat weight, cut, clarity, and colour, making it challenging to accurately predict the price. 

The objective of this project is to develop a machine learning model that can predict the price of diamonds based on their attributes for the diamond buyers. The model should be able to accurately predict diamond prices, considering multiple factors and providing an objective and consistent pricing strategy.


Problem Definition: Our group is set out to explore the prediction of diamond price based on the attributes of the diamond(carat, colour, clarity, cut , depth and table). 

Sub-problem: How does the attributes help to decide the price of diamonds in the market?

We are planning to create a diamond price predictor for the general customers to use as well.

Our dataset is extracted from [Kaggle: Diamond Prices](https://www.kaggle.com/datasets/nancyalaswad90/diamonds-prices), the dataset can be found [here](https://github.com/jjiunnbeh/SC1015_C133_Team2/blob/5b9867094d690015a24ad3ac25284e4cc32fb072/Dataset/Diamonds%20Prices2022.csv).



## The available features in our data set are: ##


PRICE : Diamond price in USD

CARAT : Weight of the diamond (1 carat equals 0.2 grams).

CUT : Quality of the cut (Ideal, Premium, Very Good, Good, Fair).

COLOR : Diamond colour, from D (Best) to J (Worst).

CLARITY : Measurement of how clear the diamond is (IF (Best), VVS1, VVS2, VS1, VS2, SI1, SI2, I1 (Worst)).

DEPTH% : Measure of the depth in relation to the width of the diamond’s table, calculated as --> Depth (%) = Depth (mm) / Diameter (mm)

TABLE : Top facet of the stone; table percentage is the ratio between the table size and the diameter of the diamond

X : Length in mm

Y : Width in mm

Z : Depth in mm
 
## Models Used ##
1. Linear Regression
2. Random Forest Regression (3 versions) with hyperparameter tuning
3. XGBoost Regressions (3 versions) with hyperparameter tuning

## Conclusion ##
In conclusion, we have faced different limitations thorughout the preparation of this project. The large dataset used in this project is difficult to observe in detail. Hence, with the proper use of different graphs and plots, the details can be clearly understood such as the spread of data, trend of data and relationship between the variables. Beside, the dataset contains a lot of categorical data, which limits the implementation of regression in the training process. By implementing label encoding, the categorical data is converted to numerical data, which can be used in the regression model as well. 

Based on different performace metrics(RMSE and R^2) to predict the accuracy of our models, we found out that Random Forest Regression (V3) is the most accurate model which can predict the price of diamond. 

The customers who are purchasing diamonds will be able to use the UI developed based on our best machine learning model to predict the price of diamonds they are going to purchase and determine if the price set by the diamond sellers are similar to the price predicted. 

Thus, we can avoid customers overpaying for diamonds. With that, we believe that our project has somewhat developed a solution which can be used in partical terms.

For the future improvement, exploration of more hyperparameters in the regression model is importatnt to further optimize the training model performance. More predictors such as the dimension of diamond should be included in the training process if the information about the predictors are more readily accessible to the customer in the future. In reality, the dataset might be too clean with very little outliers and null values which might have made our machine learning prcocesses slightly easier. 

## What did we learn? ##
- How to use github to collaborate with other peers in a team project
- Solve real world problems using proper real world related dataset
- Use of Label Encoding to convert ordinal data of categorical variables into numeric values
- Perform regression model which is not covered in class (XGBoost)
- Proper tuning of hyperparameter to avoid overfitting or underfitting
- Program a User Interface (UI) to easily estimate the diamond price

## Contributors ##
| Name              |                    Contributions                     |
|---|:---:|
|Selvakumar Karthik Adharsh | Label Encoding,Linear and Random Forest Regression, Presentation Slides, Video Presentation |
| Beh Jia Jiunn | Data Preparation, Exploratory Data Analysis, Presentation Slides, Video Presentation |      
|  Tan Wu Ji |   XGBOOST Regression, Prediction UI, Presentation Slides, Video Presentation |

## References ##

1. Source:                  https://www.globenewswire.com/news-release/2014/12/09/689825/10111532/en/NEW-STUDY-Americans-Overpaying-by-as-Much-as-72-for-an-Engagement-Ring.html
2. Kaggle : Diamond Prices: https://www.kaggle.com/datasets/nancyalaswad90/diamonds-prices
3. Diamond 4C's:            https://shira-diamonds.com/about/education/4-cs/ 
4. Diamond Colour:          https://4cs.gia.edu/en-us/diamond-color/
5. Diamond Clarity:         https://www.onlinediamondbuyingadvice.com/diamond-education/diamond-clarity/
6. Diamond Report:          https://bnsec.bluenile.com/bnsecure/certs/LD13571559/GIA?country=USA&language=en-us
7. Random Forest:           https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
8. XGBOOST:                 https://www.geeksforgeeks.org/xgboost/?ref=rp





