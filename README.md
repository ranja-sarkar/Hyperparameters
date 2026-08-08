We need optimally performing models built for the business, when the business aims to minimize cost, time, etc. For optimal performance, the model parameters or so-called hyperparameters are tuned. The main techniques of optimization are **random search**, **grid search**, and **Bayesian search**. 

The very premise of machine learning relies on a form of function optimization, so inputs can be most accurately mapped to expected output. 

---

Grid search systematically explores all combinations within a predefined grid, while random search randomly samples hyperparameters to cover a range of possibilities. 

The grid search technique is used to place the hyperparameters in a matrix-like structure or a parameter space/grid, and the model is trained on every combination of hyperparameter values. While the grid search looks at every possible combination of hyperparameters, random search selects and tests a random combination of hyperparameter values. Th random search technique randomly samples from a grid of hyperparameters instead of conducting an exhaustive search making grid search an expensive one. We can also specify the number of total runs the random search should try.

<img width="220" alt="ss" src="https://github.com/user-attachments/assets/b922c6b2-48af-4003-a965-fa884e47adda" />

---

**Bayesian optimization** is best when the objective function is complex. The Bayesian process keeps updating the hyperparameter configuration until an optimal point (global minimum) is reached in the search space. 


<img width="449" alt="bo" src="https://github.com/user-attachments/assets/460dc35b-300e-4aa2-90f7-284547ca3d07" />

The different techniques of hyperparameter tuning are discussed in part-III of my [book](https://a.co/d/0bYEq8Qn). 

----

The essential ingredients of a Bayesian optimization algorithm are the surrogate model and the acquisition function. The surrogate model is often a Gaussian Process that can fit the observed data points and quantify the uncertainty of unobserved areas. We can define an acquisition function is one that provides a single measure of how useful it would be to try any given point, then we can find the point that maximizes this acquisition function and try it next in iterations.

---

Open-source tools for hyperparameter optimization:

1. Ray Tune
2. Hyperopt
3. Optuna
4. Scikit-optimize (skopt)
5. Scipy.optimize
6. [Neural Network Intelligence](https://github.com/microsoft/nni) (NNI - an AutoML toolkit by Microsoft)
      
Enterprise tools for hyperparameter tuning and model optimization:

1. Vertex AI Vizier by Google: https://cloud.google.com/vertex-ai/docs/vizier/overview
   
2. AWS Sagemaker by Amazon
4. Azure ML by Microsoft

**Hyperparameter Tuning in the Cloud**: 

https://cloud.google.com/blog/products/ai-machine-learning/hyperparameter-tuning-cloud-machine-learning-engine-using-bayesian-optimization   


