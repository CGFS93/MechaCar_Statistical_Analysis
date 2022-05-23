# MechaCar_Statistical_Analysis

## Overview of the Analysis:
R Analysis: Linear Regression to Predict MPG, Summary Statistics on Suspension Coils, T-Test on Suspension Coils, Design a Study Comparing the MechaCar to the Competition.

### Purpose:

Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers.


## Resources

**Data Source:** MechaCar_mpg.CSV, Suspension_Coil.CSV.

**Software:** R, R Studios, Git_Hub.

## Results:

## Linear Regression to Predict MPG

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879902-e84fdeab-99b6-4ccd-a7d6-a37a966e7354.png"> 
</p>

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 

The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. As indicated by the yellow arrows in the image above, a linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.

- Is the slope of the linear model considered to be zero? Why or why not? 

The slope of the linear model can not be considered to be zero, as the p-value of 5.35x10-11, indicated by the orange arrow above, is lower than even an extreme level of significance, and thus the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not? 

Although there are still unconsidered factors, this model does predict the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149, highlighted in the purple box, indicates that the model is 71% accurate... though it could probably do better.

<br>
