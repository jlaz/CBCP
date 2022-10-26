# Credit-Based Congestion Pricing: Equilibrium Properties and Optimal Scheme Design

This repository contains the code used to conduct the numerical experiments in the paper ["Credit-Based Congestion Pricing: Equilibrium Properties and Optimal Scheme Design"](https://arxiv.org/...) submitted for presentation at the ["22nd International Conference
on Autonomous Agents and Multiagent Systems (AAMAS 2023)"](https://aamas2023.soton.ac.uk).

Credit-based congestion pricing (CBCP) address the equity challenges of congestion pricing strategies by allocating a budget of free credits to a group of eligible users to use to pay the tolls on a priced facility (e.g., an express lane on a highway, a cordoned portion of a road network). The numerical experiments were conducted to investigate the influence of CBCP schemes on the traffic patterns and study their optimal design through a case study of the San Mateo 101 Express Lanes Project. The equilibrium distribution of traffic flow on a four-lane highway with a single tolled express lane is estimated by solving the convex program presented in the paper. 

### Running the experiments
In the 'CBCP Experiments.ipynb' notebook, we provide the code used to set-up the case study, including the specification of the travel time functions, the generation of values of time (VoT) for each road user, and the designation of eligible versus ineligible road users. The code also includes the implementation of the dense sampling approach for the optimization of CBCP presented in the paper, wherein the convex program is solved with varying toll and budget values. Finally, the notebook includes code to produce the figures presented in the paper, including the distributions of key metrics by toll and bugdet values and the distributions of objective functions with various pareto weighting shceme.

### Dependencies
This code depends on maplotlib for visualization and gurobipy for optimization.

### Dataset
* VOT_distr.csv : the probability density function of VoT in San Mateo and Santa Clara counties estimated from the US Census 2021 American Community Survey (ACS) 1-Year Annual Earnings Esimates
