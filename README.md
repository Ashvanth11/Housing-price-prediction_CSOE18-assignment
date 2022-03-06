# Housing-price-prediction_CSOE18-assignment
Dataset Chosen:
The Boston Housing Dataset
The Boston Housing Dataset is a derived from information collected by the U.S. Census Service concerning housing in the area of Boston. The dataset contains 506 cases. The following describes the dataset columns:
•	CRIM - per capita crime rate by town
•	ZN - proportion of residential land zoned for lots over 25,000 sq.ft.
•	INDUS - proportion of non-retail business acres per town.
•	CHAS - Charles River dummy variable (1 if tract bounds river; 0 otherwise)
•	NOX - nitric oxides concentration (parts per 10 million)
•	RM - average number of rooms per dwelling
•	AGE - proportion of owner-occupied units built prior to 1940
•	DIS - weighted distances to five Boston employment centres
•	RAD - index of accessibility to radial highways
•	TAX - full-value property-tax rate per $10,000
•	PTRATIO - pupil-teacher ratio by town
•	B - 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
•	LSTAT - % lower status of the population
•	MEDV - Median value of owner-occupied homes in $1000's
Model chosen:
We chose Linear Regression Model to predict the prices of homes using the above Dataset. Linear Regression is a machine learning algorithm based on supervised learning. It performs a regression task. Regression models a target prediction value based on independent variables. It is mostly used for finding out the relationship between variables and forecasting. Different regression models differ based on – the kind of relationship between dependent and independent variables, they are considering, and the number of independent variables being used.

Calculated Bias: 20.803
Calculated Variance: 0.621

Feature Selection:
We use correlation feature selection. Linear correlation scores are typically a value between -1 and 1 with 0 representing no relationship. For feature selection, we are often interested in a positive score with the larger the positive value, the larger the relationship, and, more likely, the feature should be selected for modeling. As such the linear correlation can be converted into a correlation statistic with only positive values.

The scikit-learn machine library provides an implementation of the correlation statistic in the f_regression() function. This function can be used in a feature selection strategy, such as selecting the top k most relevant features (largest values) via the SelectKBest class.

For example, we can define the SelectKBest class to use the f_regression() function and select all features, then transform the train and test sets.

Calculated Bias after feature selection: 2.967
Calculated Variance after feature selection: 0.328 

We have reduced Bias and Variance after feature selection.
