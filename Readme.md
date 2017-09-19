
# Practical Work: Recognizing Iris flowers

# Introduction

This first homework has to do with the classical problem of recognizing different species of Iris flowers relying on the [Iris flower dataset](https://en.wikipedia.org/wiki/Iris_flower_data_set).

The Iris flower data set or Fisher's Iris data set is a multivariate data set introduced by [Ronald Fisher](https://en.wikipedia.org/wiki/Ronald_Fisher) in his 1936 paper *"The use of multiple measurements in taxonomic problems as an example of linear discriminant analysis"*.

* The data set consists of 50 samples from each of three species of Iris (*Iris setosa*, *Iris virginica* and *Iris versicolor*).
* Four features were measured from each sample, the length and the width of the sepals and petals, in centimetres.
* Based on the combination of these four features, Fisher developed a linear discriminant model to distinguish the species from each other.

Similarly, we will use this homework to get you familized with `numpy` and `scikit-learn`.

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

# Problem description

**If we want to design an algorithm to recognize iris species, what might the data be?**

* We need a 2D array of size `[n_samples x n_features]`.

    - What would the `n_samples` refer to?
    - What might the `n_features` refer to?

Remember that there must be a **fixed** number of features for each sample, and feature
number ``i`` must be a similar kind of quantity for each sample.

# Jupyter Notebook

We have prepared a the [`Recognizing Iris flowers.ipynb`]() Jupyter notebook that explains the Iris flowers problem in detail.

# Your work

* ...you have the data!
* You must now program a Multi-Layer Perception and, at least one other machine learning method for recognizing the flowers in the iris dataset.
* Compare their performance.

Ask yourself some questions:

* What kind of problem is this?
* Must we transform the data?
* How would you implement the train/test/validation cycle for comparing.

## Implementation details

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

* Prepare a Jupyter notebook describing your work and showing your results -> **plots and expected!**
* Do not used any pre-existing library (like Keras, theano, Tensoflow, etc.) for programming your algorithms.
* You may use them for support but not for the algorithm itself.
* `params` is a dictionary with the configuration of the algorithm: layers, number of nodes in each layer, activation functions, learning rates, etc.

# Submission

Submit your notebook files via Google Classroom.
