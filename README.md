# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
Based on the results attached, the two variables that provided a non-random p-value variance to MPG values are vehicle length and ground clearance (p<0.05). The rest of the values, vehicle weight, spoiler angle, and AWD provided results greater than 0.05, which indicates a random correlation. 

The slope of the linear model is not considered to be zero. This is because the p-value on this linear model is 5.35e-11, suggesting the slope is not zero. 

<img src="supporting documents/P-and-Rsq-Value.png">

With a resulting r-squared value of 0.7149, the linear model does predict MechaChar prototypes effectively. Approximately 71% of all mpg predictions will be determined by this model.  

<img src = "supporting documents/D1-Statistical-Summary.png">

## Summary Statistics on Suspension Coils
- The design specs for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 PSI. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
The current manufacturing data meets the design spec not to exceed 100PSI. The variation for all lots is 62.29 PSI, well within the 100 PSI variance. 
However, for individual lots, we see the full picture. Lots 1 and 2 have an extremely low variance at 0.97 and 7.47 respectively, well within the variance requirement. Lot 3, though, shows a variance of 170 PSI, outside of the requirement. This has clearly skewed the all-lot variance data. 

<img src = "supporting documents/summary.png">

<img src = "supporting documents/lot_summary.png">

## T-Tests on Suspension Coils
- Summarize interpretation and findings for the t-test results. 
When performing a one-sample t-test for all lots, we get a mean of 1498.78. The p-value is 0.06, which is higher than the significance value of 0.05. We do not have enough evidence to reject the null hypothesis.

<img src = "supporting documents/D3 t-test-result.png">

We then ran a t-test on each of the individual lots. 

Lot 1: 
The resulting p-value of 1 suggests no difference between the groups other than due to chance. In this case we would accept the null hypothesis.

<img src="supporting documents/Lot1 PSI Subset .png">

Lot 2: 
The mean of 1500.2 and resulting p-value of 0.61 suggests the sample mean and presumed population mean of 1500 are statistically similar.

<img src="supporting documents/Lot2 PSI Subset.png">

Lot 3: 
Mean of 1496.14 and p-value of 0.04 (smaller than the significance value of 0.05) determines that the groups are statistically different.

<img src="supporting documents/Lot3 PSI Subset.png">

## Study design: MechaCar vs Competition
I would like perform a study to analyze how the MechaCar performs against its competitors regarding cost. Here are the metrics to be considered:

1. Cost comparison v competitors of similar size and features?
2. Maintenance cost and features v competitors?
  
  Null hypothesis: MechaCar is priced correctly based on a  comparison or performance and features of it's competitors.
  Alternative hypothesis: MechaCar is not priced correctly. 
  Statistical test: Multiple linear regression & t-test.
  Data needed: Costs of competitor vehicles, features of competitors for like model (MPG, maintenance costs, etc), maintenance cost and frequency of MechaCar and competitors.
  

