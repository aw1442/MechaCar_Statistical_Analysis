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

