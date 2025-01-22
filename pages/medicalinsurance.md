# Predicting Medical Insurance Costs Using Multiple Linear Regression

This project was created by myself, Bobbi Boyce, Stephen Bonsu, Kennedy Gunderson and  Noah Seminoff. All of the analysis was completed using R and statistical analysis libraries such as dplyr, tidyr, olsrr, lmtest and mctest.

The entire project report can be found [HERE](https://maxwellpaterson.github.io/projects/Data_603_Final.pdf).

### Goal

The goal of this project was to create a model that could determine the medical insurance cost of a customer based on certain health and lifestyle metrics provided. The approach that we took to answer this question was creating a model by using multiple linear regression. 

### Process

First, we began by creating a full model for the data, including all of the variables in our regression model. The model that this created was the following

<img src="/images/fullmodeleq.png?raw=true" height = "50%" width = "50%"> 

Using this model we started by checking to make sure there was no multicollinearity present. This is to ensure that the variables that we are looking at are not affecting eachother as this would cause problems when we have a model with both variables as one of the independent variables, as they are technically speaking not independent if they affect eachother. Luckily, we found no multicollinearity in our model.

We then conducted multiple tests, such as the ANOVA test, F-test and T-test to determine which of the varibles were significant in our model. Using these tests we found that the sex variables was not significant and thus could be left out of our model.

From here we began to look at possible interaction terms and higher order terms that could be used to increase the accuracy of our model and found that the following interaction terms and higher order terms were significant enough to be included in our model.

highermodeleq (pic)

### Conclusion

In conclusion, the model that we found to be the best fit based on criteria such as RSE, adjusted R squared and AIC is the higher order model. Although, we do have to be cautious here of actually overfitting our model. Overfitting occurs when the model you have created works so well for your specific data that it actually does not generalize to other data well. If you get too specific and perfect with your model you actually end up just creating a model for your data that is not representative of the whole population.
