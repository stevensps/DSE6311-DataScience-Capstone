# The Evaluation of how Healthcare Access Impacts Self-Reported Mental Health Outcomes
By: Ben K., Chris R., and Steven S.

## Project Background and Question
### Project Background
This project explores the relationship between access to healthcare and the likelihood of self-reporting mental health outcomes. Using BRFFS survey data, various machine learning (herein referred to as ML) algorithms are applied to understand: 
- If access to healthcare predicts self-reported mental health outcomes.
- Whether survey weighting alters ML model performance.
- Best practices for applying ML to large, weighted survey datasets.
### Project Question
To what extent is self-reported mental health influenced by access to healthcare, and how does survey weighting impact the predictive performance of machine learning models trained on BRFSS data?
## Hypothesis and Prediction
### Hypothesis
Applying survey weighting adjustments on machine learning models changes feature importance, model fairness, and correctness of predictions because the adjustments are made to correct for representativeness of populations.
### Prediction
- ML models trained on weighted BRFSS data will yield different variable importance rankings and predictive performance compared to unweighted models.
- Weighting will enhance generalization across demographic groups but may introduce trade-offs in model complexity and performance metrics.
- Access to healthcare will significantly predict self-reported mental health, with more substantial effects observed in weighted models.




