# Molecular-Property-Optimization-Algorithms

This repository contains research-driven implementations exploring how artificial intelligence can accelerate molecular discovery and optimization. The work focuses on three core approaches:

1. Genetic Algorithms for Molecular Search
Implements a population-based evolutionary algorithm to optimize molecular properties such as logP. Molecules are represented as SMILES strings, and crossover/mutation operations are designed to preserve chemical validity. RDKit is used for molecular property evaluation and structure handling.

2. Bayesian Optimization for Molecular Property Prediction
Applies Gaussian Process Regression (GPR) as a surrogate model to efficiently explore the chemical space. The acquisition function (e.g., Expected Improvement) guides the search toward molecules with potentially high logP. The approach balances exploration and exploitation in property optimization.

3. Conditional Generative Models
Develops neural network architectures (such as conditional VAEs) that learn to generate valid molecules given target property constraints. Models are trained using PyTorch, leveraging datasets like ZINC for supervised learning. Emphasis is placed on learning latent representations that align with desired molecular characteristics.

These methods demonstrate how data-driven algorithms can be applied to real-world scientific problems in cheminformatics and computational chemistry.

