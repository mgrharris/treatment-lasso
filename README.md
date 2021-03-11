# treatment-lasso
In this group project, our team performed a two-stage Lasso Regression (Treatment Lasso) to isolate the effect of our treatment variable, the number of connections, on the propensity to receive a loan for households in rural India.

We attempted to assess the impact of the number of connections independent of other X variables. As this was an observational study rather than an experiment, it was necessary to control over all other variables in the multivariate X. 

To do this, our group implemented a two-stage Lasso regression, also called a Treatment Lasso Method. In the first stage, we regressed the number of connections on other X variables to obtain a treatment variable of the number of connections independent of changes in X. In the second stage, we performed a subsequent Lasso regression using our treatment variable, our predicted treatment, and our multivariate X, only penalizing the multivariate X and treatment, and leaving the predicted treatment (d-hat) unpenalized.

To evaluate the effectiveness of our model, we evaluated the Mean Squared Error to measure deviance, and employed a Confusion Matrix to assess our prediction accuracy. 

Team members: Qihan Guan, Chloe Wang, Michael Harris. 
