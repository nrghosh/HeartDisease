# Comparison Analysis
## 1. Model Preference

Based on the results, I prefer the Random Forest model. Not only is it more accurate (0.79) than the XGBoost counterpart (0.71), but it has a higher measure of specificity (0.795 compared to 0.64) and equivalent sensitivity as the XGBoost model. In addition, the Random Forest model was much faster to train and processes than the XGBoost equivalent.

## 2. How would you suggest these findings be used?

These findings would definitely be useful to hospitals so that they could prioritize patients based on risk factors and be aware of the misclassifications that could occur. The false negatives are obviously more serious, as they result in those affected not getting treatment- examining these false negatives more closely could help hospitals tune and optimize their screening processes, so that they can identify risky individuals with higher accuracy.


# Theoretical Points
## 1. Similarities between Random Forest and Gradient Boosted Tree approaches

They are both obviously ensemble approaches to decision trees, utilizing the base model of a decision tree as their common estimator. Both processes involve creating a distribution of sub-models that work on subsets of the original "problem", or data, then aggregating said distribution into one cohesive model.


## 2. Differences between Random Forest and Boosted Regression Tree approaches

In general, a BRT model takes longer than a RF model to train and utilize. They also have different approaches to sampling and different goals, reflected in the techniques they use. Random forests use bagging (bootstrapped aggregating) as a sampling technique and use parallel ensembling. Also, Random Forests are low-bias, high-variance type models, and attempt to reduce variance. Compare this to Boosted Regression Trees, which are high-bias, low-variance type models and attempt to reduce bias, while using Boosting as a sampling technique, as well as sequential ensembling. In addition, Boosted Trees have a handful of hyperparameters that require tuning, while Random Forests require practically no tuning. We expect Boosted Regression Trees to perform better than Random Forests in general- one reason that this hypothesis could have been contradicted by our experimental model results is that our dataset was comparively small. 
