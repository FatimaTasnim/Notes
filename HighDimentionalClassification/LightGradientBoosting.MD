# Light Gradient Boosting
Light GBM is a gradient boosting framework that uses tree based learning algorithm.Light GBM grows tree vertically while other algorithm grows trees horizontally meaning that Light GBM grows tree leaf-wise while other algorithm grows level-wise. It will choose the leaf with max delta loss to grow. When growing the same leaf, Leaf-wise algorithm can reduce more loss than a level-wise algorithm.


## Advantages
- high speed.
-  large size of data and takes lower memory to run. Another reason of why Light GBM is popular is because it focuses on accuracy

## When to use
- When dataset is large (atleast contains 10000 data)
- Overfitting sensitive to overfitting and can easily overfit small data.

## Parameters
- ###  Control Parameter
    - **max_depth:** This parameter is used to handle model overfitting. So, if model overfits then lower the max depth.
    - **min_data_in_leaf:** It is the minimum number of the records a leaf may have. The default value is 20, optimum value. It is also used to deal over fitting.Generally lower values should be chosen for imbalanced class problems because the regions in which the minority class will be in majority will be very small.
    - **feature_fraction:** Define how many parameter will be randomly selected(0.8==80%). It's for random forest algorithm.
    - **bagging_fraction:** specifies the fraction of data to be used for each iteration and is generally used to speed up the training and avoid overfitting. 
    - **bagging_freq:** Defines how frequently to perform bagging. bagging_freq = k means perform bagging at every k iteration.
     Smaller fractions and frequencies reduce overfitting. **to enable bagging, bagging_fraction should be set to value smaller than 1.0.**
    - **lambda:** lambda specifies regularization. Typical value ranges from 0 to 1.
    - **min_gain_to_split:** This parameter will describe the minimum gain to make a split. It can used to control number of useful splits in tree.
- ### Core Parameters
    - **task:** It specifies the task to perform on data. It may be either train or predict.
    - **application:** regression/binary/multiclass
    - **boosting:** gbdt/rf/dart( Dropouts meet Multiple Additive Regression Trees)/goss(Gradient-based One-Side Sampling)
    - **num_boost_round:** Number of boosting iterations, typically 100+
    - **learning_rate:** This determines the impact of each tree on the final outcome. GBM works by starting with an initial estimate which is updated using the output of each tree. The learning parameter controls the magnitude of this change in the estimates. Typical values: 0.1, 0.001, 0.003
    - **num_leaves:** number of leaves in full tree, default: 31
    - **device:** default: cpu, can also pass gpu.
- ### Metric Parameters:
    - **mae:** mean absolute error
    - **mse:** mean squared error
    - **binary_logloss:** loss for binary classification
    - **multi_logloss:** loss for multi classification