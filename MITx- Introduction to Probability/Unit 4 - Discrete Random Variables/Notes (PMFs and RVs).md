# Random Variables
- Loosely, a RV is a numerical quantity that takes random values based on some probabilistic experiment.
- We can derive  RVs from other RVs. For example BMI of a randomly selected student in a school is a RV that can be determined by two other RVs, Height and Weight R.Vs.
- To emphasise, a function of a RV is also a RV.
- RVs are denoted by capital letters (e.g X) and values of the function are denoted by lowercase letters (e.g. x)

# Probability Mass Functions (PMF)
- Probabilities of the different values of the RV
- denoted by P<sub>x</sub>
- note that PMFs are non-negative since we are talking about Probabilities.
- total of the PMF is equal to 1.

# Bernoulli

- bernoulli.pmf(k) 
    - = 1 - p, if k = 0
    - = p, if k = 1

# Expectations
- The expected value of a Random Variable is given by the value of RV multiplied by its probability.
- The expected value can be taken as average of the RV when we conduct many such experiments.
- Expected value rule: E[Y] = E[g[X]] = Σ g(X) * p<sub>X</sub>(x)
- Linearity of Expectations : E[aX + b] = a * E[X] + b
    - This is generally true for linear functions and does not hold for non-linear functions