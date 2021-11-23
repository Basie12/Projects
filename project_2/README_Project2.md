# GA DSI:  Project Two
## Ames Housing Project Suggestions

> ### Name Basazin Belhu

## Purpose:
This project is focus on develop a machine learning model that able to extract the different criteria that play a big role in determining the hous price. It also optimize sales based specifying some feature of  the future house. It will guess the price of the house as accurate possible depending on the information feed from the real state. 
- Want to know which criteria has main impact on determine the house price
- Create a multi linear regression to predict the price of the hase based on the selected features
- They want to know how well the model predict the price.

## Methods Used

#### EDA 
- Import the training and testing datasets
- Determine _what_ missing values mean.
- Figure out what each categorical value represents.
- Consider whether discrete values are better represented as categorical or continuous.
- Decide how to impute null values.
- Drop columns filled mostly with NaN

#### Exploratory Visualizations and Feature Engineering
- Distributions and correlations.
- Check features relationships to target
- Combine any features
- Do you want to manually drop collinear features
- Match the testing dummy columns with traing dummy columns

#### Modeling and Metrics
- Train test split
- Fit the model
- Baseline, Linear Regression, Lasso and GridSearch
- Eval the model, R2, RMSE 
- Check assumptions 

## Technologies
- Python3
- GitHub
- Pandas,Numpy, Matplotlib, Seaborn, jupyter lab, Scikit-learn

##  Data
The data for this model very complaex as it has a lot of null values and many columns. The raw data consists of a training dataset with the features listed in the data dictionary in the following link. The traing data of this training dataset was split into a testing and training dataset to traing the model with corresponding house price. 

There is a testing dataset that does not contain the sale price columns information and was used as a substitute for unseen data to test the performance of the model.

Data dictionary here  https://www.kaggle.com/c/dsi-us-12-project-2-regression-challenge/data

## Challenges

- Selecting the important features and create a visualization for column very challenging sisnce there are many columns.
- Cobined all the analysis and visualization to make concise summary
## Summary
There are four model trained to predicth the h
Applying the standard scaling and grid search to the features and lasso regression gave me the most accurate predictions with the least error when using a this lasso regression model. The result modelhase Train RMSE: `$`26842 dollars and Test RMSE: `$`26972 dollars with a 88% accuracy rate.

This model can be used as a guide when determining house price since it shows pretty good predictions when given informations have higher coefficients, like the Gr live area and Kictchen quality.
## Conclusion and Recommendation
The most valuable feature in this project  the Kichetchen Qulaity, Nieghborhood and GrLIvArea while Electrical_FuseA least valuable features based on their lasso and gridsearch model coefficinets.

The Lasso model for predict the house price  based on different features. I has a features that explained the 88% variability in target value. I have used the baseline, linear regeression and lasso to predict the house, except the baseline model all the models have similar significance and accuracy.

**Recomendation:** In the future, I would add more feature interaction, add some columns such as school zone  and transform my target values to improve th R2 value and reducs the RMSE