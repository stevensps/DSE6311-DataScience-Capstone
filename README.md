# The Evaluation of how Healthcare Access Impacts Self-Reported Mental Health Outcomes
By: Ben K., Chris R., and Steven S.

## Code Execution Flow
The code within this project should be run in the following order to reproduce the results discovered from this reasearch:
1) **Optional**: Download and run 2 EDAcode.Rmd in RStudio. NOTE: This step is optional in the process, and highlights the initial data analaysis done for modeling.
2) Run 3 calcSplitRatio-3.R in RStudio and place in the user's working directory, which can be any folder on your computer. This is a custom function that determines the optimal train and test splits.
3) Run 4 Data Pre-Processing.Rmd in RStudio and place in the user's working directory, which can be any folder on your computer. These are the preprocessing steps to get the data in a model-ready state, and includes data imputation.
4) Run 5 PCA and K-Means.Rmd in RStudio and place in the user's working directory, which can be any folder on your computer. This file performs PCA to explore dimensionality reduction and Knn to K-Means to examine clustering of data points.
5) Run 6 Binary Logistic Regression.Rmd and place in the user's working directory, which can be any folder on your computer. This model runs binary logistic regression, both with and without hyperparameter tuning as a baseline model.
6) Run 7 Random Forest.Rmd and place in the user's working directory, which can be any folder on your computer. This model runs our champion model, Random Forest, and outputs metrics and results.
7) Run 8 XGBoost.Rmd and place in the user's working directory, which can be any folder on your computer. This model runs our runner-up model, XGBoost, and outputs metrics and results.
8) **Optional**: If you wish to run all code, ranging from 4 Data Pre-Processing through.Rmd 8 XGBoost.Rmd, you may do so with this file. Please note that 3 calcSplitRatio-3.R is still required to run first. **Note**: Running step 8) requires significant computing resources, and for the common machine (i.e. personal laptop, etc.) will take at least 4 hours to run all of this code.
9) **Optional**: Run 9b Additional Data Visualizations.Rmd and place in the user's working directory, which can be any folder on your computer. This file performs optional data visualizations to contribute to the overall insights and findings within the BRFSS dataset.

## Project Background and Question
### Project Background
This project explores the relationship between access to healthcare and the likelihood of self-reporting mental health outcomes, taking into account various demographic and social factors. Using BRFFS survey data, various machine learning (herein referred to as ML) algorithms are applied to understand: 
- If access to healthcare and other various demographics predicts self-reported mental health outcomes.
- Best practices for applying ML to large, weighted survey datasets.
### Project Question
Can we predict poor mental health outcomes, measured by self-report, among Americans by access to healthcare, after controlling for mental illness, demographics and other exposures?
## Hypothesis and Prediction
### Hypothesis
healthcare access has a significant bearing on self-reported mental health outcomes because individuals without sufficient access are likely to suffer from unresolved mental health issues, along with higher stress levels and lower utilization of essential health services.
### Prediction
- Machine learning models trained on BRFSS data will identify access-to-care variables—such as health insurance status, cost-related barriers, and having a regular healthcare provider—as strong predictors of the number of poor mental health days.
- Tree-based models (e.g., Random Forest and XGBoost) will reveal disparities in predictive accuracy and feature importance across demographic subgroups (e.g., race, income, education), even without survey weighting.
- Respondents without health insurance, without a primary care physician, or who report being unable to afford medical care will be more likely to report a higher number of poor mental health days, even after accounting for demographic and behavioral covariates.




