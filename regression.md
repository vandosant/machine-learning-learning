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

###Simple linear regression model:
Straight Line
f(x) [aka y] = w0 + w1 * x  

where w0, w1 represent regression coefficients (features)
where w0 represents intercept
where w1 represents slope

###Quality metric:  
Residual sum of squares (RSS) - Add up errors from prediction to actual values  
RSS(w0,w1) = &#949;(y - [w0 + w1 * x])<sup>2</sup>  

Choose the model that minimizes RSS [aka cost].

###Using the model:  
Predicting y for some value; plug x into the equation.  
Predicting x for some value; plug y into the equation. (y - w0) / w1  

Magnitude only has meaning for the specific units of input and output (e.g. $, sq. ft)

###Algorithms for fitting models
Minimize cost for parameters.  

###Optimizations
Convex/concave functions:
- Solution is unique.
-   Concave - line lies below function
-   Convex - line lies above function

Find the max or min analytically
- concave: max g(w) [derivative = 0]
- convex: min g(w) [derivative = 0]
- neither: no solution to derivative = 0 (multiple answers)

Derivative example:
g(w) = 5 - (w-10)<sup>2</sup>
dg(w) / dw = 0 - 2(w-10)<sup>1</sup> * 1
           = -2w + 20
