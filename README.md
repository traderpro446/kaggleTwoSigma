# Kaggle Competition: Two Sigma: Using News to Predict Stock Movements


### Task
 - Predict a signed confidence value, \hat{y}_{ti} \in [-1,1]
 - It is multiplied by the market-adjusted return of a given assetCode over a ten day window. 
 - x_t = \sum_i \hat{y}_{ti}  r_{ti}  u_{ti},
 - r_{ti} is the 10-day market-adjusted leading return for day t for instrument i
 - u_{ti} is a 0/1 universe variable that controls whether a particular asset is included in scoring on a particular day.
 - submission score: the mean divided by the standard deviation of daily x_t values
 - \text{score} = \frac{\bar{x}_t}{\sigma(x_t)}.
          
          
 
 
### Data
- There are two sources of data
- Market data (2007 to present) provided by Intrinio contains financial market information such as opening price, closing price, trading volume, calculated returns, etc.
- News data (2007 to present) Source: Thomson Reuters - contains information about news articles/alerts published about assets, such as article details, sentiment, and other commentary.
- Each asset is identified by an assetCode
- a single company may have multiple assetCodes
- synthetic future data within competition data to simulate 
- During stage one, the leaderboard will show performance on a historical period from 2017-01-01 to 2018-07-31.
- During stage two, Kaggle will re-run participants' selected Kernels on approximately six months of future data.

#### Market Data
- The data includes a subset of US-listed instruments.
- The set of included instruments changes daily and is determined based on the amount traded and the availability of information. 
- There may therefore be gaps in the data provided.
