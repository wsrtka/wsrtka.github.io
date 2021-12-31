---
layout: default
permalink: /algorithms/moving-average
---

# Exponential moving average
An exponential moving average, also known as an exponentially weighted moving average, is a way to estimate the average value of an unknown number of data points. This can be done by aplying the formula:

$$
\begin{equation}
    S_t =
    \begin{cases}
        Y_t, & \text{if}\ t=0 \\
        \alpha Y_t + (1 - \alpha) S_{t-1}, & \text{if}\ t > 0
    \end{cases}
\end{equation}
$$

where \\(Y_t\\) is the value at period \\(t\\), \\(S_t\\) is the current value of the moving average and \\(\alpha\\) is the coefficient that represents the degree of weighting decrease. It is a constant factor between 0 and 1. A higher \\(\alpha\\) discounts older observations faster. It also makes the choice of \\(S_1\\) less important.

It is also worth noting that the exponential moving average is an infinite impulse response filter. This is a property applying to many linear time-invariant systems that are distinguished by having an impulse response which does not become exactly zero past a certain point, but continues indefinitely.

