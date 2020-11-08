# Factors Affecting NFL Teams' Winning Rates

## Background Information

American football is another industry by itself. According to the American Gaming Association, a total of $6 billion was wagered on the 2019 Super Bowl.

Each team has a winning rate ever since the team was founded. The team with the highest winning rate is Dallas Cowboys -- 0.571, and the lowest rate is Tampay Bay Bunccaneers -- 0.389. 


![lowhigh](/img/lowhigh.png)


You can also check the NFL teams ranked by their wining rates below.


[NFL Rate.ipynb](https://github.com/gratefullee/NFL_WinningRate/blob/main/img/NFL_WinningRate.png)

Or winning rates by conference:


[AFC Rate.ipynb](https://github.com/gratefullee/NFL_WinningRate/blob/main/img/AFC_WinningRate.png)

[NFC Rate.ipynb](https://github.com/gratefullee/NFL_WinningRate/blob/main/img/NFC_WinningRate.png)


## Data Sources
This project is based on multiple datasets showing -- 
1) all-time teams' winning rates: https://www.pro-football-reference.com/teams/
2) players PT records: https://stathead.com/football/nfl-combine-results.cgi
3) all-time each players' stats (punt, fumbles, etc.): https://www.kaggle.com/tobycrabtree/nfl-scores-and-betting-data


## Data Analysis

1. There is no correaltions between teams' winning rates and players' physical scores. 

![correlations](/img/PTCorr.png)

2. Teams' completion rate, yards per punt return, the number of fumbles can determine teams' winning rate.

![SingleFactor](/img/SingleFeature.png)
![PartialRegression](/img/PartialRegression.png)

Partial regression rate for each factor: 

Average Completion Percentage: 0.005176

Average Number of Fumbles Lost: -0.177058

Average Yards Per Punt Return: 0.014572

Based on the rate, the completion rate has the least impact. 
Below is a 3D graph without the completion rate. 
![3DPartialR](/img/3DPartialR.png)


## Conclusions

1. Players' physical scores does not affect teams' winning rates. 
2. Completion rates, the number of fumbles lost, and yards per punt can highly decide teams' winning rates. 
