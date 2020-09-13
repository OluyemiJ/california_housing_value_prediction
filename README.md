# california_housing_value_prediction

# Project Overview
* Created a tool that estimates house value in california to help real estate practitioners or potential house buyers negotiate better. 
* Explored data to gain initail insights into correlations
* Encoded categorical data using on-hot encoding
* Optimised Linear, Decision Tree and Random Forest Regressors using GridsearchCV to reach the best model. 
* Tested best model on test set to determine performance

## Code and Reources Used
This work was inspired by Aurelien Geron's Hands-On Machine-Learning with Scikit-Learn, Keras and TensorFlow book (Chapter 2) - https://www.oreilly.com/library/view/hands-on-machine-learning/9781491962282/

**Python Version:** 3.8
**Packages:** pandas, numpy, sklearn, matplotlib, six.moves, seaborn

##EDA
Looked at the spread of the observation of the features to understand the kinds of distributions involved. Explored correlations. Here are some plots from the EDA:

![alt text](https://github.com/OluyemiJ/california_housing_value_prediction/blob/master/scatter_values.png "Housing Values by Geography")
![alt text](https://github.com/OluyemiJ/california_housing_value_prediction/blob/master/correlation_heat_map_values.png "Correlation")
![alt text](https://github.com/OluyemiJ/california_housing_value_prediction/blob/master/scatter_matrix.png "Scatter Matrix")

##Model building and performance
Built transformers and combined them in a pipeline to transform the data sets. Tried three models - Linear, Decision Tree and Random Forest Regressors. Carried a 10 fold corss-validation on the training set in order to select the best model. The models performed on validation as follows:

**Linear:** RMSE = 69050.88
**Decision Tree:** RMSE = 70794.37
**Random Forest:** RMSE = 50078.05

Random Forest Regressors turned out best based on the validation process and so I tuned it:

**Random Forest:** Best Params = {'max_features': 6, 'n_estimators': 30}

Performance on test set:

**Random Forest:** RMSE = 46491.44
