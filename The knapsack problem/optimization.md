# Gradient & Hessian

Gradient is the vector of first order derivatives of a scalar field. A gradient guides you with the direction in a landscape.

<img width="566" alt="111" src="https://github.com/user-attachments/assets/bc5cec50-65ed-4dd1-b128-8e1addb64fac" />

Hessian is a matrix of second order partial derivatives of a scaler field. A Hessian not only guides, it also tells if you're climbing, falling, or stuck in the landscape.

<img width="419" alt="222" src="https://github.com/user-attachments/assets/15dae48a-d29a-40a3-b5fd-7637cb8b55cb" />

Jacobian is a matrix of gradients of a vector field.

<img width="574" alt="333" src="https://github.com/user-attachments/assets/c5540b9c-e925-4307-bb65-8437720526eb" />


# Classification of Optimization Problems

Optimization uses a rigorous mathematical model to determine the most efficient solution to a described problem. 

One must first identify an objective function, a quantitative measure of the model examples of which are profit, cost, energy. The objective is subject to constraints such as resources, time. 

 1. **Linear Programming (LP)** ->  Objective function and constraints are both linear
 
 2. **Quadratic Programming (QP)** -> Objective function is quadratic and constraints are linear
 
 3. **Non-Linear Programming (NLP)** -> Objective function or (atleast one) constraint is non-linear

<img width="410" alt="12" src="https://github.com/user-attachments/assets/4e9e2682-676f-4aeb-8b72-3a9af557bc6f" />




# LP example

 **Objective function**:
 
 1. Goal is to maximize total profit
 2. Products A and B are sold at 25$ and 20$ respectively

    
 **Constraints**:
 
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

Optimal x1 and x2 are 45 and 75 respectively.

Blog on LP in python: https://mlabonne.github.io/blog/posts/2022-03-02-Linear_Programming.html


# QP example

Portfolio optimization: https://www.cvxpy.org/examples/basic/quadratic_program.html

Convex optimization: https://www.cvxpy.org/

In my book (**chapter 4**), I have briefly touched upon convex functions and their optimization.

<img width="173" alt="rr" src="https://github.com/user-attachments/assets/60c42c5e-e9d8-4223-9b75-c5f7b356911e" />

Buy from Amazon: https://a.co/d/6U6Q6WT

An excerpt from the book:

<img width="402" alt="16" src="https://github.com/user-attachments/assets/34ae602c-6954-4c89-92d3-a737ab992bc2" />

When we talk about convex and non-convex functions, we think of the **Hessian**. The Hessian matrix has two important utilities:
- to know whether a function is concave or convex

<img width="562" alt="22" src="https://github.com/user-attachments/assets/c2114793-4dd7-43df-b504-9019046439ad" />
  
- to determine whether a critical point is a local minimum, a local maximum, or a saddle point [If the gradient of a function is zero at some point, that is f(x)=0, then function f has a critical point at x]


<img width="563" alt="11" src="https://github.com/user-attachments/assets/d2ddebdb-e5a9-49e8-b5cd-45ea0065f09d" />


<img width="199" alt="pp" src="https://github.com/user-attachments/assets/85c5f867-00f3-4750-bc4e-7c63b06d87a9" />


In general, QP in python: https://scaron.info/blog/quadratic-programming-in-python.html

# NLP example


<img width="425" alt="12" src="https://github.com/user-attachments/assets/3226387d-f786-4df7-a43a-b965595c6d87" />


Solving nonlinear optimization problems with multiple python libraries: 

https://github.com/marcelcases/nonlinear-optimization

NLP with python: https://paulminogue.com/posts/a0d8c837-a40d-4b17-9d30-e0bd36a6befc

