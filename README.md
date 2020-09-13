# california_housing_value_prediction

# Project Overview
* Created a tool that estimates house value in california to help real estate practitioners or potential house buyers negotiate better. 
* Explored data to gain initail insights into correlations
* Encoded categorical data using on-hot encoding
* Optimised Linear, Decision Tree and Random Forest Regressors using GridsearchCV to reach the best model. 
* Tested best model on test set to determine performance

## Code and Reources Used
This work was inspired by Aurelien Geron's Hands-On Machine-Learning with Scikit-Learn, Keras and TensorFlow book (Chapter 2) - https://www.oreilly.com/library/view/hands-on-machine-learning/9781491962282/
**Python Version:* 3.8
**Packages:** pandas, numpy, sklearn, matplotlib, six.moves, seaborn

##EDA
Looked at the spread of the observation of the features to understand the kinds of distributions involved. Explored correlations. Here are some plots from the EDA:

![alt text](https://github.com/OluyemiJ/california_housing_value_prediction/blob/master/scatter_values.png "Housing Values by Geography")
![alt text](https://github.com/OluyemiJ/california_housing_value_prediction/blob/master/correlation_heat_map_values.png "Correlation")
![alt text](https://github.com/OluyemiJ/california_housing_value_prediction/blob/master/scatter_matrix.png "Scatter Matrix")
