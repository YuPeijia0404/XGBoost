# XGBoost
## Bagging
* Data -> several models -> several predictions -> final perdiction by weighted average
### Bagging vs Boosting
* Bagging
    * Leverages unstable base learners that are weak because of <font color=red>overfitting </font>
    * Leverages unstable base learners that are weak because of <font color=red>underfitting</font>
## Boosted Tree
#### Based on residual(残差)
* Use residual of <font color=red>y</font> as the y of next model
    * y = y(origin) - y1 - y2 - y3
    * The final prediction is the sum of each <font color=red>y</font>
    * Sum instead of weighted average
#### Multiple trees for predictions
* The i-th sample's final prediction based on K trees
![avatar](/img/finprediction.png)
* Construction of the objective function
![avatar](/img/objectivefunction.png)
    * loss function -> `l(y_actual, y_predict)` + penalty / regulation -> expressed by parameters
    * Minimise the objective function



