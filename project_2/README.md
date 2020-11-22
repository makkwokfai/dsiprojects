# Project 2 - Ames Housing Data and Kaggle Challenge


## Problem Statement

The question is what is the predicted Sale Price of a house in Ames, IA.


## Summary

For this project, i am using the dataset for individual residential properties sold in Ames, IA from 2006 to 2010.

Using this dataset, we build a regression model to predict the selling prices of houses. For each Id in the test set, i will predict the value of the Sale Price based on these variables.


## Conclusion and Recommendation

Based on the numerical datas i am using, i have studied them and handled all the null values.

After that, i have handled all the Nominal and Ordinal datas. Based on the correlation i have identified, i have insert all my datas into 4 different model:
     1) Linear Regression
     2) Ridge CV
     3) Lasso CV
     4) ElasticNet CV
 
After checking the Adjusted R-Squared and Root-Mean-Squared-Error, i found that Lasso CV is the most suitable out of these 4.

Using Lasso CV, I have constructed a model by minimizing the data to 22 variables: 

SalePrice = 183260 + (15001 * Overall Qual) + (21031 * Gr Liv Area) + (9196 * Total Bsmt SF) + (5753 * Garage Area) + (2684 * Year Built) + (3509 * Year Remod/Add) + (7442 * Mas Vnr Area) + (3302 * Fireplaces) + (10195 * BsmtFin SF 1) + (4166 * Lot Frontage) + (5694 * Lot Area) - (6506 * Exter Qual) - (5762 * Kitchen Qual) - (3815 * Bsmt Qual) + (3273 * Exterior 1st_BrkFace) + (2508 * Exterior 1st_CemntBd) + (2362 * Neighborhood_Crawfor) + (2516 * Neighborhood_NoRidge) + (6739 * Neighborhood_NridgHt) + (7872 * Neighborhood_StoneBr) - (2213 * Mas Vnr Type_BrkCmn) - (4117 * Mas Vnr Type_BrkFace)