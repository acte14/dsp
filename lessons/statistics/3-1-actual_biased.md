[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

response = nsfg.ReadFemResp()
massfunc = thinkstats2.Pmf(response.numkdhh, label='numkdhh')
thinkplot.Pmf(massfunc)
thinkplot.Config(xlabel='Actual # of children', ylabel='Probability Mass Function')
childeyes = BiasPmf(response, label='child reported')
thinkplot.PrePlot(2)
thinkplot.Pmfs([response, childeyes])
thinkplot.Config(xlabel='# of children', ylabel='Probability Mass Function')
response.Mean() = 1.024205155043831
childeyes.Mean() = 2.403679100664282


