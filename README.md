# MechaCar Statistical Analysis

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Linear Regression to Predict MPG
![Step 1 Dataset](https://user-images.githubusercontent.com/111723067/208008164-fef82dd3-4e56-4f4a-a02c-8b802f9217ea.png)

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
- Vehicle length and ground clearance provided a non-random amount of variance, meaning that those two variables heavily influence fuel efficiency.

### Is the slope of the linear model considered to be zero? Why or why not?
- No, the slope of the linear model is not zero because the p-value of the analysis is 5.35e-11. The p-value is less than the significance level of 0.05%, meaning there is sufficient evidence to reject the null hypothesis. 

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
- No, it does not due to lack of significant variables. 

![Step 1 Lin  Regression](https://user-images.githubusercontent.com/111723067/208008189-780632c7-47d6-421f-a291-6d9c30d5b783.png)

## Summary Statistics on Suspension Coils
![Step 2 Dataset](https://user-images.githubusercontent.com/111723067/208008738-e9f041bd-71a7-4469-b26b-0b32a6982d64.png)

### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
- The current manufacturing data meets thie design specifications for all manufacturing lots in total, but not individually. 
- In total: variance is 62.29.
- Individually: lot 3's variance is 170.26 which is 70% over the limit.

![Part 2 total summary](https://user-images.githubusercontent.com/111723067/208008777-68099629-85f4-4a00-86de-44fc5bb4c47d.png)
![Part 2 lot summary](https://user-images.githubusercontent.com/111723067/208008785-b2af5bcb-9153-401b-adde-4486ed5a7715.png)

## T-Tests on Suspension Coils
### The population: p-value = .06028 > .05
- No sufficient evidence to reject our null hypothesis -> fail to reject our null hypothesis -> the means of sample and population are statistically *similar*.
### The sample: p-value = .3758 > .05
- No sufficient evidence to reject our null hypothesis -> fail to reject our null hypothesis -> the means of sample and population are statistically *similar*.
### Lot 1: p-value = 1.0 > .05
- No sufficient evidence to reject our null hypothesis -> fail to reject our null hypothesis -> the means of sample and population are statistically *similar*.
### Lot 2: p-value = 0.6072 > .05
- No sufficient evidence to reject our null hypothesis -> fail to reject our null hypothesis -> the means of sample and population are statistically *similar*.
### Lot 3: p-value = 0.04168 < .05
- Sufficient evidence to reject our null hypothesis -> reject our null hypothesis -> the means of sample and population are statistically *different*.

![Part 3 T-Tests](https://user-images.githubusercontent.com/111723067/208009209-77e5afb4-d283-4128-bec8-bcdc7c170e28.png)
![Part 3 Sample Susp  Coil T-Test](https://user-images.githubusercontent.com/111723067/208009217-36794abd-502d-483f-9f70-a077a21d8f2b.png)

## Study Design: MechaCar vs Competition
### What metric or metrics are you going to test?
- Total number of recalls
- Overall safety
- Customer ratings/reviews
### What is the null hypothesis or alternative hypothesis?
- The null hypothesis: There is no statistical difference between average customer reviews of MechaCar in comparison to their competition.
### What statistical test would you use to test the hypothesis? And why?
- I would run tests using a dataset of customer satisfaction reviews of vehicles from MechaCar and their competitors. From there, I would find the average and see if there is a significant difference in reviews/ratings. I wouldl perfrom T-tests to find any statistical differences.
### What data is needed to run the statistical test?
- The data needed is customer reviews of cars from MechaCar and their main competitors.
