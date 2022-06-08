# MechaCar Statistical Analysis

## Deliverable 1 Linear Regression to Predict MPG

The dataset “MechaCar_mpg.csv” has miles per gallon (mpg) test results for 50 prototype MechaCars.  These prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using my knowledge of R, I designed a linear model that predicts the mpg of MechaCar prototypes using several variables from the “MechaCar_mpg.csv” dataset.


## Statistical Summary: 

- The vehicle length, and vehicle ground clearance are statistically unlikely to provide random variance results to the linear model. The vehicle length and vehicle ground clearance have a significant impact on the mpg the prototypes. In contrast, the spoiler angle, vehicle weight and all wheel drive (AWD) have p-Values that point to a random amount of variance within the “MechaCar_mpg.csv” dataset.
 -  The p-value of 5.35e-11 is much smaller than the significance level of 0.05. There is sufficient evidence that the slope of the linear model is not 0.
- With an R-squared of 0.7149 there is a moderate to strong chance that this linear model is effective at predicting mpg. There is a 71% chance that the variability of mpg is explained using this linear model.

![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/853909cc444a6e30f923f304077917712714246b/images/Screen%20Shot%202022-06-01%20at%207.25.16%20PM.png)<br>

### Additional Step
If we remove the vehicle weight, spoiler angle, and AWD (less impactful independent variables), the predictability does decrease, but not drastically: the r-squared value falls from 0.7149 to 0.674.

![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/853909cc444a6e30f923f304077917712714246b/images/Screen%20Shot%202022-06-01%20at%207.25.55%20PM.png)<br>

## Deliverable 2: Create Visualizations for the Trip Analysis
Useing the "Suspension_Coil.csv" data set two dataframes were created. 

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch (PSI).   

### Total Summary Dataframe
![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/853909cc444a6e30f923f304077917712714246b/images/Screen%20Shot%202022-06-01%20at%207.33.06%20PM.png)<br>

### Lot Summary Dataframe
![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/853909cc444a6e30f923f304077917712714246b/images/Screen%20Shot%202022-06-01%20at%207.34.06%20PM.png)<br>

Based on a review of the dataframes Lot 3 exceeds 100 PSI, therefore does not meet the design specification. The reason for this are numerous outliers (refer to plot below).

![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/853909cc444a6e30f923f304077917712714246b/images/image-2.png)<br>

## Deliverable 3: T-Tests on Suspension Coils 

The true mean of the sample is 1498.78.  With a p-Value of 0.06028, which is higher than the common significance level of 0.05, there isn’t enough evidence to support rejecting the null hypothesis. The mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/5840c0bd4ed03d950ac2b84b3955c23f3d002da0/images/Screen%20Shot%202022-06-01%20at%208.53.16%20PM.png)<br>

Lot 1 has a true sample mean of 1500 and a p-Value of 1.  We can’t reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean of 1500.


![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/5840c0bd4ed03d950ac2b84b3955c23f3d002da0/images/Screen%20Shot%202022-06-01%20at%208.53.30%20PM.png)<br>

Lot 2 has a true sample mean of 1500.02 and a p-Value of 0.6072.  Again we can’t reject the null hypothesis.


![image](https://github.com/blueschistrocks/MechaCar_Statistical_Analysis/blob/5840c0bd4ed03d950ac2b84b3955c23f3d002da0/images/Screen%20Shot%202022-06-01%20at%208.53.52%20PM.png)<br>

Lot 3 has a true sample mean of 1496.14and a p-Value of 0.04168.  The p-Value is lower than the common significance level of 0.05, therefore we should reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.
.
Some appears to have happened in the production cycle of Lot 3. The lot needs to be inspected to identify the issue. 

## Deliverable 4: Design a Study Comparing the MechaCar to the Competition

I would perform a study of the MechaCar up against competitors for the following:
- Fuel Economy 
- Emissions

#### Details to understand
-	What are the competitor models that are comparable to the MechaCar?
-	What factors should we look at in the study to determine?
-	What are the dependent and independent variables?

#### Data
- Obtain emissions data for the MechaCar and comparable competitor models that were provided to the U.S. Environmental Protection Agency (EPA) and/or California Air Resources Control Board (CARB).  


#### Hypothesis
The null hypothesis would be the MechaCar fuel economy and emissions are statistically similar to it’s competitors. The alternative hypothesis is that MechaCar fuel economy and emissions are not statistically similar to it’s competitors.

## Statistical Tests
A one-way Analysis of Variance (ANOVA) test is used to investigate the mean of a single continuous dependent variable across a single independent variable with multiple groups, similar to categorical data. In the two ANOVA) test analysis our independent variables are the type of transmission for a test of fuel efficiency and type of emissions controls for a test of emissions, which are categorical data types, and our dependent variables are fuel efficiency and emissions, respectively. These are numerical continuous data types.




