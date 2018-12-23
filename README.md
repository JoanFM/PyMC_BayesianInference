# PyMC_BayesianInference
Code example obtained from the first chapter of the book BAYESIAN METHODS FOR HACKERS.

This example takes information of the number of SMS sent by a user for a period of time. We can use bayesian inference to see and validate the hypothesis that the SMS-sending behaviour follows a Poisson distribution. But this Poisson distribution may have two different lambda parameters based on the supsicious that at some day in the period the behaviour changes and the number of SMS sent increase.

We assume the prior assumption that lambda1 and lambda2 follow an Exponential distribution with a parameter 1/mean(count).
The prior distribution of the parameter tau refering to the moment where the behaviour switches is a DiscreteUniform.

The trained model using the Markov Chain MonteCarlo shows that it is very likely that there is a change of behaviour around the day 45.
