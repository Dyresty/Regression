# Polynomial Regression

##### Simple Linear Regression
y = b0 + b1x1

##### Multiple Linear Regression
y = b0 + b1x1 + b2x2 + ... + bnxn

##### Polynomial Linear Regression
y = b0 + b1x1 + b2(x1^2) + ... + bn(x1^n)<br>
The powers make the curve more parabolic<br><br>

It is still linear regression<br>
Polynomial regression is linear in parameters/coefficients<br>
The term "linear regression" refers to linearity in coefficients, not in input variables<br>

In polynomial regression, we transform the input features but still fit a linear model to these transformed features.
y = b0 + b1x1 + b1x1^2 + C
x^2 is just another feature, so the model is still linear in the parameters 
This is different from nonlinear regression, where parameters appear in nonlinear ways (e.g., exponentials, products of parameters).
