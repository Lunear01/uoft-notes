 ### Counters
- Similar to shifters but instead of all bit shifters having the same clock, the right clock takes in NOT Q as input to the clock, having a counter effect (Asynchronous counter)
	- Synchronous counter 
		- Implementing and gates to check all previous values with a single clock 
- MUX used to chose between load (holds/load the input) and count
- NOTE: Counter halves the time as it moves from right to left
	- Powers of 2, so we can use that to determine the speed being asked for
		- Use a MUX to choose which rate we want and wire the output
	- Morsecode
		- shifter register
	- Use MUX to implement a look up table 

### State Machines
- Thomas the train
	- Transitions from one state to another
- State Tables
- Finite state machines 


### Designing Finite State Machines 
- Define input and outputs
- Making a state diagram: drawing FSM
	- What are the possible states and how do they relate to each other with different inputs
- Make a state table: translate the diagram in table form 
	- prev state
	- input value
	- next state
- Flip flops: Converting the states into flip flops
	- Decide how many flip flops (powers of 2, so do $log_2(numOfstates)$ and round up) 
	- Assigning flip flop values to represent each state
		- **Intermediate states and race condition**
		- Avoiding multiple changes at once
			- From 0000 to 0010, there's a moment that the device with hold the value of 0001 before transitioning to 0010
	- 