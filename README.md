#Project: Stratified Sampling Allocation – R Implementation
This project presents an R-based implementation of stratified sampling techniques used to estimate the population mean with a predefined level of precision.
The focus is on determining the required sample size and allocating samples across strata using classical and optimal allocation strategies.
Finite Population Correction (FPC) is applied to ensure accurate variance estimation when sampling from a finite population.

#Objectives
-Estimate the minimum required sample size for a given confidence level and margin of error
-Allocate samples efficiently across multiple strata
-Compare proportional, Neyman, and optimal allocation methods
-Analyze the effect of cost and time constraints on sampling design

#Stratified Sampling Overview
Stratified sampling divides the population into homogeneous subgroups (strata).
Independent random samples are drawn from each stratum, and combined to estimate overall population parameters.

This approach improves precision when:
Within-stratum variability is low
Between-stratum variability is high

#Precision and Sampling Bias
In this project, sampling bias refers to the allowable margin of error in estimating the population mean.
The sample size is determined such that the variance of the stratified sample mean does not exceed the specified precision level at the chosen confidence interval.

#Allocation Methods Implemented
1. Proportional Allocation
Samples allocated in proportion to stratum population size
Simple and effective when stratum variances are similar

2. Neyman Allocation
Allocation based on stratum size and variability
More samples assigned to highly variable strata
Provides better precision than proportional allocation

3. Optimum Allocation (Cost-Based)
Considers stratum size, variability, and cost per observation
Minimizes total survey cost while maintaining required precision

4. Optimum Allocation (Time-Based)
Uses time per observation instead of cost
Useful when survey duration varies across strata
Helps design time-efficient sampling plans

#Finite Population Correction (FPC)
Since sampling is conducted without replacement, FPC is applied to:
Adjust variance estimates
Prevent overestimation of uncertainty in finite populations
