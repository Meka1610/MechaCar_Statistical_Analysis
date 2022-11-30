# MechaCar_Statistical_Analysis


## Linear Regression to Predict MPG

![mpg](https://user-images.githubusercontent.com/111043588/204923495-c73f6502-1e86-4b8b-982a-3fddb7e77f91.PNG)


**•	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

  Vehicle length (p-Value: 2.60e-12) and vehicle ground clearance (p-Value:5.21e-08) are the non-random variances to the mpg   values in the dataset. 


**•	Is the slope of the linear model considered to be zero? Why or why not?**

  No, the slope of the linear model is not considered to be zero. The above output indicates the coefficients (vehicle         length, vehicle weight, spoiler angle, ground clearance, and AWD) contain significant non-zero values). In addition, we       would reject the null hypothesis because the model for the p-Value: 5.35e-11 is not greater than .05. Typically, this is     considered to be statistically significant.


**•	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

  Yes, the linear model does predict mpg of MechaCar prototypes effectively because r-squared value: 0.7149. the model needs   to be r >= 0.7. Roughly 71 percent of all miles per gallon predictions can be determined by this model. This makes the       dataset a strong and effective one. 


## Summary Statistics on Suspension Coils

Total Summary Dataframe
![total_summary](https://user-images.githubusercontent.com/111043588/204931236-6f27dd1f-65ac-4509-bc7f-6d445e118342.PNG)


Lot Summary Dataframe
![lot_summary](https://user-images.githubusercontent.com/111043588/204931253-1a5a017e-86ad-4114-a93d-23aae62ab8b7.PNG)


**•	The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?**

The current manufacturing data meets the design specification for all manufacturing lots in total. This is true because the total summary variance is 62.29 which does not exceed 100 pounds per square inch (PSI) suspension coils. However, when looking at the lots individually the answer is slightly different. The variance for lot 1 (0.97) and lot 2 (7.47). Both lot 1 and lot 2 respectfully do not exceed 100 lbs.  PSI. Regarding lot 3 the variance is 170.29. It exceeds the 100 lbs. PSI. 
