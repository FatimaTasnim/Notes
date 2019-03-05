<h1 align = "center"> Feature Preprocessing </h1>
We use preprocessing to scale all features to one scale, so that their initial impact on the model will be roughly similar. 
<h4> KNN Model </h4>
<li> If features are multiplied by zero it results in KNN as ignoring /don't care features </li>
<li> If features are multiplied by 1000000 slightest differences in that features values will impact predictions & this will result in KNN favouring that feature overall others.</li>
<h4>Linear Model</h4>
<p>  Linear models are also experiencing difficulties with differently scaled features.  First, we want regularization to be applied to linear models coefficients for features in equal amount. But in fact, regularization impact turns out to be proportional to feature scale. And second, gradient descent methods can go crazy without a proper scaling. Due to the same reasons, <b>Neural Networks</b> are similar to linear models in the requirements for feature preprocessing.</p>

<b><h2>Outliers</h2></b>
To protect linear models from outliers, we can clip features values between two chosen values of lower bound and upper bound. We can choose them as some percentiles of that feature.

<b><h2>Rank Transformation</h2></b>

Rank transformation is better than MinMaxScaler when we have outliers in the features. So that we can move the outliers closer to the other objects.<br>
If we apply a rank to the source of array, it will just change values to their indices. Now, if we apply a rank to the not-sorted array, it will sort this array, define mapping between values and indices in this source of array, and apply this mapping to the initial array. Linear models, KNN, and neural networks can benefit from this kind of transformation if we have no time to handle outliers manually. Rank can be imported as a random data function from scipy. One more important note about the rank transformation is that to apply to the test data,we need to store the creative mapping from features values to their rank values. Or alternatively, we can concatenate, train, and test data before applying the rank transformation
<h4>Scalers</h4>
<li>MinMaxScaler from sklearn</li>
<li>StandardScaler from sklearn</li>
<li> Rank can be imported as random data function from scipy.</li>
