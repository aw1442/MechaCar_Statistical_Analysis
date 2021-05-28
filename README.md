# MechaCar_Statistical_Analysis

# Deliverable 1:

## Linear Regression to Predict MPG

The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using your knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. 

Resulting model: 

mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD + (-104.0)

![image](https://user-images.githubusercontent.com/76754655/119601579-4977c300-bd9e-11eb-9e40-a180a366ec3d.png)

Based on the output above:

1. The vehicle length and ground clearance variables provided a non-random amount of variance to the mpg values in the dataset. The remaining variables, vehicle weight, spoiler angle, and AWD do not proved a non-random amount of variance to the mpg values in the dataset.
2. The slope of the linear model is not considered zero since the p-value for this model, 5.35e-11, is much smaller than the significance level of 0.05. This indicates there is sufficient evidence to reject the null hypothesis, which further indicates that the slope of this linear model is not zero.
3. This linear model does predict mpg of MechaCar prototypes effectively since the r-squared value is 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. 

# Deliverable 2:

## Summary Statistics on Suspension Coils

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

- The suspension coil’s PSI continuous variable across all manufacturing lots
- The following PSI metrics for each lot: mean, median, variance, and standard deviation.

The mean, median, variance, and standard deviation were calculated across all manufacturing lots:

![image](https://user-images.githubusercontent.com/76754655/119745862-ea6c8980-be43-11eb-916d-d8f39c4099e1.png)

The mean, median, variance, and standard deviation were also calculated for each manufacturing lot:

![image](https://user-images.githubusercontent.com/76754655/119745977-2acc0780-be44-11eb-913b-7e670e784849.png)

For all manufacturing lots, the variance of the coils is 62.29 PSI, which is within the 100 PSI variance reqruiement.

In addition, Lot 1 and Lot 2 are within the 100 PSI variance requirement with variances of 0.98 and 7.47, respectively. However, Lot 3 has a much larger variance of 170.29 which causes the majority of the variance for the overall manufacturing lots.

# Deliverable 3

## T-Tests on Suspension Coils

Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

Here is a summary of the t-test results across all manufacturing lots:

![image](https://user-images.githubusercontent.com/76754655/119756002-bdc26d00-be57-11eb-98fb-a114062fdea0.png)

Based on the above, the true mean of the sample is 1498.78, which is also in the summary statistics for delivrable 2. With a p-value of 0.06, which is higher than the significance level of 0.05, there is not enough evidence to reject the null hypothesis. In other words, the mean of all manufacturing lots is statistically similar to the presumed population mean of 1500.

![image](https://user-images.githubusercontent.com/76754655/119756354-49d49480-be58-11eb-99a3-d414cac27642.png)

Lot 1 has a true sample mean of 1500, as shown in deliverable 2 as well. With a p-value of 1, the null hypothesis is not rejected so the mean of lot 1 is statistically similar to the presumed population mean of 1500.

![image](https://user-images.githubusercontent.com/76754655/119756671-b2237600-be58-11eb-9ac7-f7b27fcf3e1c.png)

Lot 2 has a similar true sample mean of 1500.02 with a p-value of 0.61, so the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.

![image](https://user-images.githubusercontent.com/76754655/119756806-dd0dca00-be58-11eb-9bcd-b582b006adb8.png)

Lot 3 has a sample mean of 1496.14 and the p-value is 0.04, which is lower than the significance level of 0.05. Thus, the null hypothesis is rejected showing that this sample mean and the presumed population mean are statistically different.

As a result, lot 3 may have had some production issues to have statistically different PSI values from 1500.

# Deliverable 4

## Study Design: MechaCar vs Competition

A statistical study that can quantify how the MechaCar performs against competition can be the following metrics collected over the past 3 years:

- Cost: Dependent Variable
- Miles per gallon: Independent Variable
- Horse power: Independent Variable
- Maintenance cost (including insurance, gasoline): Independent Variable
- Safety rating: Independent Variable
- Engine (electric, hybrid, gasoline): Independent Variable

The null and alternative hypotheses include:

- Null Hypothesis: MechaCar is priced correctly based on its performance of key factors for its genre.
- Alternative Hypothesis: MechaCar is not priced correctly based on performance of key factors for its genre.

For statistical test, a multiple linear regression can be used to determine the factors that have the highest correlation/predictability with the list selling price (dependent variable) to determine which combination has the greatest impact on price (which could be multiple independent variables).

The data needed to run the statistical test would be what the cost of each car would be based on miles per gallon, horse power, maintenance cost, safety rating, and engine for the past 3 years. As a result, the multiple linear regression can be run to determine the correlation between the dependent and independent variables.
