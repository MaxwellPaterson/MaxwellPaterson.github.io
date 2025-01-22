# Predicting Success Rate of Kickstarter Campaigns Using Linear Regression

This project was created by myself, Jackson Meier, Noah Seminoff and Weiwei Wang.

All of the analysis was completed using R.

Libraries used: Mosaic, Dplyr, Tidyr and GGplot.

The entire project report can be found [HERE](https://maxwellpaterson.github.io/projects/Data_602_Final.pdf)

### Goal

In this project we wanted to look at Kickstarter data and see if we could find a relationship between any of the variables present. We figured that there was most likely some type of correlation present between kickstarters success and their metrics. For example one of our first ideas was to see if a higher goal correlated to a lower success rate.

### Process

After doing lots of exploratory data analytics and struggling to find two variables that actually had a significant correlation coefficient, we stumbled upon the correlation between the number of projects launched in a month, and the overall success rate for projects launched that month.

<a href="https://maxwellpaterson.github.io/pages/kickstarter.html">
<img src="/images/kickstarterpic.png?raw=true" height = "100%" width = "100%"> 
</a>

In this scatterplot we can see that there seems to be a negative relationship between these two variables. 

The correlation coefficient between these variables is -0.46, which is not an overly strong relationship but compared to all the other variables we were looking at it proved to be one of the strongest relationships we could find.

### Conclusion

In conclusion, we can not definitively say that there is a causation between the number of projects launched in a month and the overall success rate of that month. But we can say that we found there was a correlation between these two variables where when there was an increase in the number of projects posted in a month, their chance of succeeding lowered with each additional project.
