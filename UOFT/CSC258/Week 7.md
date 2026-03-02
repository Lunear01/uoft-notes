### Processor Components
- Microprocessor
	- Controller unit 
	- Storage unit
	- Arithmetic unit
- Datapath
	- Where data computations takes place
	- Calculation per clock cycle
		- Example of $x^2 + 2x$
- Control: Finite State Machine
	- FSM to send signals to perform specific calculations
- ALU Outputs
	- V: Overflow condition
		- The result can't be stored in the n bits of G, thus the result is incorrect
	- C: Carry out bit 
	- N: Negative
	- Z: Zero 
- Multiplication: Lab 6
	- Doing state table without kaughnal map
		- Using a big MUX with select bits to represent a single value of a flip flop and an select bit to represent the input 
		- Combinational circuit to decide when to turn on
	- Part II: determine what operations and how operations to do first and where is it stored

### Binary Multiplication
- You take both binaries and `AND` them together bitwise
	- ![[Pasted image 20260227120056.png]]
	- Booth's Algorithm
		- Separate complex operations into multiple easier steps for example, having something like $11 \times 99$ is the same thing as $11 \times 100 - 11 \times 1$ 