# logistic-Regression

In statistics, the logistic model (or logit model) is a statistical model that is usually taken to apply to a binary dependent variable. In regression analysis, logistic regression or logit regression is estimating the parameters of a logistic model. More formally, a logistic model is one where the log-odds of the probability of an event is a linear combination of independent or predictor variables. The two possible dependent variable values are often labelled as "0" and "1", which represent outcomes such as pass/fail, win/lose, alive/dead or healthy/sick. The binary logistic regression model can be generalized to more than two levels of the dependent variable: categorical outputs with more than two values are modelled by multinomial logistic regression, and if the multiple categories are ordered, by ordinal logistic regression, for example the proportional odds ordinal logistic model.


    Mathematically this can be written 
                                        g(E(y)) = α + βx1 + γx2
                                        
In logistic regression, we are only concerned about the probability of outcome dependent variable ( success or failure). As described above, g() is the link function. This function is established using two things: Probability of Success(p) and Probability of Failure(1-p). p should meet following criteria:

It must always be positive (since p >= 0)
It must always be less than equals to 1 (since p <= 1)
Now, we’ll simply satisfy these 2 conditions and get to the core of logistic regression. To establish link function, we’ll denote g() with ‘p’ initially and eventually end up deriving this function.

Since probability must always be positive, we’ll put the linear equation in exponential form. For any value of slope and dependent variable, exponent of this equation will never be negative.

                  p = exp(βo + β(Age)) = e^(βo + β(Age))    ------- (b)

To make the probability less than 1, we must divide p by a number greater than p. This can simply be done by:

                  p  =  exp(βo + β(Age)) / exp(βo + β(Age)) + 1   =   e^(βo + β(Age)) / e^(βo + β(Age)) + 1   



                  p = e^y/ 1 + e^y           --- (d)

where p is the probability of success. This (d) is the Logit Function
If p is the probability of success, 1-p will be the probability of failure which can be written as:

                 q = 1 - p = 1 - (e^y/ 1 + e^y)    --- (e)




                                





