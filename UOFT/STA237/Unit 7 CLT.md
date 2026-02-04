## Central Limit Theorem
### Limitations
1. Must random experiment
2. Must but independent of each other, without replacement
3. Sampling size must be large enough 
4. Must have finite variance 

Central Limit Theorem states that no matter what distribution you use, the sampling distribution of their sampling mean for a large sample size are always going to looking like a bell-curve/Normal Distribution. 

==Standard Derivation Error== (Standard Deviation for Sampling Mean): $$\sigma_{x} = \frac{σ​}{\sqrt{n}}$$
This is used to estimate how close the values are to $\lambda$ 


==Sampling Mean:== Essentially add everything divide the total added. 
$$\frac{1}{n}\sum_{i=1}^{n}X_{i}$$
==Expected Value of Sampling Mean: ==Derived using linearity of expected values.
$$E(aX + bY) = aE(X) + bE(Y)$$
$$\mu$$
==Variance of Sampling Mean:== Derived using linearity of variance 
$$Var(aX) = a^2E(X)$$
and Variance independence
$$Var(X + Y) = Var(x) + Var(Y)$$
$$\frac{\sigma^2}{n}$$

Consequences of CLT: 
1. Sample size too small: The sample distribution will not look normal
2. Variables not independent: Standard error is going to be underestimated. 
3. Variables not random: biased estimator, meaning the mean of the sampling will not be the same. 

Example Problem: 

The time (in minutes) a U of T student spends looking for parking on campus follows a highly **right-skewed** distribution with a **population mean (μ) of 15 minutes** and a **population standard deviation (σ) of 8 minutes**.

A random sample of **n=40** students is taken. What is the probability that the sample mean parking time (x) is between 14 and 16 minutes?

- Solution: 
	- Check necessary condition for CLT
		- Random and independent? 
			- Yes since the sample students are randomly selected
			- Independent size student are not interfering with one another
		- Large enough sample size?
			- Yes since sample size is 40 
	- Want P(14 < X < 16), where X is the number of minutes parked on campus. 
		- Given $\mu$ = 15, $\sigma$ = 8, n = 40. 
		- Expected value (mean) of sample mean = $\lambda$ = 15
		- Standard error (standard deviation of sample mean) 
			$$\frac{\sigma}{\sqrt{n}} = \frac{8}{\sqrt{40}} = 1.2649$$
		- We have 
			$$P(14 < X < 16) = P(\frac{14-15}{1.2649}< \frac {X-15}{1.2649} < \frac{16-15}{1.2649}) = P(-0.79 < Z < 0.79)$$
		- Finally
			$$P(-0.79) < Z < 0.79) = P(0.79) - P(-0.79)$$
