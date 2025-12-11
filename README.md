Overparameterization and Double Descent: Rethinking Model Complexity and Generalization
Overview

This repository contains the code and accompanying tutorial developed for a university machine learning assignment exploring the relationship between model capacity and generalization performance. The project focuses on the phenomenon of overparameterization and double descent, which challenges the classical bias–variance trade-off by demonstrating that increasing model size beyond the interpolation threshold can, in some settings, improve generalization.

The tutorial combines theoretical analysis with controlled empirical experiments to illustrate how training error, test error, and interpolation behaviour change as model capacity increases.

Repository Structure
├── notebooks/
│   └──srinidha_ml_code.ipynb
│
├── figures/
│   └── (generated plots used in the tutorial)
│
├── 
├── README.md
└── LICENSE

Topic Focus

Model family: Polynomial regression / neural network models
Core concept: Double descent and overparameterization

The tutorial investigates:

the classical bias–variance trade-off

the interpolation threshold

non-monotonic test error behaviour

differences between underparameterized, interpolating, and overparameterized regimes

limitations of classical generalization intuition

The goal is to provide conceptual clarity on why large modern models can generalize well despite having more parameters than training samples.

Dataset

A synthetic supervised learning dataset is generated to allow full control over noise and sample size.

Small training set to expose the interpolation regime

Smooth underlying target function

Additive noise to induce realistic generalization challenges

This setup is designed to make changes in generalization behaviour observable as model capacity varies.

Requirements

The code was developed using Python 3.9+.
Required libraries:

pip install numpy matplotlib pandas scikit-learn

How to Run

Clone the repository:

git clone 

Navigate to the notebooks directory:

cd double-descent/notebooks


Launch the Jupyter Notebook:

jupyter notebook double_descent_experiment.ipynb


Run all cells sequentially to reproduce:

training and test error curves

plots illustrating the interpolation threshold

example model predictions

results tables used in the tutorial

All figures in the report are generated directly from this notebook.

Experimental Design Notes

Model capacity is varied systematically while all other factors are held constant

No explicit regularization is applied

Models are trained until interpolation is achieved where possible

Results are evaluated using mean squared error

This design isolates the effect of overparameterization on generalization.

Accessibility Considerations

Plots use high-contrast, colour-blind–safe palettes and clear axis labels. Tables present numerical values directly without relying on colour encoding. The tutorial document uses structured headings to support screen readers.

License

This repository is released under the MIT License. It may be used, modified, and redistributed with appropriate attribution.
