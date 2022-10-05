# :chart: MechaCar_Statistical_Analysis

## Overview of the analysis

The purpose of this analysis is to help AutosRUs’ manufacturing team with insights on how the production process is working. The team has asked for a statistical analysis of the production data in order to identify any areas of improvement. The analysis will be performed using R and the following datasets:

- [MechaCar_mpg.csv](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/MechaCar_mpg.csv)
- [Suspension_Coil.csv](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/Suspension_Coil.csv)

----

## Deliverable :one

## :chart_with_upwards_trend: Linear Regression to Predict MPG

Deliverable 1 is a linear regression analysis that predicts the mpg of MechaCar prototypes using several variables from the [MechaCar_mpg.csv](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/MechaCar_mpg.csv) file. The variables used in the analysis are vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD. The analysis is performed using R and the lm() function. The results of the analysis are shown below:

![Deliverable 1](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_1_linearRegression_lm.png)

![Deliverable 1](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_1_linearRegression_summary.png)

The results of the analysis show that the variables provided are statistically unlikely to provide random amounts of variance to the linear model. The slope of the linear model is not considered to be zero. The `p-value` is `5.35e-11`, which is much smaller than the assumed significance level of `0.05%`. This means that there is sufficient evidence to reject the null hypothesis, which states that there is no relationship between the variables and the mpg of the MechaCar prototypes. The `r-squared`value is `0.7149`, which means that approximately `71%` of all mpg predictions will be determined by this linear model. The variables that provide a non-random amount of variance to the linear model are vehicle length and ground clearance, with `p-values` of `2.60e-12` and `5.21e-08`respectively. **The slope of the linear model is not considered to be zero.**

---

## Deliverable :two

## :bar_chart: Summary Statistics on Suspension Coils

Deliverable 2 is a summary statistics analysis of the suspension coil’s PSI capacity using the [Suspension_Coil.csv](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/Suspension_Coil.csv) file. The analysis is performed using R and the summary() function. The results of the analysis are shown below:

![Deliverable 2](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_2_boxplot_wholeLot.png)

![Deliverable 2](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_2_boxplot_individualLot.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed `100 pounds per square inch`. The current manufacturing data meets this design specification for all manufacturing lots in total and each lot individually. The variance for all manufacturing lots is `62.29`, which is well below the `100` pound per square inch limit. The variance for manufacturing lot 1 is `0.98`, which is well below the `100` pound per square inch limit. The variance for manufacturing lot 2 is `7.47`, which is well below the `100` pound per square inch limit. The variance for manufacturing lot 3 is `170.29`, which is well above the `100` pound per square inch limit.

---

## Deliverable :three:

## :memo: T-Tests on Suspension Coils

Deliverable 3 is a t-test analysis of the suspension coil’s PSI capacity using the [Suspension_Coil.csv]()

The analysis is performed using R and the t.test() function. The results of the analysis are shown below:

The results of the analysis show that the PSI across all manufacturing lots is statistically different from the population mean of `1,500` pounds per square inch. The `p-value` is `0.06028`, which is much larger than the assumed significance level of `0.05%`. This means that there is insufficient evidence to reject the null hypothesis, which states that there is no difference between the sample mean and the population mean. The `p-value` is `0.06028`, which is much larger than the assumed significance level of `0.05%`. This means that there is insufficient evidence to reject the null hypothesis, which states that there is no difference between the sample mean and the population mean.

![Deliverable 3](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_3_mecha_coil_t_test.png)

The results of the analysis show that the PSI for manufacturing <lot 1> is statistically different from the population mean of `1,500` pounds per square inch. The `p-value` is `1`, which is much larger than the assumed significance level of `0.05%`. This means that there is insufficient evidence to reject the null hypothesis, which states that there is no difference between the sample mean and the population mean.

![Deliverable 3](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_3_lot1_t_test.png)

The results of the analysis show that the PSI for manufacturing lot 2 is statistically different from the population mean of `1,500` pounds per square inch. The `p-value` is `0.6072`, which is much larger than the assumed significance level of `0.05%`. This means that there is insufficient evidence to reject the null hypothesis, which states that there is no difference between the sample mean and the population mean.

![Deliverable 3](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_3_lot2_t_test.png)

The results of the analysis show that the PSI for manufacturing lot 3 is statistically different from the population mean of `1,500` pounds per square inch. The `p-value` is `0.04168`, which is much smaller than the assumed significance level of `0.05%`. This means that there is sufficient evidence to reject the null hypothesis, which states that there is no difference between the sample mean and the population mean.

![Deliverable 3](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_3_lot3_t_test.png)

---

## Deliverable :four:

## :blue_book: Study Design: MechaCar vs Competition

Deliverable 4 is a statistical study design that compares the MechaCar to the competition. The study design is performed using R and the t.test() function.

![Deliverable 4](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_4_statistacal_design.png)

The metrics that will be tested are city and highway fuel efficiency, safety rating, and cost. 

Within this analyisis, the null hypothesis is that there is no difference between the MechaCar and the competition. 

![Deliverable 4](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_4_analytical_errors.png)

The alternative hypothesis showed that there is a difference between the MechaCar and the competition. 

Meanwhile, the statistical test used is a two-sample t-test. The data needed to run the statistical test is the city and highway fuel efficiency, safety rating, and cost against both the MechaCar and the competition. 

The data will need to be collected:
* over a period of time to account for seasonal and weather changes
* from a large enough sample size to ensure statistical significance
* from a representative sample of the population. 

![Deliverable 4](https://github.com/hastyjr/MechaCar_Statistical_Analysis/blob/main/Resources/images/Deliverable_4_a_b_testing.png)

In Summary, the statistical study design that compares the MechaCar to the competition is a two-sample t-test. The data needed to run the statistical test is the city and highway fuel efficiency, safety rating, and cost against both the MechaCar and the competition. The data will need to be collected over a period of time to account for seasonal and weather changes, from a large enough sample size to ensure statistical significance, and from a representative sample of the population.

---