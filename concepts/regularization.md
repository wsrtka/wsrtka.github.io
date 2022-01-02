---
layout: default
permalink: /concepts/regularization
---

# Regularization
Regularization is a technique used to discourage learning a more complex or flexible model so as to avoid the risk of overfitting. This is often done by setting a \\(\lambda\\) parameter and adding it as a penalty term to the cost function, for example:

$$
Cost(X, Y) = Loss(X, Y) + \lambda
$$

This way learning parameters with larger norms will be penalized. Two popular regularization techniques are L1 and L2 regularization. A regression model that uses the former technique is called Lasso Regression and a model using the latter is called Ridge Regression. The key difference lies in the penalty term:

$$
\text{L1 regularization: } \sum^{n}_{i=1}(y_i - \sum^{p}_{j=1} x_{ij} \beta_{j})^2 + \lambda \sum^{p}_{j=1} |\beta_{j}|
$$

$$
\text{L2 regularization: } \sum^{n}_{i=1}(y_i - \sum^{p}_{j=1} x_{ij} \beta_{j})^2 + \lambda \sum^{p}_{j=1} \beta^{2}_{j}
$$


