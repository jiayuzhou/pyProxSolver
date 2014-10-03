pyProxSolver
============

A proximal optimization solver in Python for solving objectives including a smooth and a non-smooth part. 
If the objective is a convex one, the solver gives a optimal solution. 
For an objective `min_x f(x)+g(x)`, one needs to provide a function that computes the function value 
of the objective `f(x)` and its gradient `\nabla f(x)`, and another function computes the proximal operator 
associated with `g(x)`: `min_x ||x - x'|| + g(x)`, given `x'`.
