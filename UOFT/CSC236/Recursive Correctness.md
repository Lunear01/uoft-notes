### Correctness
- To prove correctness of a function we mean that the function should ==terminate== and return a value correctly if the correct parameters are given. 
	1. Returns the correct value
	2. Terminates
	3. Check for valid operators used
	4. Returned values matches with post conditions
- Template for proving recursive correctness assuming that the algorithm is ==recursively valid==. 
- ![[Pasted image 20251212234630.png]]
- 

### Validity 
- Validity is when the recursive function
	1. Always perform valid calls to the function
		- By checking function preconditions
	2. Call tree is finite, it terminates
		- For example, if a recursive function is a decreasing sequence of naturals, it must end
	3. Smaller recursive calls are also valid
- Template: 
	- Summary:
		1. Let size(n) = n 
		2. Valid measure $\because n \in \mathbb{N} :\ by Pre$ 
		3. Valid Call
			- Show that calls satisfy all preconditions 
		4. Valid Recursively $$Show\:size(n-k) = n-k < n = size(n)$$ 
	- ![[Pasted image 20251212200331.png]]
	- Example question: 
	- ![[Pasted image 20251212200427.png]]
- 