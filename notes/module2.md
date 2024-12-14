# Module 2 

types of regression models 
- simple regression : one independent variable to estimate a dependent variable 
    - simple linear regression 
    - simple non-linear regression 
- multiple regression : more than one independent variable 
    - multiple linear regression 
    - multiple non-linear regression 

regression algorithms 
- ordinal regression 
- poisson regression 
- fast forest quantile regression 
- linear, polynomial, lasso, stepwise, ridge regression 
- bayesian linear regression 
- neural network regression 
- decision forest regression 
- boosted decision tree regression 
- KNN (K-nearest neighbors)

pros of linear regression 
- very fast 
- no parameter tuning 
- easy to understand, and highly interpretable 

model evaluation approaches 
- train and test on same dataset 
    - high training accuracy
        - high training accuracy isn't necessarily a good thing 
        - result of over-fitting 
    - low out of sample accuracy 
        - important that models have a high out of sample accuracy 
- train/test split 
    - still very dependent on dataset 
- K fold cross-validation 
    - performs multiple train/test split 

errors of the model 
- mean absolute error 
- mean squared error 
- root mean squared error 
- relative absolute error 
- relative squared error 
- R squared (not error, but popular metric for accuracy of model)

examples of multiple linear regression 
- independent variables effectiveness on prediction : the strength of the effect that the independent variables have on the dependent variable 
- predicting impacts of changes : predict the impact of changes; how the dependent variable changes when we change the independent variables 

estimating multiple linear regression parameters 
- ordinary least squares 
    - linear algebra operations 
    - problem : time complexity (if rows < 10K)
- optimization algorithm 
    - gradient descent 
    - used if very large dataset 