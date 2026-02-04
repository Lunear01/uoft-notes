 ### Discrete Joint PMFs and Marginal/Conditional Distributions
 
 - ==Discrete Joint PMFS==
	 - When you can have two variables happening simultaneously

 - ==Marginal PMF==
	 - Probability of a single variable (holding one variable constant)
		$$P_x = \sum_{all(y)} p(x,y)$$
		$$P_y = \sum_{all(x)} p(x,y)$$
	- This is essentially adding all the probabilities of a single variable constant. Kind of like partial derivatives. 
	
- ==Conditional PMF==
	- Find probability of an event given that an event had already happened
	- Probability of X given Y
		$$P_x(X|Y) = \frac{p(x,y)}{p_y(y)}$$
	- This is essentially getting the probability of everything and divides out the probability of the given value`y` 

- ==Find E(X) and E(Y) ==
	$$E(X) = \sum_{all(x)} x * p_X(x)$$
	$$E(Y) = \sum_{all(y)} y * p_Y(y)$$

- ==Finding E(XY)==
	$$E(XY) = \sum_{all(x)}\sum_{all(y)}xy * p(x,y)$$
- ==Find Covariance==
	$$Cov(X,Y) = E(XY) - E[X]E[Y]$$
	- Essentially subtracting off the overlap between E\[X\] and E\[Y\]
	- ==If Covariance is negative==, then it has negative linear association
		- When one increase, the other decrease
			- So if X represents success and Y represents cost, it indicates that high success with low cost
	- ==If Covariance is positive==, then it has positive linear association
		- What one increase the other also increase
			- High success indicates high cost
	- ==If Covariance is 0==, X and Y are unrelated.

- ==Finding Correlation  Coefficient==
	$$\rho(x,y) = \frac{Cov[X,Y]}{\sqrt{Var[X] + Var[Y]}}$$
	- This always produces a value between 1 - 0, indicates the direction of increase or decrease, how strong the relation is. 
			$$Recall\:that: Var[X] = E[X^2] - E[X]^2$$
	- If the value is 0.8-1.0, it's considered to be strong
	- If the value is 0.6-0.8, it's considered to be moderately strong
	- If the value is 0.4-0.6, it's considered to be moderate
	- If the value is 0.0-0.4, it's considered to be weak/negligible
- 