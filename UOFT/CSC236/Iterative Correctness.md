3 Parts to proof iterative correctness
1. Recursively Validity
2. Recursively Correctness
3. Termination

Recursive Validity
1. Declare $I_k$ ==Mostly for the loop variable==
2. Ensure that $I_0$ is correct by preconditions
3. Assume $I_k$ is correct, that is when the invariant holds until the k-th iteration
4. Show that $I_{k+1}$ also satisfy the loop invariant 

Termination
1. Loop variant: measure of a size of a loop
2. Prove that the loop variant is a natural number and decreasing using WOP. 
- Steps 
	1. Show that $V_0$ satisfies the variant conditions
	2. Assume $V_k$ (The inductive hypothesis)
	3. Show that $V_{k+1}$ satisfies the variant conditions

Correctness
- Proving the post-condition 
- Steps
	1. Assume the negation of the loop condition