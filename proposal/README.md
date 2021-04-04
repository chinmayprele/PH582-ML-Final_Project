# Predicting Breast Cancer using the _Breast Cancer Wisconsin_ (Diagnostic) Dataset

### Dataset

- [Dataset Page](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)
- [Dataset Download Link](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)

##### Attribute Information:

1) ID number
2) Diagnosis (M = malignant, B = benign)
3-32)

Ten real-valued features are computed for each cell nucleus:

a) radius (mean of distances from center to points on the perimeter);
b) texture (standard deviation of gray-scale values);
c) perimeter;
d) area;
e) smoothness (local variation in radius lengths);
f) compactness (perimeter^2 / area - 1.0);
g) concavity (severity of concave portions of the contour);
h) concave points (number of concave portions of the contour);
i) symmetry;
j) fractal dimension ("coastline approximation" - 1)

The mean, standard error, and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features.  For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.


### Technique(s)

1. __Handling imbalanced Dataset__
	- Our dataset is imbalanced since the distribution across samples is known to be skewed/biased.
	- We will be using [SMOTE](https://github.com/scikit-learn-contrib/imbalanced-learn) (Synthetic Minority Over-sampling TEchnique) to handle this.
		- It contains algorithms in multiple categories, including SMOTE, and:
			- Under-sampling the majority class(es).
			- Over-sampling the minority class.
			- Combining over- and under-sampling.
			- Create ensemble balanced sets.

2. __Undersampling, oversampling and generating synthetic data__
	- These methods are often presented as great ways to balance the dataset before fitting a classifier on it. In a few words, these methods act on the dataset as follows:
		- undersampling consists in sampling from the majority class in order to keep only a part of these points
		- oversampling consists in replicating some points from the minority class in order to increase its cardinality
		- generating synthetic data consists in creating new synthetic points from the minority class (see SMOTE method for example) to increase its cardinality

<!-- https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/ - this tutorial is for us and not for proposal -->

3. __Feature Selection__
	- The `scikit-learn` library provides the `SelectKBest` class that can be used with a suite of different statistical tests to select a specific number of features.
	- Use the chi-squared (chi^2) statistical test for non-negative features

4. __Algorithm Selection__
	- Other than using the algorithms prescribed above, we will also experiment with a few others.
	- A few popular decision tree algorithms like C4.5, C5.0, CART, Random Forest, Neural networks, SVM
	- We will experiment with all of them, and maybe use an Ensemble to predict our dataset.

5. __Loss Functions__
	- We will have to determine the loss functions we use depending on whether we choose to use a single decision tree algorithm, or whether we use an Ensemble.
