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

in this repo i reproduce the first paper listed below, and the methodology is nearly to same just to swtich the metrics in the other paperss.

# intro
This repository contains the implementation and replication of methods described in several research papers focused on decision-making under uncertainty in energy transition scenarios. The key papers reproduced here include:

### Low-regret Decisions for the Steam Supply in the Chemical Industry:
This paper introduces a method to identify low-regret decisions for steam supply decarbonization in the chemical industry. By using global sensitivity analysis, the method characterizes uncertainties, samples parameters, and evaluates potential decisions to find those that are near-optimal across various future scenarios.

### A Machine Learning Method to Extract Key Policy Decisions from Energy Transition Scenarios under Uncertainty:
This study leverages decision trees, a popular machine learning technique, to translate complex energy transition scenarios into a small set of key policy decisions. The method involves clustering scenarios and training decision trees to identify critical decisions that shape the energy transition.

### The Role of Biomass in the Swiss Energy Transition: Low-Regret Strategies for an Uncertain Future:
This paper presents a method for long-term energy system planning under uncertainty, specifically focusing on biomass utilization in Switzerland. The approach identifies low-regret strategies by clustering scenarios and evaluating them using a regret-based analysis.

### Streamlining Energy Transition Scenarios to Key Policy Decisions:
This paper demonstrates a method to streamline numerous energy system scenarios into a few interpretable storylines by training decision trees on key outputs of interest. The approach simplifies the decision-making process by highlighting critical policy decisions and their trade-offs.

# Repository Content

 - Data Preparation: Scripts for preprocessing and generating input data based on various uncertainty parameters.

 - Clustering Analysis: Implementation of k-means clustering to group similar scenarios.

 - Decision Tree Training: Code for training decision tree models to identify key policy decisions based on clustered data.

 - Regret Analysis: Functions to compute and analyze regret for different strategies across various scenarios.

 - Visualization: Tools for visualizing decision trees, scenario clusters, and regret distributions to interpret and communicate results effectively.

# Getting Started
To get started with the code, please follow the instructions provided in the Installation section. Each directory contains detailed information about the scripts and their usage. Refer to the Examples section for practical demonstrations of replicating the methods from the papers.

# Goals
The goal of this project is to provide a comprehensive and replicable implementation of state-of-the-art methods in decision-making under uncertainty for energy systems. By offering these tools, we aim to support researchers and policymakers in making informed decisions to facilitate the energy transition.


