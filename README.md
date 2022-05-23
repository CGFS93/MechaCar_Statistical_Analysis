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

The most significant variables in the dataset that show a non-random effect on the MPG of the MechaCar_mpg are the Vehicle Length and the Ground Clearance. A linear regression model run on these variables against figures for MPG resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.

- Is the slope of the linear model considered to be zero? Why or why not? 

The slope of the linear model can not be considered to be zero, as the p-value of 5.35x10-11, is lower than even an extreme level of significance, the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is subject to more than random chance.

- Does this linear model predict the mpg of MechaCar prototypes effectively? Why or why not? 

Although there are unconsidered factors, this model does predict the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149, indicates that the model is 71% accurate.

<br>

## Summary Statistics on Suspension Coils

<p align="center">
Total Summary 
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879908-88c318d7-1603-4395-b9b9-98685dd983c9.png"> 
</p>

<p align="center">
Lot Summary
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879906-96f066a1-09dd-4506-8c99-b50eee47ffb5.png"> 
</p>

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with one of the individual lots. As shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28.

<br>

## T-Tests on Suspension Coils

<p align="center">
    Suspension Coils Cumulative T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879911-c2cd55b4-9b8b-487d-82a6-f9fdf55e7a84.png"> 
</p>

- A review of the results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.

<p align="center">
    Suspension Coils Lot 1 T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879913-441551a5-d902-458b-b22a-07492b640d48.png"> 
</p>

- A review of the results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) for us to reject the null hypothesis.

<p align="center">
    Suspension Coils Lot 2 T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879914-ecf657d1-8fea-4db3-9dba-37580fe2d7d8.png"> 
</p>

- A review of the results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis.

<p align="center">
    Suspension Coils Lot 3 T-test
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/98966503/169879915-799e8148-f71d-4d1c-8fba-c2222e24d6f4.png"> 
</p>

- A review of the results of the T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) for us to reject the null hypothesis. This lot may be need to be discarded, or at least more closely evaluated.

<br>

## Summary:

## Study Design: MechaCar vs Competition

There are many factors that consumers take into consideration when evaluating a car to purchase. However, in a world where ridesharing is becoming more ubiquitous and it's easy and cheap to get around in other people's vehicles, customers looking to purchase a car are looking for more than just a conveyance. They will be looking to buy a car that is an economical means to regularly transport themselves and their items on a reliable, regular basis.

</p>

- What metric or metrics are you going to test?

<p align="center">

To narrow down our test, we should evaluate MechaCar's carrying capacity, in cubic inches, in comparison to various competitors' vehicles.

</p>

- What is the null hypothesis or alternative hypothesis?

<p align="center">

H<sub>0</sub>: MechaCar prototypes' average carrying capacity is similar to competitor's vehicles in the same vehicle class
H<sub>a</sub>: MechaCar prototypes' average carrying capacity is statistically above or below that of competitor vehicles.

</p>

- What statistical test would you use to test the hypothesis? And why?

<p align="center">

The best statistical test for this would be two-sample t-tests.

</p>

- What data is needed to run the statistical test?

<p align="center">

We would need to gather cubic space data from the carrying compartments of all MechaCar prototypes, as well as from all major competitor vehicles.

</p>
