## Random Forests
Random forest is a collection of decision trees. So instead of depending on a single decision tree one can consider result of a different trees and pick the suitable or most voted one. <br>
Example: If there is 3 decision trees in the forest and 2 of them resulted Yes for a particular situation and rest one resulted No in this case the final result will be Yes. <br>

Randomness depends on dataset or more precisely when different dicision tree works on different data portion. And this data for each decision tree gets selected randomly. There is 2 kind of randomness.
- At a row level
- At a column level

## Gradient Boost
Very flexible non parametric method that can be used for both classification and regression. In this method Each member is an expert of the error of it's predecessor. But it does not perform well when there is only few number of trees. And increasing the number of tree can overcome over fitting problem. I 

## KNN
To find out a class  The “K” is KNN algorithm is the nearest neighbors we wish to take vote from. If K = 3 then need make a circle as center just as big as to enclose only three nearest datapoints on the plane.
