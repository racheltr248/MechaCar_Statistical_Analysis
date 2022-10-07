# MechaCar_Statistical_Analysis
Demo of R and its statistical test capabilities

## Background
AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. The data analyst has been asked to review the production data for insights that may help the manufacturing team. 

## Deliverable 1: Linear Regression to Predict MPG.
Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.

![linear_model](/Images/linear_model.PNG)

Q1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 
* Based on the dataset, vehicle length and ground clearance have a significant impact on miles per gallon. 

Q2. Is the slope of the linear model considered to be zero? Why or why not? 
* No. The p-value of 5.35e-11 is much smaller than our assumed significance level of 0.05%, allowing us to reject our null hypothesis.

Q3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
* Although there may be other, more effective models, the r-squared value of 0.7149033 indicates that this is an effective model. 

## Deliverable 2: Summary Statistics on Suspension Coils. 
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots,

![suspension_coils](/Images/suspension_coils.PNG)

![lot_summary](/Images/lot_summary.PNG)

Q1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
* Variance does not exceed 100 pounds per square inch for all manufacturing lots. However, the lot_summary dataframe shows that Lot3 has a variance of 170.2861224 PSI, exceeding the limitation. 

## Deliverable 3: T-Tests on Suspension Coils. 
Run t-tests to determine if the manufacturing lots are statistically different from the mean population. 

![t-test](/Images/t-test.PNG)
* The p-values of Lot1 (1) and Lot2 (0.6072) are above 0.05 and therefore we fail to reject the null hypothesis. However, the p-value of Lot3 (0.04168) is less than the level of significance and therefore we reject the null hypothesis.


## Deliverable 4: Study Design: MechaCar vs Competition. 
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.
* Additional metrics to include in a study comparing MechaCar to the competition could be: horsepower, fuel efficiency, price, and safety ratings. 
* The null hypothesis would be that there is no statistical difference whereas the alternate hypothesis would be that there is a statistical difference. 
* Since there are multiple variables of continuous types, I would use Multiple Linear Regression to test the hypothesis.
* In order to run the statistical test, I would need the data regarding horsepower, fuel efficiency, price, and safety ratings of MechCar vehicles and vehicles from other manufacturers. 