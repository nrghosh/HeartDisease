# Part 4: Comparing
##1. Based on the results in Part II, III, which model do you prefer? Justify your answer.

Based on the results in parts 2 and 3, I prefer the Random Forest model. Not only is it more accurate (0.79) than the XGBoost counterpart (0.71), but it has a higher measure of specificity (0.795 compared to 0.64) and equivalent sensitivity as the XGBoost model. In addition, the Random Forest model was much faster to train and processes than the XGBoost equivalent.

##2. How would you suggest these findings be used?

These findings would definitely be useful to hospitals so that they could prioritize patients based on risk factors and be aware of the misclassifications that could occur. The false negatives are obviously more serious, as they result in those affected not getting treatment- examining these false negatives more closely could help hospitals tune and optimize their screening processes, so that they can identify risky individuals with higher accuracy.


# Part 5: Theoretical Discussion
##1. In general, what are the similarities between a Random Forest and a Boosted Regression Tree approach?

They are both obviously ensemble approaches to decision trees, utilizing the base model of a decision tree as their common estimator. Both processes involve creating a distribution of sub-models that work on subsets of the original "problem", or data, then aggregating said distribution into one cohesive model.


##2. In general, what are the differences between a Random Forest and Boosted Regression Tree approach?

In general, a BRT model takes longer than a RF model to train and utilize. They also have different approaches to sampling and different goals, reflected in the techniques they use. Random forests use bagging (bootstrapped aggregating) as a sampling technique and use parallel ensembling. Also, Random Forests are low-bias, high-variance type models, and attempt to reduce variance. Compare this to Boosted Regression Trees, which are high-bias, low-variance type models and attempt to reduce bias, while using Boosting as a sampling technique, as well as sequential ensembling. In addition, Boosted Trees have a handful of hyperparameters that require tuning, while Random Forests require practically no tuning. We expect Boosted Regression Trees to perform better than Random Forests in general- one reason that this hypothesis could have been contradicted by our experimental model results is that our dataset was comparively small. 
