# Linear regression in Python
**linear regression:** is a process to find relationships between variables.

it can be done by using numpy, scipy, stats model and **sckit learn**.

**Scikit-learn** is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction.

Typically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related.

Regression is also useful when you want to forecast a response using a new set of predictors. For example, you could try to predict electricity consumption of a household for the next hour given the outdoor temperature, time of day, and number of residents in that household

In order to use linear regression in Python we need to import it:
```
from sklearn.linear_model import LinearRegression
```
Some important functions to fit a linear regression model:
 	 |function|model|
|--------|-------------------|
|```lm.fit()```|fits a linear model|
|```lm.predict()```|Uses estimated coefficients with the linear model to predict Y|
|```lm.score()```|The coefficient of determination is returned|

> With increeasing data, the error in prediction might also increase.
## Training and validation data sets
Usually linear regression isn’t implemented on the entire data set, it’s usually used on some training and testing data sets to monitor it’s performance and efficiency.

- scilit learn provides a function for training and testing by spliting, called train_test_split().

- A good why to visualize errors in data is by using Residual plots.
