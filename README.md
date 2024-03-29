# Two-fluid model sample code

Repository containing code for dynamic simulations of two-phase flows in pipes using the two-fluid model and finite element methods.

## Description 

This code consists of a unified framework for performing transient simulations and stability analysis of two-phase flows using the one-dimensional averaged Navier-Stokes equations, frequently employed in sizing and monitoring pipelines and receiving facilities of the oil and gas industry. This code simulates liquid wave growth by considering stratified flows as the initial conditions.

This code version uses the finite element method for constructing fully-discrete flow pattern maps by resolving the linearized equations and performing linear stability analysis. Also, the capability of the numerical formulation for describing wave growth is accomplished through stiffness analysis of the semi-discrete equations, which reveal the influence of convection and acoustic modes on flow stability and consequent liquid wave growth.

After formulating the variational problem, the [FEniCS Project](https://fenicsproject.org/) library is employed to construct the basis functions, solve the integral functions on the element level, and assemble the system matrix. The system matrix is solved through the Newton method and the eigenvalue problem through the ARPACK library. The code is written in the Python 3 language.


## Requirements

The code requires Python 3.5 or higher, NumPy, SciPy, Matplotlib, math, and FEniCS.


## FEniCS Project platform

(base) root@MacBook twofluidmodel # conda activate fenicsproject

