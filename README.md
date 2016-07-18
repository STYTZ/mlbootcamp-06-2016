# ML Boot Camp 06-07.2016
My solution to ML Boot Camp contest

# Problem description

Propose an algorithm able to predict time required to mulptiply two matrices of sizes *m x k* and *k x n* on a given computer system described by a set of system parameters like CPU frequency, memory size and so on.

# Algorithm outline

- Group data by system parameters. There are 92 groups, which are the same for train and test set.
- Fit a Linear Regression (see jupyter notebook for details) for each group using matrix size as features, so there are 92 regressors.
- To make a prediction, select a group by system parameters and use corresponding regressor.
