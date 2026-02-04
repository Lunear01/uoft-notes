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
	- 