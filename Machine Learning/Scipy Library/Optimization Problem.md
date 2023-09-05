The problem is to determine the optimal r and h for a cococola bottle when the company require a volume of 330 inch^3. Consider the bottle to be a cylinder.

Solution:

This is one of the convex optimization problem where we are minimizing the r and h values by minimizing the surface area of the bottle minimal. The minimum surface area
means minimum production cost. Thus resulting in least material for the bottle.

### Python Solution
```
import numpy as np
from scipy.optimize import minimize

# Function for calculating the surface area of a cylinder.
def surface_area(x):
    r, h = x
    return 2*np.pi*r**2 + 2*np.pi*r*h

# Function for the ares of a cylinder is taken as the constraint.
def constraint(x):
    r, h = x
    return np.pi*r**2*h - 330

# Initial guess for r and h
x0 = [1, 1]

# Define the optimization problem
problem = {
    'fun': surface_area,
    'x0': x0,
    'constraints': [{'type': 'eq', 'fun': constraint}],
    'method': 'SLSQP'
}

# Solve the optimization problem
result = minimize(**problem)

# Extract the optimal values of r and h
r_optimal, h_optimal = result.x

print("Optimal values:")
print("r =", r_optimal)
print("h =", h_optimal)

"""Output
Optimal values:
r = 3.7449402246284995
h = 7.489870114127434

Fun fact : The height of 7.4" is the actual height of a 8 oz cococola bottle.
"""
```
