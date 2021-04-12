## Preprocessing the data:

### 1.	Working with an imbalanced dataset

#### Oversampling

We chose to use `random.choices()` to oversample our minority set (malignant) since we thought it biologically appropriate.
The script used to oversample can be found at `/outline/script/data_modifier.py`

- [ ] Calculate the performance metrics: F1 score, precision and recall, Confusion matrix

### 2.	Identify relevant variables to make predictions.

- Drop the target columns (what we want to predict)
- The following `sklearn` methods will be applied and we will pick the features that will be found to have high relevance to make necessary predictions.
	1. Import `sklearn.feature_selection.SelectKBest`
		- Score functions to be used are either f_classif (ANOVA F-value between feature/label) or chi2 (chi-squared stats of non-negative features) for our classification task.
		- Fit the best features and concatenate dataframes of the columns selected using the Univariate feature selection “SelectKBest”
	2. Feature Importance method
		- `from sklearn.ensemble import RandomForestClasifier -> .feature_importances_`
	3. Feature correlation method: `.corr()`
- We will chose the “top” features generated in our list for each method.              
- Generate heat map to make decisions about which features to include in the new dataset.

### 3.	Algorithm selection

- Other than using the algorithms prescribed above, we will also experiment with a few others.
- A few popular decision tree algorithms like C5.0, Random Forest, Neural networks, SVM
- We will experiment with all of them, and maybe use an Ensemble of these models to predict our dataset.

### 4.	Loss functions

- We will have to determine the loss functions we use depending on whether we choose to use a single decision tree algorithm, or whether we use an Ensemble.
- We will test multiple loss algorithms with each strategy, and then use the most appropriate one.

### 5.	Evaluating the model and making predictions

- The mammograms generally identify the irregular edges of the tumor which are categorized as malignant tumors. Biologically, we expect that the following features will have the largest effect on the model:
	- radius
	- perimeter
	- area
	- compactness
	- symmetry
- We can use the `data_modifier.py` script to subset our initial and oversampled dataset to only grab these features.
- We will also use `sklearn.feature_selection.SelectKBest` to validate these results.
