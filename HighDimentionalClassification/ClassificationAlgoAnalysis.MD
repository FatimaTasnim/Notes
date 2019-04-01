# Classification Algorithms
- Neural Network
- Linear Discriminant analysis
- Support Vector Machine
- Boosting
- Random Forest.

# Curse of dimentionality
- The best Error was achieved using finite numbers of features.
- Using an infinite number of features test error degreads to the accuracy of random guessing
- The optimal dimentionality increase with incresing sample size.

# Suppport Vector Machine
## Hard Margin Support Vector Machine
 Standard
SVM construct a hyperplane, also known as decision boundary, that best divides the input space χ into two disjoint regions.The higher the value of the C multiplier, the more SVM will be sensitive to noise. In the limit where C goes to positive infinite,will have a hard-margin SVM. Hard-margin SVM will try to find a separating hyper-plane that has maximum distance from either classes' data points, such that all the data points in each side of the hyper-plane should be of the same class. This constraint might make problem unsolvable, i.e. SVM can't find a hyper-plane to separate data points perfectly, or equally, the optimization problem doesn't have an answer.Hard margin SVM can work only when data is completely linearly separable without any errors (noise or outliers). In case of errors either the margin is smaller or hard margin SVM fails.

## Soft Margin Support Vector Machine
Soft margin SVM can overcome overfitting problem. Soft margin works when data are not linearly seperable.
## Kernel Support Vector Machine
SVM algorithms use a set of mathematical functions that are defined as the kernel. The function of kernel is to take data as input and transform it into the required form. Different SVM algorithms use different types of kernel functions. These functions can be different types. For example linear, nonlinear, polynomial, radial basis function (RBF), and sigmoid.
**Observations were reported in the field of document classification,
where SVM were trained directly on the original high dimensional input space. Kernel SVM (gaussian and polynomial kernels) were employed and compared with other conventional classifiers like k-NN classifiers, Naive-Bayes Classifier, Rocchio Classifier and Decision Tree Classifier. The results show that Kernel SVM outperform the traditional classifiers.**

# Feature Selection Methods
The goal of feature selection techniques is to find an optimal set of features based on different measures of optimality.Irrespective of the measure of optimality, the selected subset of features should ideally possess the following characteristics

- The cardinality of the subset should be minimal such that it is necessary and
sufficient to accurately predict the class of unknown samples,
- The subset of features should improve the prediction accuracy of the classifier
run on data containing only these features rather than on the original dataset
with all the features,
- The resulting class distribution, given only the values for the selected features,is as close as possible to the original class distribution given all feature values.

Based on the above feature characteristics, it is obvious that irrelevant features would not be part of the optimal set of features.

Features are defined as
- Irrelevance
- Strong relevance
- Weak relevance
- Markov Blanket
- Redundant feature

# References
- [Paper- High Dimentional Data Classification](https://www.researchgate.net/publication/248149710_High_Dimensional_Data_Classification)
- [Soft-Hard SVM](https://www.researchgate.net/post/Can_anyone_explain_to_me_hard_and_soft_margin_Support_Vector_Machine_SVM)
- [SVM blog](https://blog.statsbot.co/support-vector-machines-tutorial-c1618e635e93)