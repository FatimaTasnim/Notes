# Real World ML Pipeline
- Understanding of business problem
- Problem formalization
- Data collecting
- Data preprocessing
- Modeling
- Way to evaluate model in real life
- Way to deploy Model

# Libraries/Frameworks

## Linear Regression
- Scikit-learn
- Vowpal Wabbit: It's designed to handle very large set of data
## Decision Tree
- Scikit learn
- DMLC-XGBoost for higher speed & Accuracy
## KNN-based Methods
- Scikit learn (speeds up calculation)
## Neural Network
- Tensorflow
- K
- dmlc mxnet
- Pytorch (most prefarable, flexible) 
- Lesagne

# Key Points
- Linear models split spaces into 2 subspaces.
- Tree based models splits space into boxs.
- K-NN methods heavily rely on how to measure points "Closeness".
- Feed Forward NNs produce smooth non-linear decision boundaries.

# Some Suggested Algorithm as Prerequisite:
## Random Forests
Random forest is a collection of decision trees. So instead of depending on a single decision tree one can consider result of a different trees and pick the suitable or most voted one. <br>
Example: If there is 3 decision trees in the forest and 2 of them resulted Yes for a particular situation and rest one resulted No in this case the final result will be Yes. <br>
#### Why random??
Randomness depends on dataset or more precisely when different dicision tree works on different data portion. And this data for each decision tree gets selected randomly. There is 2 kind of randomness.
- At a row level
- At a column level
#### Drawbacks:
- Random forests don't train well on smaller dataset
- There is a problem of interpretability with random forest
- Decision trees and hence random forest can't take values outside the training data. 

#### Advantages
- Decrease the chance of overfitting: the bias remains same as that of a single decision tree. However, the variance decreases
- Quick way to do prediction and no need to care about assumptions of the model or linearity in the dataset. 

## Gradient Boosting
Very flexible non parametric methon that can be used for both classification and regression.
#### Advantages
- Work pretty well with heterogeneous data. Where data is featured or measured on a different scales.
- Can use any loss function of choice. No need of any proxy loss function
- Automatically detects (non-linear) feature interactions.
- Can see how predictions are derived.
- Fast to predict.
#### Disadvantages
- Recuires careful tuning
- Slow to train
- cannot extrapolate

*** Gradient boosting can be used for web page ranking. 

#### AdaBoost
- Ensemble: Each member is an expert of the error of it's predecessor
- Iteratively re-weights training examples based on errors 

In AdaBoost over fitting can be reduced.

#### Why should care about features of different types?
- strong connection between preprocessing at our model
- common feature generation methods for each feature type.

#### Feature Processing:
Each type of features has it's own ways to be preprocessed in order to improve quality of the model. And it depends on the model. So, It's another hyparparameter to determine.
#### Feature Generation:
A very powerful technique which can aid significantly in competitions and sometimes provide the required edge 



# Important links for learning: 
- [Random Forests](https://www.datasciencecentral.com/profiles/blogs/random-forests-explained-intuitively)
- [Gradient Boosting](http://arogozhnikov.github.io/2016/06/24/gradient_boosting_explained.html)
- [Gradient Boosted Regression Trees in scikit-learn](https://www.youtube.com/watch?v=IXZKgIsZRm0)
- [k-Nearest Neighbors](https://www.analyticsvidhya.com/blog/2018/03/introduction-k-neighbours-algorithm-clustering/)
- [Scikit-Learn (or sklearn) library](https://scikit-learn.org/stable/)
- [Overview of k-NN (sklearn's documentation)](https://scikit-learn.org/stable/modules/neighbors.html)
- [Overview of Linear Models (sklearn's documentation)](https://scikit-learn.org/stable/modules/linear_model.html)
- [Overview of Decision Trees (sklearn's documentation)](https://scikit-learn.org/stable/modules/tree.html)
- [Overview of algorithms and parameters in H2O documentation](http://docs.h2o.ai/h2o/latest-stable/h2o-docs/data-science.html)
- [Vowpal Wabbit repository](https://github.com/VowpalWabbit/vowpal_wabbit)
- [XGBoost repository](https://github.com/dmlc/xgboost)
- [LightGBM repository](https://github.com/Microsoft/LightGBM)
- [Interactive demo of simple feed-forward Neural Net](http://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.16753&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false)
- [Frameworks for Neural Nets: Keras,PyTorch,TensorFlow,MXNet, Lasagne](https://www.tensorflow.org/)
- [Example from sklearn with different decision surfaces](https://scikit-learn.org/stable/auto_examples/classification/plot_classifier_comparison.html)
- [Arbitrary order factorization machines](https://github.com/geffy/tffm)

[Stand cloud computing, AWS Spot options, Stack and packages](https://www.coursera.org/learn/competitive-data-science/supplement/Djqi7/additional-material-and-links)

