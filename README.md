# Kaggle Competition: Two Sigma: Using News to Predict Stock Movements


### Task
 - Predict a signed confidence value, \hat{y}_{ti} \in [-1,1]
 - It is multiplied by the market-adjusted return of a given assetCode over a ten day window. 
 - x_t = \sum_i \hat{y}_{ti}  r_{ti}  u_{ti},
 - r_{ti} is the 10-day market-adjusted leading return for day t for instrument i
 - u_{ti} is a 0/1 universe variable that controls whether a particular asset is included in scoring on a particular day.
 - submission score: the mean divided by the standard deviation of daily x_t values
 - \text{score} = \frac{\bar{x}_t}{\sigma(x_t)}.
          
          
 
 
