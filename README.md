# Joel Vääräniemi's BSc thesis: Training decision trees using mixed-integer optimisation

Link to the thesis: https://sal.aalto.fi/publications/pdf-files//theses/bac/tvaa23_public.pdf

The code is based on the mathematical formulation for solving the optimal classification tree proposed by Bertsimas and Dunn (2017). The code solves the optimal classification tree for the iris dataset for given parameters D (maximum depth of the tree), α (complexity parameter) and N_min (minimum number of data points in each leaf node). We used JuMP as the optimisation framework and Gurobi 10.0.1 as the solver. CART-solutions for the sake of benchmarking are computed using DecisionTree.jl. The code is not implemented as structured packages as already in the early parts of speed testing we found out that desired computation speeds were not attainable without advanced heuristics in the optimisation process. 


## References: 
Bertsimas, D., & Dunn, J. (2017). Optimal classification trees. Machine Learning, 106, 1039-1082.
