# treatment-lasso
In this group project, our team performed a two-stage Lasso Regression (Treatment Lasso) to isolate the effect of our treatment variable, the number of connections, on the propensity to receive a loan for households in rural India. This two-stage Lasso is intended to control for other X variables which were not randomized over, as this is an observational study, and to isolate the effect of our treatment variable.

Our group was provided with data on whether or not households in India were granted loans based on a variety of provided variables. Our task was to determine how the 'number of connections' variable affected the outcome variable ('loan'), a binary response variable that provided whether or not a loan was granted.

We attempted to assess the impact of the number of connections independent of other X variables. As this was an observational study rather than an experiment, it was necessary to control over all other variables in the multivariate X. 

To do this, our group implemented a two-stage Lasso regression, also called a Treatment Lasso Method. In the first stage, we regressed the number of connections on other X variables to obtain a treatment variable of the number of connections independent of changes in X. In the second stage, we performed a subsequent Lasso regression using our treatment variable, our predicted treatment, and our multivariate X, only penalizing the multivariate X and treatment, and leaving the predicted treatment (d-hat) unpenalized.

To evaluate the effectiveness of our model, we evaluated the Mean Squared Error to measure deviance, and employed a Confusion Matrix to assess our prediction accuracy. 
