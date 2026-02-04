## Week 1
Resistance
Current
- Current moves positive to negative for historical reasons
Transistor
- nMos: On with high voltage 
- pMos: On with low voltage
Conductors
Insulators
Semiconductor 

## Week 2
Circuit Creation
- Create truth table
- Express as boolean expression
- Covert into gates
- Minterm expression
	- Represents the `and` expressions, what is causing output to be 1
	- Combination of inputs needed to produce an output to go high
	- Examples: 
		- In terms of binary expressions
		- $m_{12} = A + B + not C + not D$  
	- Combining minterms using `or`
		- Sum of minterm
- Maxterm expression
	- Represents the `or` expressions, what is causing output to be 0
	- High all the time except for one case
		- Exact way of thinking of a minterm but flipped over (its negation)
	- Product of maxterms
		- Use `and` gates
- Converting SOM to gates 
- Reducing circuits
	- Karnaugh Map
		- Grouping adjacent 1's into groups of powers of 2's: $2^n$ 
		- De Morgan's Law: 
			- $\overline{X} * \overline{Y} = \overline{X} + \overline{Y}$
			- Important bc allows use to convert to NAND gates, cheapest/ 
		- The order goes 00, 01, 11, 10
			- Ordered so that it's different to neighbors by 1 value
		- Grouping restrictions
			- Has to be neighboring
			- 