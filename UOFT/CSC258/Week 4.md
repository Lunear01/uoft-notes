### Sequential Circuits
- Thomas toy example
	- Pushing the same button gives different outputs
- Circuits that depends on both the current input and the previous state of the circuit

### Feedback Circuit 
- Have the output of the gate go into the input
	- Kinda like a recursive call
- Oscillation can happen 
	- NAND Gate 
### Latches
- Multiple unstable gates such as NAND and NOR, combined to get a more steady behavior
- D Latch
	- combining the set and reset into a single input

Flip-Flop
- More controlled, the flow of input and output is more expected
	- Calculator example
D Latch and Flip flop
- Flip flip: More controlled, the flow of input and output is more expected
	- Calculator example
- Latch: Less controlled, the flow of input and output is unexpected as it allows the flow of input and output go wild before stopping the clock
	- Can be fixed through a canal model to fix the timing issue
	- Two latches connected together
		- The clock turns off in the second latch as soon as the input latch gives in its inputs
	- Negative edge-triggered
- Positive-edge triggered 
	- Sticking a not gate in the front clock input
		- total of 2 not gates in the clock input
	- Default flip flop is the D-positive edge triggered


### Sequential vs Combinational
- Combinational circuits can be measured and predicted through a truth table
	- Inputs always maps to a single output 
- Sequential circuits can't be measured through a truth table
	- Single input can map to different outputs

### Gate Delay
- It requires time for the electrons to flow, it does not happen instantaneously
- Clock
	- When can certain operations happen
	- Indicates how long in between things that happen: processing power
		- 2.4GHz, 2.4 billion things happening per second 

### Shifters
- Logical: treat everything as bits
- Arithmetic: treat it as a number
	- Preserves negative numbers 

### Registers
- Gatekeeper, setting the clock speed before sending it back to the input
- Stores the output from a previous state
	- Shift registers
		- shifted bit by bit