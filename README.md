# Optimizing models

When the business objective is minimizing cost, time, etc. we need an optimally performing model built for the business. For optimal performance, the model hyperparameters are tuned. The main techniques of tuning hyperparameters for optimization are **random search**, **grid search**, and **Bayesian search**. 

Grid search systematically explores all combinations within a predefined grid, while random search randomly samples hyperparameters to cover a range of possibilities. 

The grid search technique is used to place the hyperparameters in a matrix-like structure or a parameter space/grid, and the model is trained on every combination of hyperparameter values. 
While the grid search looks at every possible combination of hyperparameters, random search selects and tests a random combination of hyperparameter values. Th random search technique randomly samples from a grid of hyperparameters instead of conducting an exhaustive search making grid search an expensive one. We can also specify the number of total runs the random search should try.

<img width="220" alt="ss" src="https://github.com/user-attachments/assets/b922c6b2-48af-4003-a965-fa884e47adda" />


The very premise of machine learning relies on a form of function optimization, so inputs can be most accurately mapped to expected output. 
**Bayesian optimization** is best when the objective function is complex. The Bayesian process keeps updating the hyperparameter configuration until an optimal point (global minimum) is reached in the search space. 


<img width="449" alt="bo" src="https://github.com/user-attachments/assets/460dc35b-300e-4aa2-90f7-284547ca3d07" />

The different techniques are discussed in **Chapter 9** of my book. The chapter's title is **exploring optimization techniques** for machine learning.

<img width="179" alt="0" src="https://github.com/user-attachments/assets/2303322f-e4e3-4636-b533-57b38a7ca9ed">

Buy at Amazon: https://a.co/d/iRN1WK5



More about **Hyperparameter tuning in ML using Bayesian Optimization**: https://cloud.google.com/blog/products/ai-machine-learning/hyperparameter-tuning-cloud-machine-learning-engine-using-bayesian-optimization


**Note**: The 'sonar' dataset is used for classification task. The 'auto-insurance' dataset is used for regression task. Look up the **codes** directory.

------

Open-source tools for hyperparameter optimization:

1. Ray Tune
2. Hyperopt
3. Optuna
4. Scikit-optimize (skopt)
5. Scipy.optimize
6. Neural Network Intelligence (NNI - an AutoML toolkit by Microsoft): https://github.com/microsoft/nni
      
Enterprise tools for hyperparameter tuning and model optimization:

1. Vertex AI Vizier by Google: https://cloud.google.com/vertex-ai/docs/vizier/overview
   
2. AWS Sagemaker by Amazon
4. Azure ML by Microsoft

   
