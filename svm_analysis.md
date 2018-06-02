# Analysis
## 2. Optimized values of Gamma and Cost?

The best values of Gamma and Cost are 0.01 and 1, respectively.

## 3. Applying the tuned model from #3 to the test data. 

Accuracy is 0.84, sensitivity is 0.79, and specificity is 0.87. 

## 4. Comparing (3) results to the results for the random forest and boosted classification tree models

These results are completely either better than or equal to the previous models we created with RF/XGB models. 
The sensitivity of 0.79 around the board isn't great, since it means there are people who have the condition who've 
been told they don't, so there is room for improvement. However, this SVM model is on par with the other models in 
that regard. In overall accuracy, this model soars above the others, beating the best one by 5%. Its specificity, 
clocking at 0.87, is also comparatively superb. From these various performance metrics, we can conclude that the SVM 
is the optimal way to carry out our task, given its speed of training and computation, and the limited dataset we have. 
If we had a much larger dataset, XGBoost would likely be the way to go (as discussed in Asgn. 4), but in this circumstance, 
we can conclude that the Support Vector Machine provides the optimum predictive capabilities that we are looking for. 
