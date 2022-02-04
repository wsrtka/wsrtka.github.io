---
layout: default
permalink: /concepts/regularization
---

# Regularization
Regularization is a technique used to discourage learning a more complex or flexible model so as to avoid the risk of overfitting. This is often done by setting a \\(\lambda\\) parameter and adding it as a penalty term to the cost function, for example:

$$
Cost(X, Y) = Loss(X, Y) + \lambda
$$

This way learning parameters with larger norms will be penalized. The challange is that during training and parameter exploration, the algorithm sometimes picks locally optimal though globally poor parameter values. Regularization can influence this choice by penalizing larger values for weights and trying to keep te weight exploration to the optimal area.

## L1 and L2 regularization

Two popular regularization techniques are L1 and L2 regularization. A regression model that uses the former technique is called Lasso Regression and a model using the latter is called Ridge Regression. The key difference lies in the penalty term:

$$
\text{L1 regularization: } \sum^{n}_{i=1}(y_i - \sum^{p}_{j=1} x_{ij} \beta_{j})^2 + \lambda \sum^{p}_{j=1} |\beta_{j}|
$$

$$
\text{L2 regularization: } \sum^{n}_{i=1}(y_i - \sum^{p}_{j=1} x_{ij} \beta_{j})^2 + \lambda \sum^{p}_{j=1} \beta^{2}_{j}
$$

L2 regularization penalizes weights with large magnitudes. Large weights are the most obvious symptom of overfitting, so it’s an obvious fix. It’s less obvious that L2 regularization actually has a Bayesian interpretation: since we initialize weights to very small values and L2 regression keeps these values small, we’re actually biasing the model towards the prior.

## Dropout regularization

At each training step, dropout clamps some weights to 0, effectively stopping the flow of information through these connections. This forces the model to distribute computations across the entire network and prevents it from depending heavily on a subset features.

### Sources:

- [Art of regulariation](https://greydanus.github.io/2016/09/05/regularization/) by Sam Greydanus

