# Packing

The goal of packing problems is to find an optimal way to pack a set of items of given sizes into containers with fixed capacities. 
A typical application is loading boxes onto delivery trucks efficiently. It is not often possible to pack all the items, due to the capacity constraints. 
In that case, the problem is to find a subset of the items with maximum total size that will fit in the containers. The most known packing problem is **the knapsack problem**.

**Chapter 9** of my book discusses optimization in Operations Research (OR) and the knapsack problem is elaborated.

<img width="179" alt="0" src="https://github.com/user-attachments/assets/2303322f-e4e3-4636-b533-57b38a7ca9ed">


This kind of packing problems falls under **integer optimization** or integer linear programming. https://developers.google.com/optimization/mip


For more packing problems and their optimization, please refer: https://developers.google.com/optimization/pack

The knapsack data (excerpt from the book):

<img width="407" alt="ksp" src="https://github.com/user-attachments/assets/76d4eb16-4bad-4446-ad86-78b404aa07ba">


The solution using PuLP (https://pypi.org/project/PuLP/) has been shown in the book. 

Google OR-Tools: https://developers.google.com/optimization/introduction/python

