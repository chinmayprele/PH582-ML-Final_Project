## Preprocessing the data:

### 1.	Working with an imbalanced dataset

- Using the original dataset, calculate the F1 score, precision and recall. Look at confusion matrix.
- Applying following techniques and comparing the performance metrics
	- Oversample the minority class by importing SMOTE
	- Create ensemble balanced sets.  
	- ADASYN – similar to SMOTE but just that it adds small random values to the points that makes it more realistic and have little more variance than being linearly correlated.
- Calculate the F1 score, precision and recall for both cases a and b.
- Plot the sizes of both the classes – M and B and check whether the dataset has balanced.
- Pick the case which gives better results.

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
- A few popular decision tree algorithms like C4.5, C5.0, CART, Random Forest, Neural networks, SVM
- We will experiment with all of them, and maybe use an Ensemble to predict our dataset.

### 4.	Loss functions

### 5.	Evaluating the model and making predictions
