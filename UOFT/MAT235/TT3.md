
## Find Global Maxima and Minima
- Finding global min/max on $f$ in $R$ 
	- Find critical points
		- first derivative and set to zero 
	- Check if it's min/max
		- Second derivative test
		-  ![[Pasted image 20260205082842.png]]
	- If $R$ is a bounded region, check end points
- ### Extreme Value Theorem
	- A function is guaranteed to have both global max and min over a **closed and bounded domain**

## Polar Coordinates
- Covert the integrand to r, $\theta$ by using $x = cos(\theta), y = sin(\theta), x^2 + y^2 = r^2$ 
- Put $dA = rdrd\theta$   

## Cylindrical Coordinates
- ![[Pasted image 20260205112719.png]]
- Put $dA = rdrd\theta$   
## Spherical Coordinates
- Describing $p,\phi,\theta$ for $P$ where $p = \sqrt{x^2+y^2+z^2}$  is the distance of P from the origin. 
	- $\phi$ is the angle between the positive z-axis and the x or y axis
	- $\theta$ is the angle between the x and y axis
		- $x = p\times sin(\phi)cos(\theta)$
		- $y = p\times sin(\phi)sin(\phi)$
		- $z = p \times cos(\phi)$
		- $DV = p^2sin(\phi)DpD\phi D\theta$
		

## Extremely Useful Integration Techniques
1. If the function is odd and the region of integration is symmetric along the origin, then the integral is always 0 
2. For difficult integrals, try flipping the order of integration, remember to redefine the region of integration
	- When swapping, simply just solve one variable in terms of the other variable 
	- If it's x, write it in terms of y, vice versa

