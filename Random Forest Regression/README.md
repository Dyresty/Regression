# Random Forest 
Random Forest for Classification and Regression

## Ensemble Learning
Ensemble learning is when multiple algorithms / same algorithm multiple times are put together to make something much more powerful. 
- Random forest is a version of Ensemble Learning, there are other versions such as gradient boosting. 

Random Forest 
- Step 1 - Pick K random data points from the Training Set.
- Step 2 - Build the Decision Tree associated to these K data points.
- Step 3 - Choose the number N of trees to build. Repeat Steps 1 & 2.
- Step 4 - For a new data point, make each of the N trees predict value of Y for that data point.<br>
  Assign the new data point the average across all the predicted Y values. 

So, in this way we get good results because
- The average of the decision trees will give better overall results than an individual tree. More
- Ensemble algorithms are more stable because any change in the data set could really impact one tree. But for them to affect a forest of trees is much harder, therefore ensemble is more powerful in that way.


# Random Forest Regression
For continuous values. 
