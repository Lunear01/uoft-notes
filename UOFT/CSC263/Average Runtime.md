### Steps
1. Determine the probability model being used and define the input size in terms of $n$ as a set
2. Define how we are measuring runtime
3. Define $T$ to be a random variable representing the runtime
4. Compute the expected value of T
	- Weighted average

 
### Using Indicator Variable
1. Determine the input size and probability distribution
2. Define how runtime is measured 
3. Define $T$ to be a random variable representing the TOTAL runtime 
4. Define an indicator variable that counts 1 when 1 step is performed, 0 otherwise $$X_{ij} = \begin{cases} 
1, & \text{if } i \text{ and } j \text{ are compared} \\ 
0, & \text{otherwise} 
\end{cases}$$
5. Write $T$ in terms of $X_{ij}$, thus representing the total numbers of steps
6. Apply linearity of expectation and find the expected value


### Proving $O$ 
1. Have to proof for every, it has to be less than or equal to

### Proving $\Omega$ 
1. This is the equivalent as finding the AT LEAST the algorithm runs
2. Find a specific example in terms of $n$ PROOF THERE EXISTS

### Formulas to memorize
- ![[Pasted image 20260211161737.png]]