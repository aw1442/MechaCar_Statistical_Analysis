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
