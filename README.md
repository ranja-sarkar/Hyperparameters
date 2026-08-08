We need optimally performing models built and maintained for a business, when the business aims to minimize cost, time, etc. The very premise of machine learning relies on a form of function optimization, so inputs can be most accurately mapped to expected output. 

For optimal performance, the model parameters or so-called hyperparameters are tuned. The main techniques of optimization are **random search**, **grid search**, and **Bayesian search**. 

---

Grid search systematically explores all combinations within a predefined grid, while random search randomly samples hyperparameters to cover a range of possibilities. 

The grid search technique is used to place the hyperparameters in a matrix-like structure or a parameter space/grid, and the model is trained on every combination of hyperparameter values. While the grid search looks at every possible combination of hyperparameters, random search selects and tests a random combination of hyperparameter values. Th random search technique randomly samples from a grid of hyperparameters instead of conducting an exhaustive search making grid search an expensive one. We can also specify the number of total runs the random search should try.

<img width="220" alt="ss" src="https://github.com/user-attachments/assets/b922c6b2-48af-4003-a965-fa884e47adda" />

---

**Bayesian optimization** is best when the objective function is complex. The Bayesian process keeps updating the hyperparameter configuration until an optimal point (global minimum) is reached in the search space. 


<img width="449" alt="bo" src="https://github.com/user-attachments/assets/460dc35b-300e-4aa2-90f7-284547ca3d07" />

The different techniques of hyperparameter tuning are discussed in part-III of my [book](https://a.co/d/0bYEq8Qn). 

----

The essential ingredients of a Bayesian optimization algorithm are the surrogate model and the acquisition function. The surrogate model is often a Gaussian Process (GP) that can fit the observed data points and quantify the uncertainty of unobserved areas. We can define an acquisition function is one that provides a single measure of how useful it would be to try any given point, then we can find the point that maximizes this acquisition function and try it next.

<img width="501" height="468" alt="bo" src="https://github.com/user-attachments/assets/7d3ef8ff-c5ff-4ea6-9d4b-7f77d8eb887f" />

The [acquisition function](https://ekamperi.github.io/machine%20learning/2021/06/11/acquisition-functions.html) contains exploitation and exploration terms.

---

Open-source tools for hyperparameter tuning:

1. Ray Tune
2. [Hyperopt](https://github.com/hyperopt/hyperopt)
3. Optuna
4. Scikit-optimize ([skopt](https://pypi.org/project/scikit-optimize/))
5. Scipy.optimize (for gradient-based optimization)
6. [Neural Network Intelligence](https://github.com/microsoft/nni) (NNI - an AutoML toolkit by Microsoft)
7. [BoTorch](https://botorch.org/) by Meta
      
Enterprise tools for hyperparameter tuning:

1. [Vertex AI Vizier](https://cloud.google.com/vertex-ai/docs/vizier/overview) by Google
   
2. [AWS Sagemaker by Amazon](https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning-how-it-works.html)
   
3. [Azure ML by Microsoft](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-tune-hyperparameters?view=azureml-api-2)



