Regression
==========

Simple
------
Have some data point x, want to predict some output of interest y as f(x)  
Assumes mean error value of 0; equally likely to be + or -  
y = f(x) + E(epsilon)  

1. Which model f(x)? [quadratic]
2. Estimate a specific fit to data.
  - Find the model that fits data with minimal error.

Simple linear regression model:
### Straight Line
f(x) = w0 + w1 * x  
where w0, w1 represent regression coefficients (features)
where w0 represents intercept
where w1 represents slope

Quality metric:  
Residual sum of squares (RSS) - Add up errors from prediction to actual values
RSS(w0,w1) = &#949;(y - [w0 + w1 * x])<sup>2</sup>
