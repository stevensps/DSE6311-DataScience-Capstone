# The Evaluation of how Healthcare Access Impacts Self-Reported Mental Health Outcomes
By: Ben K., Chris R., and Steven S.

## Code Execution Flow
The code within this project should be run in the following order to reproduce the results discovered from this reasearch:
1) Download and run EDAcodes.RMD in RStudio.
2) Run calcSplitRatio-3.R in RStudio and place in working directory
3) Run Data Pre-Processing.Rmd in RStudio and place in working directory

## Project Background and Question
### Project Background
This project explores the relationship between access to healthcare and the likelihood of self-reporting mental health outcomes. Using BRFFS survey data, various machine learning (herein referred to as ML) algorithms are applied to understand: 
- If access to healthcare predicts self-reported mental health outcomes.
- Best practices for applying ML to large, weighted survey datasets.
### Project Question
Can we predict poor mental health outcomes, measured by self-report, among Americans by access to healthcare, after controlling for mental illness, demographics and other exposures?
## Hypothesis and Prediction
### Hypothesis
Healthcare access has a significant bearing on self-reported mental health outcomes because individuals without sufficient access are likely to suffer from unresolved mental health issues, along with higher stress levels and lower utilization of essential health services.
### Prediction
- Machine learning models trained on BRFSS data will identify access-to-care variables—such as health insurance status, cost-related barriers, and having a regular healthcare provider—as strong predictors of the number of poor mental health days.
- Tree-based models (e.g., Random Forest and XGBoost) will reveal disparities in predictive accuracy and feature importance across demographic subgroups (e.g., race, income, education), even without survey weighting.
- Respondents without health insurance, without a primary care physician, or who report being unable to afford medical care will be more likely to report a higher number of poor mental health days, even after accounting for demographic and behavioral covariates.




