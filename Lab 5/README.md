## Task 1 -- Feature Engineering Explanation

A new feature, **price_per_item**, was created by dividing **Total_Price** by **Quantity**. 
This represents the average cost per item in an order and normalizes price across 
orders of different sizes. Higher values may indicate premium meals that require 
longer preparation times, while lower values may reflect simpler or fast-food orders. 
This feature helps the model capture pricing patterns that may influence **Order_Status**.


## Task 4 -- Feature Selection Explanation

Feature selection was applied using a model‑based approach with
**RandomForestClassifier** and **SelectFromModel**. The selector keeps
only features with importance scores above the median importance of the
trained model. After reducing the feature set, the model was retrained
using only the selected features and the new accuracy was compared with
the original model.

In this case, feature selection helped simplify the model by removing
less informative variables while keeping the most predictive features.
Although the accuracy improvement may be small or sometimes unchanged,
the model becomes easier to interpret and computationally more
efficient. Reducing the number of features can also help prevent
overfitting and make the model more robust when applied to new data.
