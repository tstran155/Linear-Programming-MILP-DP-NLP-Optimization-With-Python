# Linear Programming and Mixed-Integer Linear Programming Optimization with Python

Mixed Integer Linear Programming extends LP to include cases where some or all of the decision variables are required to be integers. This is particularly useful in scenarios where decisions involve discrete units (like numbers of plants, machines, or hectares in your case). MILP is ideal for scenarios requiring discrete decisions. For this rice planting problem, this would mean specifying the exact number of hectares for each type of rice in each field type, which cannot realistically be fractional. It can model a wide range of practical problems more accurately than LP when integer constraints are involved.

On the flip side, solving MILP problems is generally more computationally intensive than LP. This is because the integer constraints make the problem NP-hard, leading to potentially longer solve times and higher computational resource usage. As the size of the problem (number of variables and constraints) grows, MILPs can become significantly harder to solve optimally.

1. Problem formulation
   
- Let's define the variables: 𝑥𝑖𝑗 = hectares of rice type
 
Where 𝑖 ranges over field types (I, II, III) and j ranges over rice types (IR8, CBC, IR132).

- The constraints based on the total hectares available for each rice type are:
![rice type](https://github.com/tsujit139/Linear-Programming-Optimization-With-Python/assets/130299613/dd6c4008-e305-4f91-adee-1184313910e9)


- And the constraints based on the total hectares available for each field type are:
![field type](https://github.com/tsujit139/Linear-Programming-Optimization-With-Python/assets/130299613/037278d0-f871-4b18-b7fd-587f72cc28ef)


- The objective function to maximize the total yield (in tons) is:
![objective function](https://github.com/tsujit139/Linear-Programming-Optimization-With-Python/assets/130299613/971e07eb-63b2-4191-ae74-5723711ab4b7)


Maximize 
​
2. MILP formulation
This problem is linear as the objective and constraints are linear relations. MILP is suitable in case integer constraints on the 𝑥𝑖𝑗 variables (assuming that only whole hectares can be allocated). If the variables can be fractional, a simple linear programming approach would suffice.
