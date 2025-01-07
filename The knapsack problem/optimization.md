
# Classification of Optimization Problems
 
 1. **Linear Programming (LP)** ->  Objective function and constraints are both linear
 
 2. **Quadratic Programming (QP)** -> Objective function is quadratic and constraints are linear
 
 3. **Non-Linear Programming (NLP)** -> Objective function or atleast one constraint is non-linear

<img width="410" alt="12" src="https://github.com/user-attachments/assets/4e9e2682-676f-4aeb-8b72-3a9af557bc6f" />


Optimization uses a rigorous mathematical model to determine the most efficient solution to a described problem. One must first identify an objective function which is a quantitative measure of the model performance. Examples: profit, cost, energy. The objective is subject to constraints for example, resource, time. 

# LP example

 Objective function:
 1. Goal is to maximize total profit
 2. Products A and B are sold at 25$ and 20$ respectively
 Constraints:
 1. Product A requires 20 resource units, product B 12 units
 2. Only 1800 resource units are available per day
 3. Both products require a production time of 1/15 hour
 4. A working day has a total of 8 hours.

**Mathematical Formulation:**

Objective function maximizes total sales. 

<img width="168" alt="13" src="https://github.com/user-attachments/assets/d225fbc3-289d-4983-8f5a-124f4b2d5e0e" />

Resource and time constraints are given by:

<img width="353" alt="14" src="https://github.com/user-attachments/assets/9913411c-25df-48f5-90e0-0c1e5aa5d3f1" />


x1 = #items of product A, x2 = #items of product B


<img width="389" alt="15" src="https://github.com/user-attachments/assets/0bff54c7-e77b-4961-95e3-143b3753a6d4" />


# QP example

Portfolio optimization: https://www.cvxpy.org/examples/basic/quadratic_program.html

In general, QP in python: https://scaron.info/blog/quadratic-programming-in-python.html

# NLP example

<img width="425" alt="12" src="https://github.com/user-attachments/assets/3226387d-f786-4df7-a43a-b965595c6d87" />


