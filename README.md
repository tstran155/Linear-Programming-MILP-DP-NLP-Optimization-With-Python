# Dynamic Programming (DP) and Nonlinear Programming (NLP) Optimization with Python 

1. Dynamic Programming

Dynamic Programming is a method for solving complex problems by breaking them down into simpler subproblems. It is used when a problem can be divided into overlapping sub-problems, and the overall solution can be constructed from solutions of these sub-problems. DP is especially powerful for problems that can be described by a set of recursive equations.

Typical applications of NLP are to (1) Develop algorithms like Fibonacci number calculation, shortest path problems (e.g., Bellman-Ford), knapsack problems, and many others in operations research, and (2) Optimize portfolio and decision-making processes where outcomes are based on previous decisions.

2. Nonlinear Programming

NLP involves optimizing a nonlinear objective function subject to nonlinear constraints. Unlike linear programming, which can be efficiently solved, NLP problems are generally more complex and can have multiple local optima rather than a single global optimum.

Typical applications of NLP are in (1) Engineering design problems where the behavior of a system is nonlinear, (2) Economics and finance for utility maximization and cost minimization where effects are non-linear, and (3) Machine learning in training neural networks, where weight adjustment often involves nonlinear optimization.

3. DP vs. NLP

- DP solves problems with a recursive breakdown and is highly effective for combinatorial optimization and where decisions are staged over time. 

- NLP solves problems where relationships between variables are nonlinear and are often used in continuous space optimization. It uses a deterministic, recursive methodology that builds solutions by combining solutions to subproblems. 

- NLP generally uses numerical methods that require calculations of derivatives and iterative refinement, while DP is ideally suited for problems characterized by stages or sequences, like resource allocation over time, whereas NLP is suited for optimizing systems and processes that are modeled with nonlinear equations.

This notebook contains 2 mini problems to demonstrate the DP and NLP optimization techniques. The purpose of these problems is to provide ample practice in formulating optimization problems and gaining familiarity with commonly used optimization packages and solvers in Python.
