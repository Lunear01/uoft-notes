### File Descriptors
- File descriptor is a field in a FILE struct
- File descriptor of 1 links to standard output
- The global variable for stdin is of `FILE *` type

Pipes
- Allows processes to communicate with each other
	- Contains `fd[0]` and `fd[1]` 
		- 0 is to read
		- 1 is to write
- ![[Pasted image 20260302184809.png]]
- The parent process is on the left and child process is on the right
- When using a pipe, only 1 write and 1 read should be on.
	- use `close` to close the other tunnels that are not used
- ### Producer Consumer Problem
	- In a buffer queue we have producer and consumer
	- When the rate of the producer and the consumer are not the same
		- Can fill up the entire buffer queue 
		- Can consume on a blank queue
	- #### Problematic situations
		- Produce add when queue is full
		- Consumer remove when queue is empty
		- Both operating the queue at the same time