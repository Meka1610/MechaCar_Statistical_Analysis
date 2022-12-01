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


## T-Tests on Suspension Coils

Clarifying several terminologies below.

•	p-value : the probability we will get a sample that is as different from 1500 of this magnitude or more

•	T-test : asking something about the average

•	Alpha level : the probability of rejecting the null hypothesis when it is true

T-test Entire Lot
![t_test_entire](https://user-images.githubusercontent.com/111043588/205001626-e2acb79e-3b84-4cdc-a195-bc9c62238c45.PNG)


All Manufacturing Lots: p-value = .6028, alpha = .05
.60 > .05, we accept the null hypothesis. We are 95% confident that the true mean lies between 1497.51 and 1500 from this sample data. The sample data is not significantly different than 1500. The mean or average is 1498.78 → 1500. This is statistically similar to Lot 1 and Lot 2.

T-test Lot 1
 ![t_test_lot_1](https://user-images.githubusercontent.com/111043588/205001679-a67b7582-f293-467e-b85c-bd247074b223.PNG)

Lot 1: p-value = 1, alpha = .05
1 > .05, we accept the null hypothesis. We are 95% confident that the true mean lies between 1499.72 and 1500 from this sample data. The sample data is not significantly different than 1500. The mean or average is 1500. This is statistically similar to Lot 2 and entire manufacture lot.

T-test Lot 2
 ![t_test_lot_2](https://user-images.githubusercontent.com/111043588/205001714-7ca4613f-d82e-498d-8c96-3cad4a3581fd.PNG)
 
Lot 2: p-value = .6072, alpha = .05
.60 > .05, we accept the null hypothesis. We are 95% confident that the true mean lies between 1499.42 and 1500 from this sample data. The sample data is not significantly different than 1500. The mean or average is 1500.2. This is statistically similar to Lot 1 and entire manufacture lot.

T-test Lot 3
![t_test_lot_3](https://user-images.githubusercontent.com/111043588/205001758-888e6fbe-a87b-4f31-a195-ec63c15cf66c.PNG)

Lot 3: p-value = .04168, alpha = .05
.04 < .05, we reject the null hypothesis. We are 95% confident that the true mean lies between 1492.43 and 1499.85 from this sample data. The sample data is significantly different than 1500. The mean or average is 1496.14. Not statistically like the entire manufacture lot, nor Lot 1 or Lot 2.


## Study Design: MechaCar vs Competition

**•	What metric or metrics are you going to test?**

Two aspects of safety:

1)	crashworthiness = how good a vehicle protects its occupants in a collision

    o	look at injury risk in real time crashes
  
    o	crash dummy reports 
  
    o	deformation patterns of the vehicles 

2)	crash avoidance and mitigation = technology that can prevent a crash or lessen the severity
  
    o	forward collision avoidance technology
    
         -lasers, radar, cameras that detect other vehicles and objects in front of them

    o	rear collision avoidance technology
    
         -lasers, radar, cameras that detect other vehicles and objects in front of them (when backing up or in low   visibility)

    o	collision mitigation system
    
          -alter drivers, potential collision via visual and audiable alerts (allow for corrective action via driver)

**•	What is the null hypothesis or alternative hypothesis?**

Null Hypothesis (Ho): MechaCar 2022 lineups are priced correctly based on safety metrics. 
Alternative Hypothesis (Ha): MechaCar 2022 lineups are not priced correctly based on safety metrics. 

**•	What statistical test would you use to test the hypothesis? And why?**

Regression analysis, wanting to show the relationship between two or more variables.
**
•	What data is needed to run the statistical test?**

Real accidents, drilling down variables like width, length, height, weight, wheelbase, steering ratio, BHP (brake horsepower). There could be a list of several other dozen variables that would factor into this statistical test. 

