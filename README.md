# Pairs-trading-with-cointegration-and-ML

The goal of this project is to develop a model that will give us better returns than the S&P
500 stock market returns by K-means clustering and pairs trading strategies . First of all ,
we will cluster the stocks on the basis of important features ( such as P/E ratio , Market Cap
) by using K- means Clustering algorithm . We will find optimal value for K by creating the
elbow graph using our fundamental data features . After finding K, we will create our
K-Means algorithm and select stocks from all Clusters to test whether or not we could
identify tradeable relationships in different combinations of pairs of particular clusters .
We'll create a method that will allow us to iterate over our pairs, compute the slope and
then perform the CADF test. The pairs that are cointegrated will be stored in a list . If two
pairs are cointegrated then they will drift towards and apart from each other around the
mean . It means their spreadness is stationary or converged . When the series diverges
from one another, we say that the spread is high. When they drift back towards each
other, we say that the spread is low. We need to buy one security and short the other .
We long the security that is underperforming and short the security that is over
performing .As the pairs are cointegrated the stock which is underperforming now, will
overperform and the stock which is overperforming now, will underperform at some
point of time to maintain the spreadness . At that point of time , We will do trading in
reverse order then the previous trading . By doing so in cointegrated pairs we will get
good returns as compared to the overall market .
