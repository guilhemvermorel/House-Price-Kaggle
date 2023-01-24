# House Prices - Advanced Regression Techniques

## Context
This project takes place with the objective of studying various regression techniques and their implementation. My teams and I have worked on a Kaggle project to determine the sales price of houses using only a few features about the residences. Kaggle project is available [here](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques), do not hesitate to try it by your side. 

## Versions 
`python` - `3.11.1` \
`numpy` - `1.24.1` \
`pandas` - `1.5.2` \
`pytorch` - `1.13.1` 

## Dataset
The dataset used consists of 1460 houses defined by characteristics, some of which are obviously correlated with its price, such as the number of rooms, and others which are not, such as the date of sale. It is available [here](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data).

## Models used
We have tried the following regressor techniques : SVR, Decision Tree Regressor, Ridge Regressor, Random Forest Regressor, Neural Network Regressor, Gradient Boostig, AdaBoost, XGBoost, Ensemble Regressor. 

## Results
All results, and so Kaggle rankings, have been made on March 2022. 

|Model | Training error (log MSE) | Kaggle score (log RMSE)  | Kaggle ranking |
| ------------- |:-------------:| ------:| ----:|
| Adaboost                  | 0.03838   | 0.2246 | 4112/4323|
| Decision Tree Regressor   | 0.21300   | 0.2083 | 3562/4323|
| Neural Network            | 0.00505   | 0.1885 | 3442/4323|
| Support Vector Regressor  | 0.01919   | 0.1516 | 2604/4323|
| Random Forest Regressor   | 0.00216   | 0.147  | 2317/4323|
| Ridge Regression          | 0.0126    | 0.142  | 1989/4323|
| XGBoost                   | 4.094e-12 | 0.1333 | 1365/4323|
| Gradient boosting         | 0.00010   | 0.1330 | 1355/4323|
| Ensemble Regressor        | 0.00260   | 0.1293 |  928/4323|


From the results we can see that the least successful models were Adaboost and the decision tree. Although Adaboost is an ensemble model, it does not seem to be the right one for the challenge. On the other hand, it is not surprising that the decision tree obtained such a low result because it is the simplest model used.

Another not successful model is the Neural Network which, although it is able to remember all the training values, suffers from overfitting. This does not allow it to achieve a better classification.

On the other hand, the support vector machine, although it is not able to achieve results of the ensemble methods, has better results than the previous models. Random forest gave a good result considering that is an ensemble method.

The best results were achieved by ensemble methods, mainly XGBoost and Gradient boosting which reduce variance and tend not to have overfitting by weak predictors. 

## Referencies
This project have been carried out by Rayan Ben Taleb, Jorge Gomez-Bravo Emilio Monroy and I during a class lesson named Advanced Data Mining at the school IMT Atlantique. Thanks a lot guys. 
