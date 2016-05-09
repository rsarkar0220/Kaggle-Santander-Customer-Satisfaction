# Kaggle-Santander-Customer-Satisfaction

I will add python codes that I wrote to predict the probability that a customer of Santander Bank is unhappy with the bank.

Challenges:
Both the training and the test datsets are heavily unbalanced, with over 95% of the users classified as happy.
The features are anonymized, and it is therefore, difficult to apply intuitive feature engineering.
A number of features have values [0, 1, ~10^10]. There are a myriad of ways in which these features may be handled. One is to consider 10^10 as missing data. The other is to consider that these are error codes, and the feature is categorical.

I used several different models:
Random Forests
Extreme Gradient Boosting (both sklearn and XGBoost)
Extra Trees Classifiers

I applied Hyperopt to find the best hyper-parameters for each of these. Finally, I blended these models together to derive my best predictions.

Here, I have only shown the general approach I applied using XGBoost.


Data:
The data files can be downloaded from Kaggle here https://www.kaggle.com/c/santander-customer-satisfaction/data
