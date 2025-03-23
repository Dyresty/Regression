# Support Vector Regression (SVR)

Linear SVR<br>
A tube with distance epsilon(vertically measured) on both sides of the regression line. Called the Epsilon Insensitive Tube. <br>
So if a point falls within the Epsilon Insensitive Tube, we do not consider the error of distance from regression line. Gives a certain amount of buffer to the model. <br>
For points falling outside the Epsilon Insensitive Tube, we measure the distance between the point and the tube itself. Points below the tube are called ci* and points above the tube are called ci.<br>

Support vectors are the points outside the tube, called so because they are supporting the structure or formation of the tube. Hence called Support Vector Regression. <br>
