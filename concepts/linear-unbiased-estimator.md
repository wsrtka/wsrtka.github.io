---
layout: default
permalink: /concepts/linear-unbiased-estimator
---

# Linear unbiased estimator
A linear estimator of \\(\beta_j\\) is a linear combination

$$
\beta_{j}^{'} = c_{1j}y_1 + ... + c_{nj}y_n
$$

in which the coefficients \\(c_{ij}\\) are not allowed to depend on the underlying coefficients \\(\beta_j\\), since those are not observable, but are allowed to depend on the values \\(X_{ij}\\), since these are observable. The estimator is said to be unbiased if and only if

$$
E[\beta_{j}^{'}] = \beta_j
$$

regardless of the values of \((X_{ij}\)).
