# Optimizing models

When it comes to minimizing costs in a business, what we need is an optimized business model. The right hyperparameter tuning technique impacts the model performance, and the model performing optimally is the one that helps achieve the business objective it's built for. The main techniques of tuning model hyperparameters for optimization are **random search**, **grid search**, and **Bayesian search**. 

Grid search systematically explores all combinations within a predefined grid, while random search randomly samples hyperparameters to cover a range of possibilities. An illustrative image is given below.

![1](https://github.com/user-attachments/assets/b6f9b380-02e9-4cac-8834-d7e697c4dc5d)

The different techniques are discussed in **Chapter 9** of my book. The chapter's title is **exploring optimization techniques** for machine learning.

<img width="179" alt="0" src="https://github.com/user-attachments/assets/2303322f-e4e3-4636-b533-57b38a7ca9ed">

Buy at Amazon: https://a.co/d/iRN1WK5

The very premise of machine learning relies on a form of function optimization, so inputs can be most accurately mapped to expected output. 
**Bayesian optimization** is best when the objective function is complex. This process keeps updating the hyperparameter configuration until an optimal point (global minimum) is reached in the search space.

<img width="209" alt="1" src="https://github.com/user-attachments/assets/88535300-9262-4298-b93a-d27e7bba2752">

<img width="62" alt="3" src="https://github.com/user-attachments/assets/cb96346e-1362-4c36-a7de-2372f95496ec">


**Note**: The 'sonar' dataset is used for classification task. The 'auto-insurance' dataset is used for regression task. Look up the **codes** directory.

