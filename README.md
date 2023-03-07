# Linear Programming Optimization with Python

Linear programming is a mathematical optimization technique used to optimize a linear objective function subject to a set of linear constraints. It involves finding the values of decision variables that minimize or maximize the objective function while satisfying the given constraints.

The objective function and constraints are represented as linear equations or inequalities, and the decision variables are the unknowns that need to be determined. The goal of linear programming is to find the optimal solution that satisfies all the constraints while optimizing the objective function.

1. Formulate a minimization problem

![image](https://user-images.githubusercontent.com/86640902/222190288-79c8d431-b109-41af-9bc6-82b9123f7c31.png)

2. Formulate a maximization problem

![image](https://user-images.githubusercontent.com/86640902/222190342-79b5e4a5-1cad-444e-808a-b379db88e24a.png)

Pulp, Pyomo, Scipy are three popular open-source modeling languages used for formulating and solving linear programming problems. They provide powerful tools for modeling and solving linear programming problems. They offer flexible and intuitive syntaxes for specifying optimization models and can be easily integrated into existing Python-based workflows. Additionally, they both support a wide range of solvers, making it easy to find the best solver for a particular problem.

Please note that I am utilizing the linprog package from the scipy.optimize library for linear programming. It is important to note that linprog solves a minimization problem by default, so to solve a maximization problem, the objective function should be defined as the opposite of its minimization problem.

For example, consider the following linear programming problem:

maximize: y = 𝑥1 + 6𝑥2 subject to:

𝑥1 ≥ 5 (1)

𝑥2 ≤ 4 (2)

80000𝑥1 + 400000𝑥2 ≤ 1600000 (3)

The objective is to maximize the value of y, subject to satisfying the inequalities (1), (2), and (3) by finding the values of x1 and x2 that satisfy these conditions.

This is how you can visualize the problem:

![image](https://user-images.githubusercontent.com/86640902/222184716-4b70b3aa-afe8-406f-8385-10abcb393f9f.png)

The feasible region represents the set of points that satisfy all the constraints. The optimal solution corresponds to the point in the feasible region that maximizes the value of y. The feasible region is the gray area, which represents all possible solutions that satisfy the constraints. There may be an infinite number of feasible solutions, but the optimal solution is the one that maximizes y.

This notebook contains 8 mini problems from various optimization topics. The purpose of these problems is to provide ample practice in formulating optimization problems and gaining familiarity with commonly used optimization packages and solvers (gurobi, cbc, and glpk) in Python.
