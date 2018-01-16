[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> 

random_list = np.random.random(1000)

pmf = thinkstats2.Pmf(random_list)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='random number', ylabel='PMF')

cdf = thinkstats2.Cdf(random_list)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='random number', ylabel='CDF')


# it's roughly uniformly distributed but given the sample size is small, some number has higher probility than others.
