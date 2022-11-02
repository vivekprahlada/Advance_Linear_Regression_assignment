# House price prediction using regularized linear regression method
Surprise housing firm wants to predict the house prices to support their business of purchase, rennovate and sell. They want to buy the properties at lower price and sell it at profit. ML method to be used to predict the house proce given the predictors and historical data


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.

- Project background: As part of the project, regularized linear regression method of Ridge and Lasso are used to derive the coefficients and therefore predict the house prices while also understand the impact of the predictors on the house sale price
- 
- Business problem: Company "Surprise Housing" wants to enter Australian market. Their business model is to buy houses at lesser price renovate and sell it to higher prices. They have collected some attributes and housing price to understand how the attributes influence the housing price and also to predict the house price given the attributes. Therefore it is important to have a generalized model where the influence of the attributes can be explained clearly (having model with correlated attributes) and prediction of the house prices can be made with good accuracy. Outcome of the model shall be used by management for further buisness adjustments

- Dataset: A dataset "train.csv" was provided with 1460 data points and 80 predictors

## Conclusions
- Regression results

    -Ridge regression results

    ++++++++++++++++++++++++++++

        -Train R2 score = 0.8613

        -Test R2 score  = 0.8611

        -Optimal lambda = 50


    -Lasso regression results

    ++++++++++++++++++++++++

        -Train R2 score = 0.8471

        -Test R2 score  = 0.8478

        -Optimal lambda = 500

- Ridge regression is preferred for prediction due to better R2 score
- Lasso regression to explain the predictor influence
- Lasso regression concludes total of 53 relevant predictors (including dummies) which are below and are aranged in the order of their highest influence

    ['Neighborhood_NWAmes', '1stFlrSF', 'Neighborhood_NoRidge', 'HeatingQC', 'MiscFeature_TenC', 'LotArea', 'HouseStyle_1.5Unf', 'Condition1_Feedr', 'Neighborhood_Crawfor', 'BsmtExposure_Mn', 'ExterCond', 'FireplaceQu', 'KitchenAbvGr', 'MSZoning_RL', 'SaleType_ConLw', 'BsmtFinType1_Rec', 'YearRemodAdd', 'MasVnrType_BrkFace', 'OverallQual', 'MasVnrArea', 'LowQualFinSF', 'BedroomAbvGr', 'GarageFinish_No Garage', 'MSSubClass_120', 'LotFrontage', 'Utilities_NoSeWa', 'MSSubClass_90', 'KitchenQual', 'GarageQual', 'Fireplaces', 'GarageFinish_RFn', 'BldgType_Twnhs', 'OverallCond', 'Neighborhood_CollgCr', 'BsmtHalfBath', 'BsmtQual', 'BsmtFinType1_BLQ', 'GarageCond', 'TotRmsAbvGrd', 'EnclosedPorch', 'FullBath', 'BsmtUnfSF', '3SsnPorch', 'HouseStyle_SLvl', 'Exterior2nd_Stucco', 'ScreenPorch', 'BsmtFinType2_Unf', 'HouseStyle_2.5Unf', 'BsmtCond', 'Neighborhood_SawyerW', 'BsmtFullBath', 'Exterior1st_BrkComm', 'GarageCars']
    

- Residual error terms are checked for assumption confirmation. Error term normality is confirmed but constant variance is not ideal visually. Any non-linear relationship could be checked if needed

## Technologies Used
- Jupyter notebook version 6.4.8
- Python 3.9.12
- IPython 8.2.0
- NumPy 1.21.5
- Pandas 1.4.2
- Matplotlib 3.5.1
- Seaborn 0.11.12
- sklearn 1.0.2


## Acknowledgements
- This project was based on UpGrad assignment

## Contact
Created by [@vivekprahlada] - feel free to contact me!
