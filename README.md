# MechaCar_Statistical_Analysis
## Overview
### AutosRUs' newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team's progress. I will be reviewing the production data for insights that may help the manufacturing team.

## Linear Regression to Predict MPG
### ![image](https://github.com/slafton/MechaCar_Statistical_Analysis/blob/main/images/linear%20regression%20of%20mecha_mpg.png)
### ![image](https://github.com/slafton/MechaCar_Statistical_Analysis/blob/main/images/p_value%20and%20r-squared%20values%20of%20linear%20regression%20mecha_mpg.png)
### Summary of Linear Regression to Predict MPG
#### * Vehicle length and vehicle ground clearance provide a non-random amount of variance to mpg values.
#### * The slope of the linear model would not be considered to be zero as the p-Value of this model is 5.35e-11 which is much smaller than the signifcance level of .05% and there is sufficient evidence to reject the null hypothesis.
#### * The linear model does predict mpg of MechaCar prototypes effectively. The r-squared is 0.71, meaning that approximately 71% of the variability of the dependent variable is explained using this linear model.

## Summary Statistics on Suspension Coils
### Total Summary Dataframe
### ![image](https://github.com/slafton/MechaCar_Statistical_Analysis/blob/main/images/total_summary%20dataframe.png)
### In the total summary the variance of the suspension coils, at 62.29 is within the 100 pounds per square inch.

### Lot Summary Dataframe
### ![image](https://github.com/slafton/MechaCar_Statistical_Analysis/blob/main/images/lot_summary%20dataframe.png)
### When we break the data up by lots, lots 1 and 2 still are within the 100 pounts per square inch at 0.98 and 7.47. However, lot 3 is not with it having a variance of 170.29!

## T-Tests on Suspension Coils
### T-Test Combined
### ![image](https://github.com/slafton/MechaCar_Statistical_Analysis/blob/main/images/one%20sample%20t-test.png)
### From this we can see that the true mean of the sample is 1498.78 with a p-Value of 0.06. The p-Value is higher than the significance level of .05 so there is not enough evidence to reject the null hypothesis. In conclusion, the mean of all of these manufacturing lots is similar to the population mean of 1500

### T-Test by Lot
### ![image](https://github.com/slafton/MechaCar_Statistical_Analysis/blob/main/images/t-test%20by%20lot.png)
### * In lot 1  we see a true sample mean of 1500 and a p-Value of 1. Again we would not reject the null hypotheses as there is no difference between the sample mean and the population mean.
### * In lot 2 it we have very similar results with a sample mean of 1500.2 and a p-Value of 0.61. We draw the same conclusion as in lot 1.
### * In lot 3 we see a sample mean of 1496.14 and a p-Value of 0.04. As this is a lower p-Value than the acceptable significance level of 0.05 we would reject the null hypothesis. This sample mean and the population mean are not a similar. 

## Study Design: MechaCar vs Competition
### With the rising fuel prices we have seen this year comparing fuel efficiency would be a smart move. By comparing MechaCar's fuel efficiency to Honda's, Ford's, Chevy's, Dodge's, and Nissan's we can see if there are improvements to be made to keep up or beat the competition.
### We will use the mpg as the dependent variable and the vehicle weight as the independent variable. 
### Null Hypothesis: If the vehicle weight does not impact the fuel efficiency, then reducing the vehicle weight will not result in using less fuel.
### Alternative Hypothesis: If the vehicle weight does impact the fuel efficiency, then reducing the vehicle weight will result in using less fuel.
### For this analysis we would need datasets of the competitors with vehicle weight and mpg and we would use simple linear regression because it builds a linear regression model with one independent variable.