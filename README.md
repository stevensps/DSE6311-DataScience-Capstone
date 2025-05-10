# The Evaluation of how Healthcare Access Impacts Self-Reported Mental Health Outcomes
By: Ben K., Chris R., and Steven S.

## Code Execution Flow
The code within this project should be run in the order below to reproduce the results discovered from this reasearch. Please note that running these files will **create and store data directly from the CDC on to your computer in the following location: C:\temp. After running the code, if you wish to remove the BRFSS dataset, please delete this folder.**
1) **Optional**: Place 2 EDAcode.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. NOTE: This step is optional in the process, and highlights the initial data analaysis done to prepare for modeling.
2) Place 3 calcSplitRatio-3.R in the user's working directory, which can be any folder on your computer, and run the code in RStudio. This is a custom function that determines the optimal train and test splits.
3) Place 4 Data Pre-Processing.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. These are the preprocessing steps to get the data in a model-ready state, and includes data imputation.
4) Place 5 PCA and K-Means.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. This file performs PCA to explore dimensionality reduction and K-Means to examine clustering of data points.
5) Place 6 Binary Logistic Regression.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. This model runs binary logistic regression, both with and without hyperparameter tuning as a baseline model.
6) Place 7 Random Forest.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. This model runs our champion model, Random Forest, and outputs metrics and results.
7) Place 8 XGBoost.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. This model runs our runner-up model, XGBoost, and outputs metrics and results.
8) **Optional**: If you wish to run all code, ranging from 4 Data Pre-Processing through.Rmd 8 XGBoost.Rmd, you may do so with this file. Please note that 3 calcSplitRatio-3.R is still required to run first. **Note**: Running step 8) requires significant computing resources, and for the common machine (i.e. personal laptop, etc.) will usually take at least 1 to 2 hours to run all of this code.
9) **Optional**: Place 9b Additional Data Visualizations.Rmd in the user's working directory, which can be any folder on your computer, and run the code in RStudio. This file performs optional data visualizations to contribute to the overall insights and findings within the BRFSS dataset.

## Project Background and Question
### Project Background
This project uses the 2023 Behavioral Risk Factor Surveillance System (BRFSS) dataset to evaluate how healthcare access predicts self-reported mental health outcomes. Our goal is to allow our findings to inform public health campaigns and healthcare resource allocation by clarifying the predictive relationships between healthcare access and mental health. Using BRFFS survey data, various machine learning (herein referred to as ML) algorithms are applied to understand: 
- If access to healthcare and other various demographic variables can predict self-reported mental health outcomes.
- Best practices for applying ML to large, weighted survey datasets.
### Project Question
Can we predict poor mental health outcomes, measured by self-report, among Americans by access to healthcare, after controlling for mental illness, demographics and other exposures?
## Hypothesis and Prediction
### Hypothesis
Healthcare access has a significant bearing on self-reported mental health outcomes because 
- Individuals without sufficient access are likely to suffer from unresolved mental health issues.
- Individuals without sufficient access experience higher stress levels and lower utilization of essential health services.
### Prediction
- Machine learning models trained on BRFSS data will identify access-to-care variables—such as health insurance status, cost-related barriers, and having a regular healthcare provider—as strong predictors of the number of poor mental health days.
- Tree-based models (e.g., Random Forest and XGBoost) will reveal disparities in predictive accuracy and feature importance across demographic subgroups (e.g., race, income, education), even without survey weighting.
- Respondents without health insurance, without a primary care physician, or who report being unable to afford medical care will be more likely to report a higher number of poor mental health days, even after accounting for demographic and behavioral covariates.




