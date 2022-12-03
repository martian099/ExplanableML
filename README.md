# ExplanableML
## Use shap to find key predictor in XGBoost
This notebook aims to provide an example on how to use shap algorithm to explain the output of ensemble tree models.

Here I created a dataset with 4 predictors x1, x2, x3 and x4, and the dependent variable y = 3*x1 + x2 + 0.1*x3. Notice here x4 is not used so y has no correlation with x4.

The shap algorithm should be able to pick out that x1 is the most important predictor, followed by x2 and x3. And x4 should have no predictive power. 

As seen in the last plot that is exactly what shap tree explainer output plot shows. 
