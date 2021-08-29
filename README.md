# MechaCar_Statistical_Analysis

## Project Overview
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. Use the R programming language to review the production data for insights that may help the manufacturing team.

## Resources
 - Data Source: [MechaCar_mpg.csv](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Resources/MechaCar_mpg.csv) [Suspension_Coil.csv](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Resources/Suspension_Coil.csv)
 - Software: Visual Studio Code, R, RStudio

## Linear Regression to Predict MPG
Linear Regression Output:
![Linear Regression Output](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig1.png)

 - Vehicle length and ground clearance are below the significance level of 0.05 and provide a non-random amount of variance to the mpg values in the dataset.
 - The linear model is not considered to be zero because the Multiple R-squared value for the regression model is 0.71 and the p-value is below the significance level of 0.05.
 - 71% of the variations in mpg can be explained by changes in the vehicle length, the vehicle weight, the spoiler angle, the drivetrain and the ground clearance. This indicates the linear model as efficient to predict mpg of MechaCar prototypes.

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

Summary Statistics for all Suspension Coil Manufacturing Lots:
![Statistics foa All Lots](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig2.png)
 - The design specifications for all Suspension Coil Manufacturing Lots in total meet the requirement with a variance of 62.3 psi.

Summary Statistics by Suspension Coil Manufacturing Lots:
![Statistics for Each Lot](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig3.png)
 - Individually, Suspension Coil Manufacturing Lot 1 and Lot 2 meet the requirement with variances of 0.98 and 7.5 psi. Suspension Coil Manufacturing Lot 3 does not meet the requirement with a variance of 170.3 psi.

## T-Tests on Suspension Coils

T-test for all manufacturing lots to population mean (1500 PSI):
![All](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig4.png)
 - The p-value of .06 does not provided evidence to eliminate the null hypotheses of the production population being similar to the mean assumption of 1500 PSI.
 - 
T-test for Lot 1 to population mean (1500 PSI):
![Lot1](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig5.png)
- The p-value of 1 does not provided evidence to eliminate the null hypotheses of the production population being like the mean assumption of 1500 PSI.

T-test for Lot 2 to population mean (1500 PSI):
![Lot2](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig6.png)
- The p-value of .06 does not provided evidence to eliminate the null hypotheses of the production population being like the mean assumption of 1500 PSI.

T-test for Lot 2 to population mean (1500 PSI):
![Lot3](https://github.com/LLeyva-bot/MechaCar_Statistical_Analysis/blob/main/Images/Fig7.png)
- The p-value of .04 indicates there is an issue with this lot and provides enough evidence to eliminate the null hypotheses of the production population being like the mean assumption of 1500 PSI.

## Study Design: MechaCar vs Competition
To quantify how the MechaCar performs against the competition, perform a statistical analysis using the following metrics:
 - clock the '0 to 60 mph' time
 - track the braking distance
 - measure the fuel economy (MPG)
 - measure of the horsepower
 - rate the safety measures

Hypotheses: All metrics are statistically similar between the MechaCar prototype and all vehicles from the other manufacturers.

ANOVA Test: Use this test to compare the means of each metric across the different manufacturers. To perform the test, gather the data in a single data frame where each metric is a column for the MechaCar prototype and its competition.
