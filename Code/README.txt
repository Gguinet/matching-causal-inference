Here is the code we used for our project:

Mains:

* simulation.rmd is the file to use for running the simulation to compare different matching methods on synthetic data. 

* traumabase.rmd is the file to use to preprocess the traumabase in order to use the matching methods (and bootstrapping) to estimate the causal effect.

Auxiliary Functions:

*amputation.R is the code from https://rmisstastic.netlify.com/how-to/generate/misssimul used to generate missing values in data

* DataGeneration.R is the code used to generate our 9 scenarios, each corresponding to a distribution of data. Parameters (means, variance) are hardcoded here.

* globalSimulation is the code used to run the simulation given as input the scenario chosen and the number of simulation

* matchingFunctions.R are the matching algorithms to use for synthetic data. It contains coarsened exact matching, propensity matching (logistic regression, random forest, backward AIC)

* matchingFunctionsTraumabase.r are the matching algorithms to use for the traumabase. It contains coarsened exact matching, propensity matching (logistic regression, random forest, backward AIC)

* missingValSimulation.R is the code used to generate our 9 scenarios with missing values, that can be generated and imputed in different ways.

* plotFunctions.R is the code used to plot ATT and difference in mean for the simulations

