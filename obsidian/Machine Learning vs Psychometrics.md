# Machine Learning vs Psychometrics

#dissertation 


Its traditional strength is in handling complicated practical tasks, such as the prediction problems in shortening CMPA, as traditional statistical techniques in social science and education research do typically not handle with many outcome categories.

While both fields run statistics, machine learning does not emphasize knowing as much as statistics applied in social science and education research. The parameter estimates, such as regression coefficients and intercepts, are not as important, to the machine learning specialist, as how well the model overall performs the prediction task, indicated by metrics like the proportion of correct classifications (if the model had been meant to predict categorical data) or R squared (if the model had been linear-regression-like). There is, likewise, little emphasis on the p-values, Type I errors, effect size, or statistical power, because statistical inference is done using cross validation instead of applying the central limit theorem. If the model chosen had been linear regression, the machine learning specialist may not interpret the regression coefficients or intercepts and simply trains enough models that have the best R squared.

Since the current study uses open source packages for neural network written by contributors from the industry or machine learning, the model fitting and evaluation procedure will follow their norms in machine learning. That is, the current study, which uses a multilabel neural network to shorten CMPA, will not be evaluating the model based on p values or statistical power, or identifying/interpreting the regression weights of the neural network. Instead, it will be looking mainly to optimize performance measures like prediction accuracies and positive predictive power.

In the paragraphs that ensue, the neural networks will be introduced from the perspective of a researcher familiar with concepts of linear and logistic regression and some linear algebra.