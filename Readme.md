
# Practical Work: Recognizing Iris flowers

## Introduction

This first homework has to do with the classical problem of recognizing different species of Iris flowers relying on the [Iris flower dataset](https://en.wikipedia.org/wiki/Iris_flower_data_set).

The Iris flower data set or Fisher's Iris data set is a multivariate data set introduced by [Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher) in his 1936 paper *"The use of multiple measurements in taxonomic problems as an example of linear discriminant analysis"*.

* The data set consists of 50 samples from each of three species of Iris (*Iris setosa*, *Iris virginica* and *Iris versicolor*).
* Four features were measured from each sample, the length and the width of the sepals and petals, in centimeters.
* Based on the combination of these four features, Fisher developed a linear discriminant model to distinguish the species from each other.

Similarly, we will use this homework to get you familiarized with `numpy` and `scikit-learn`.

<div class="container-fluid">
  <div class="row">
      <div class="col-md-2" align='center'>
      </div>
      <div class='col-md-8' align='center'>
           <img src='https://s3.amazonaws.com/assets.datacamp.com/blog_assets/iris-machinelearning.png' />
      </div>
      <div class="col-md-2" align='center'></div>
  </div>
</div>

## Problem description

**If we want to design an algorithm to recognize iris species, what might the data be?**

* We need a 2D array of size `[n_samples x n_features]`.

    - What would the `n_samples` refer to?
    - What might the `n_features` refer to?

Remember that there must be a **fixed** number of features for each sample, and feature
number ``i`` must be a similar kind of quantity for each sample.

## Loading the Iris Data with `scikit-learn`

`scikit-learn` has a very straightforward set of data on these iris species.  The data consist of
the following:

* Features in the Iris dataset:
  1. sepal length in cm
  2. sepal width in cm
  3. petal length in cm
  4. petal width in cm

* Target classes to predict:
  1. Iris setosa
  2. Iris versicolour
  3. Iris virginica

``scikit-learn`` embeds a copy of the iris CSV file along with a helper function to load it into numpy arrays.

## Your task

* You have the data.
* Modify the Jupyter notebook provided and, in particular,
* you must implement a Multi-Layer Perceptron and **at least one other** machine learning method for recognizing the flowers in the iris dataset.
* Your algorithms must be `scikit-learn` estimators.
* Compare their performance.

Ask yourself some questions:

* What kind of problem is this?
* Must we transform the data?
* How would you implement the train/test/validation cycle for comparing .

### Implementation details

Download the Jupyter notebook from the GitHub repository:

* [https://github.com/rio-group/trabalho-iris-flowers](https://github.com/rio-group/trabalho-iris-flowers).

You can either clone the repository using GitHub Desktop or by doing:
```bash
$ git clone https://github.com/rio-group/trabalho-iris-flowers
```

Alternatively, by directly downloading the repository as a [zip file](https://github.com/rio-group/trabalho-iris-flowers/archive/master.zip).

Please notice the special names that you should use for your classes:


```python
from sklearn.base import BaseEstimator, ClassifierMixin, RegressorMixin
```


```python
# Remember to set the class name appropiately.
class YourNameMLP(BaseEstimator, ClassifierMixin):  # or RegressonMixin?
    def __init__(self, params=None):
        'If params is None the method is initialized with default values.'
        pass

    def predict(self, X):
        'Returns the predictions for every element of X'
        pass

    def fit(self, X, y):
        '''In fit method you should implement all the hard work.
        At first you should check the parameters. Secondly, you should
        take and process the data. Finally you should return self.'''

        # program your MLP backpropagation here.
        return self
```


```python
# Remember to set the class name appropiately.
class YourNameMethodName(BaseEstimator, ClassifierMixin):  # or RegressonMixin?
    def __init__(self, params=None):
        'If params is None the method is initialized with default values.'
        pass

    def predict(self, X):
        'Returns the predictions for every element of X'
        pass

    def fit(self, X, y):
        '''In fit method you should implement all the hard work.
        At first you should check the parameters. Secondly, you should
        take and process the data. Finally you should return self.'''

        # program your MLP backpropagation here.
        return self
```

Bear in mind:

* Prepare the Jupyter notebook describing your work and showing your results -> **plots are expected!**
* Do not used any pre-existing library (like Keras, theano, Tensoflow, etc.) for programming your algorithms.
* You may use them for support but not for the algorithm itself.
* `params` is a dictionary with the configuration of the algorithm: layers, number of nodes in each layer, activation functions, learning rates, etc.
* See `scikit-learn` docs on how to [implement an estimator](http://scikit-learn.org/stable/developers/contributing.html#rolling-your-own-estimator).

# Submission

Submit your notebook files via Google Classroom.
