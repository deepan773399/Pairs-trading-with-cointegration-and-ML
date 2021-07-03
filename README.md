# Pairs-trading-with-cointegration-and-ML

Introduction
K-means clustering - Kmeans algorithm is an iterative algorithm that tries to
partition the dataset into Predefined distinct non-overlapping subgroups (clusters)
where each data point belongs to only one group . It assigns data points to a cluster
such that the sum of the squared distance between the data points and the
cluster’s centroid (arithmetic mean of all the data points that belong to that cluster)
is at the minimum. The less variation we have within clusters, the more similar the
data points are within the same cluster.
Pairs trading - Pairs trading is one of the most popular types of trading strategy.
In this strategy, usually a pair of stocks are traded in a market-neutral strategy, i.e.
it doesn’t matter whether the market is trending upwards or downwards, the two
open positions for each stock hedge against each other. The key challenges in pairs
trading are to:2
1.Choose a pair which will give you good statistical arbitrage opportunities over
time
2.Choose the entry/exit points
For pair selection we will use cointegration.
For entry/exit points we will use mean reversion .
Cointegration - The most common test for Pairs Trading is the cointegration
test. Cointegration is a statistical property of two or more time-series
variables which indicates if a linear combination of the variables is stationary.
Let us understand this statement above. The two-time series variables, in this
case, are the log of prices of stocks A and B. Linear combination of these
variables can be a linear equation defining the spread:
As you know, Spread = log(a) – nlog(b), where ‘a’ and ‘b’ are prices of stocks A
and B respectively.
For each stock of A bought, you have sold n stocks of B.
If A and B are cointegrated then it implies that this equation above is stationary. A
stationary process has very valuable features which are required to model Pairs
Trading strategies. For instance, in this case, if the equation above is stationary, that
suggests that the mean and variance of this equation remains constant over time.
So if we start with ‘n’, which is called the hedge ratio, so that spread = 0, the
property of stationary implies that the expected value of spread will remain as 0.
Any deviation from this expected value is a case for statistical abnormality, hence a
case for pairs trading!
Mean reversion - Mean reversion, or reversion to the mean, is a statistical
principle that can be used in finance and investing. It states that volatile prices and
historical fluctuations will eventually return, or revert, to the long-term average, or
mean, of a dataset.
