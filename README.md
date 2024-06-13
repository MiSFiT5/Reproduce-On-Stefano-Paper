# Reproduce-On-Stefano-Paper
reproduce the idea from the Stefano Moret in Escape34-PSE24 and his paper

## Basic Idea
For the three papers in ESCAPE and 1 paper from Google Scholar,

In methodology, the procedure is divided into 4 steps in general

 - Uncertainty characterization
 - Parameters sampling
 - Low regret strategy identification
 - Quantification of low-regret decisions


And for those 4 steps, corresponding to our progress, the first two could be considered the process of generation of solutions on pareto frontiers, and the last two could be considered as the 
projects on using machine learning method to identify or select the proper one from multiple feasible solutions.

For the last two steps, in all 3 papers on confernce and the paper on arxiv, the author used the combination of K-Means and Decision Tree.

K-Means for grouping the different strategies and Decision Trees are used to identify them, and then reorder them into a complete classification.

Besides, the author identify the regret model to evaluate the strategies, which could be considered as an loss function or objective function. setting a idealized situation where close to zero constraints, 
to converge the strategy selection in regret. But in the paper, there is no converge process, but only an evalution process.

Since the code and dataset have not open-sourced yet, here is a simplified version of a similar reproduction in some kind of problems in the code in this repo.
