# Maths - Mathematical Experiments

A repository for exploring mathematical concepts, particularly linear algebra, dynamical systems, and numerical methods.

## Overview

This repository contains Jupyter notebooks for experimenting with mathematical concepts and implementations. Based on educational content from Steve Brunton's lectures and other mathematical resources.

## Contents

### Steve Brunton E3 - Weather Model

A Jupyter notebook implementing a Markov chain weather model that demonstrates:
- **Matrix Operations**: Using NumPy for linear algebra
- **Markov Chains**: State transition matrices
- **Convergence**: Observing system convergence to steady state
- **Visualization**: Plotting state evolution over time

The model simulates weather state transitions (likely sunny/cloudy/rainy) using a transition matrix and shows how the system converges to a steady-state probability distribution.

## Concepts Explored

- **Linear Algebra**: Matrix multiplication, state vectors
- **Dynamical Systems**: Iterative state updates
- **Markov Chains**: Probabilistic state transitions
- **Steady-State Convergence**: Long-term behavior of systems
- **Numerical Methods**: Iterative computation

## Technologies

- **Python 3**
- **NumPy**: Numerical computing
- **Matplotlib**: Data visualization
- **Jupyter Notebook**: Interactive computing environment

## Installation

```bash
# Clone the repository
git clone https://github.com/DanielBryars/maths.git
cd maths

# Install dependencies
pip install numpy matplotlib jupyter
```

## Usage

```bash
# Start Jupyter
jupyter notebook

# Open "Steve Brunton E3 - Weather Model.ipynb"
```

## Example: Weather Model

The notebook demonstrates a 3-state weather model:

```python
import numpy as np

# Transition matrix
A = np.array([[0.5,0.5,0.25],
              [0.25,0.0,0.25],
              [0.25,0.5,0.5]])

# Initial state
xtoday = np.array([[1],[0],[0]])

# Iterate to see convergence
xtomorrow = A @ xtoday
```

The system converges to steady state: [0.4, 0.2, 0.4]

## Learning Resources

Based on content from:
- **Steve Brunton**: Control Theory, Dynamical Systems, and Machine Learning educator
- Linear algebra fundamentals
- Markov chain theory

## Topics to Explore

- Eigenvalues and eigenvectors
- Differential equations
- Optimization methods
- Numerical analysis
- Probability theory
- Data-driven modeling

## Status

Active learning repository for mathematical exploration and experimentation.

## References

- Steve Brunton's YouTube channel and lectures
- Gilbert Strang's Linear Algebra resources
- NumPy documentation
