[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> 

import scipy.stats
mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)


dist.mean()
# 178.0
dist.std()


dist.cdf(177.8) - dist.cdf(185.4)  
# 0.34209468294595308, so about 34.21% of people will qualify.
