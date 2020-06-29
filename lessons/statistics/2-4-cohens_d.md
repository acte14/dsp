[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)
Using the variable totalwgt_lb, investigate whether first babies are lighter or heavier than others. Compute Cohen’s d to quantify the difference between the groups. How does it compare to the difference in pregnancy length?
>> REPLACE THIS TEXT WITH YOUR RESPONSE

firsts = live[live.birthord == 1]
others = live[live.birthord != 1]
firsts.totalwgt_lb.mean(), others.totalwgt_lb.mean()
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
firsts.prglngth.mean(), others.prglngth.mean()
CohenEffectSize(firsts.prglngth, others.prglngth)


Cohen effect size for pregnancy length is 0.028879044654449883 , while the Cohen's D for baby weight is -0.088672927072602