Transformation are essentially substituting a new variable that includes the original variable and find its CDF and PDF. 

### Distribution Method: 
- If we have the CDF of $X$, $F_x(X)$,  $P(X\leq{x})$ , and have a transformation of $Y=g(x)$ a function X, we can perform transformation by doing the following: 
	$$F_y(Y) = P(Y\leq{y}) = P(g(x)\leq{y})$$
	Example Question of application: 
	- **Question:** If X is a continuous random variable with a known CDF $F_x(X)$, and the transformation is $Y=2X+5$ (a simple linear transformation), write out the expression for $F_Y(y)$ in terms of $F_X$​ and $y$.
		- Solution: 
			1. So we are going rewrite Y as a function of X, something that we know. 
			$$F_y(Y) = P(Y\leq{y}) = P(2X+5\leq{y}) = P(X\leq{\frac{y - 5}{2}}) = F_X(X)$$
### Deriving the PDF 
- We know that integrating the PDF gives the CDF of the function, analogous adding PMF for CDF. 
	- From CDF -> PDF we ==Differentiate==
	- From PDF -> CDF we ==Integrate==
	- From PMF -> CDF we ==Sum==
- We we have the CDF for continuous functions and we want to find the CDF we do
	$$PDF = \frac{d}{dx}[F_y(Y)] = \frac{d}{dx}[P(X\leq{\frac{y-5}{2}})]$$
	