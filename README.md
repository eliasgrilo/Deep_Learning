# Deep_Learning

Introduction:

• Energy-Based Models

• Objective: Minimize the energy

• Similar to the problem with our cost function

Energy-based models (EBMs) are a type of probabilistic model that assigns an energy level to each configuration of the variables of interest. The principle is simple: configurations with lower energy are more likely than those with higher energy.

These models are called "energy-based" because they use an energy function to measure the compatibility between the observed data and the variables of the system. The goal is to adjust the model parameters to minimize this energy.

This is somewhat similar to the problem we often face with cost or loss functions in machine learning, where the aim is to adjust the model parameters to minimize the cost function. In the case of EBMs, the energy function plays a role analogous to the cost function, with the main difference being that we try to minimize the energy function over possible configurations of the system variables, not over parameters.

# Boltzmann Machines

• A Boltzmann machine is a one-layer fully connected neural network (FNN)
• Our goal: to learn the probability distribution of the inputs
• Adjust weights to be able to reconstruct the inputs
• Restricted Boltzmann Machine (RBM)

Boltzmann machines are a type of stochastic recurrent neural network and one of the basic types of energy-based models. They are used to model complex systems by learning the underlying probability distribution. This can be particularly useful in tasks such as dimensionality reduction, classification, collaborative filtering, and feature learning.

The learning process involves adjusting the weights of the connections in the network so that the system can accurately reconstruct its input data. This is done by trying to minimize the difference (or the "energy") between the input and output of the network.

A Restricted Boltzmann Machine (RBM) is a simplified version of the Boltzmann machine, with a restriction that its neurons must form a bipartite graph. This means that there are no connections between nodes within the same layer (visible or hidden layer). The simplification allows for more efficient training algorithms, such as contrastive divergence.
