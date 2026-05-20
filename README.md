# Gradient Methods for Semi-Supervised Learning

Academic project developed for the Optimization for Data Science course at the University of Padova.
The project studies the application of first-order optimization methods to a graph-based semi-supervised learning problem for binary classification.
Different gradient-based optimization algorithms and Block Coordinate Gradient Descent (BCGD) strategies were implemented and compared in terms of convergence behavior, computational efficiency and classification performance on both synthetic and real datasets.

## Implemented Methods
The following optimization methods were analyzed and compared:

### Gradient-Based Methods
- Gradient Descent with Fixed Step Size
- Gradient Descent with Exact Line Search
- Gradient Descent with Armijo Rule
- Heavy Ball Gradient Descent
- Accelerated Gradient Descent (Nesterov)
- Gradient Descent with Improved Rate

### Coordinate Descent Methods
- Gauss-Southwell BCGD with Exact Line Search
- Gauss-Southwell BCGD with Fixed Step Size

## Problem Formulation
The project focuses on a graph-based semi-supervised learning framework where only a small subset of samples is labeled.
The optimization objective encourages:
- consistency between labeled and unlabeled samples
- smoothness across similar unlabeled points

The resulting optimization problem is quadratic, strongly convex and solved through different first-order optimization techniques.

## Datasets

Experiments were conducted on:
- Synthetic datasets with isotropic and anisotropic clusters
- Breast Cancer Wisconsin Diagnostic Dataset (UCI)

The analysis evaluates:
- loss trajectories
- convergence speed
- runtime efficiency
- classification accuracy

## Main Findings

- Accelerated Gradient Descent and Heavy Ball achieved the best convergence behavior
- Momentum-based methods significantly improved optimization speed
- Exact line search methods provided stable but computationally expensive convergence
- Gauss-Southwell BCGD methods achieved competitive performance in high-dimensional settings
- Coordinate descent approaches reduced computational overhead while preserving accuracy

## Technologies
- Python
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook
- Convex Optimization
- Semi-Supervised Learning

## Authors
- Francesco Ceron
- Emanuele Cavaliero


code/
└── Finale.ipynb
