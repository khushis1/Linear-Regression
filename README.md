EXPERIMENT — LINEAR REGRESSION (SALES VS TV)

OBJECTIVE
Train and evaluate a simple linear regression model to predict Sales from TV advertising spend, including diagnostic plots and error metrics.

RATIONALE
Linear regression is a fundamental supervised technique offering interpretability and a useful baseline for continuous targets.

THEORY SUMMARY
	•	Ordinary Least Squares (OLS): fit a linear model y = β0 + β1 x by minimizing sum of squared residuals.
	•	Performance metrics: RMSE quantifies prediction error in original units; R² indicates proportion of variance explained.
	•	Assumptions: linear relationship, independent errors, homoscedasticity, normal residuals; violations suggest transformations or alternative models.

DATA USED
advertising.csv containing TV, Radio, Newspaper, and Sales. This experiment uses TV as the predictor and Sales as the target.

STEP-BY-STEP PROCEDURE
	1.	Load and inspect the dataset.
	2.	Visualize TV vs Sales with a scatter plot.
	3.	Split data into training and test sets.
	4.	Train sklearn.linear_model.LinearRegression on the training set.
	5.	Predict on the test set, compute RMSE and R².
	6.	Plot actual vs predicted and residuals for diagnostics.
	7.	Investigate any large residuals or influential points.

HOW TO RUN
Place advertising.csv in the working directory, open the notebook in Colab, and run all cells.

EXPECTED OUTPUT
	•	Model coefficients (slope and intercept).
	•	RMSE and R² on the test set.
	•	Scatter plot of predictions vs actual values and residuals plot.

PRACTICAL NOTES
	•	If residuals show systematic patterns, consider polynomial features or transformations.
	•	Use cross-validation for more robust performance estimation.
	•	Check for influential observations with Cook’s distance when interpreting coefficients.
