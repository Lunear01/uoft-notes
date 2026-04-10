
#### Artificial Intelligence
#### Machine Learning
- Supervised Learning: data with labels / correct answers
	- Regression: Predict continuous value
		-  Linear Regression
		- Multiple Linear Regression
		- Assumptions:
			- Linearity: Relationship exists between predictor target variable
			- Independence: Observations in dataset are independent of each other
			- Homoscedasticity: Spread of residuals should be roughly the same across the range of predicted values.
			- Normality: Errors normality distributed 
		- Ordinary Least Squares (OLN): minimize the error between output value and actual value 
			- **1. Calculate Residual:** 
				- Residual is the difference between actual output and predicted by model
			- **2. Square the Residuals**: 
				- Add weight to errors and make it non negative
			- **3. Sum the Square Residuals**: 
				- Residual Sum of Squares, add all the squared values up to get RSS to get the model's overall error
			- **4. Minimize the Sum of Squared Residuals**: 
				- Adjust the coefficients to minimize RSS
	-  Classification: Identification based on trained data
		- Logistic Regression: 
			- Sigmoid function
- Unsupervised learning
#### Deep Learning