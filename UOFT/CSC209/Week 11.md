## Shell Programming

#### The Shell (Big loop)
- Print prompt
- Read command
- Parse command
- Exec command

- Shell needs to do parsing to the user command
	- Parsing the * from `cat *.c` for example, can see this in action  using echo
- Variables
	- No space in between
		- `i=4`, otherwise, sh would think it's running program called i with two parameters
- `expr`
	- arithmetic in shell
- back quotes runs the command first, like a parenthesis
- `test`
	- runs the test and store the status in $?
- `$?`
	- 0 means success 
	- 1 means fail
- `if` takes the success or fail from running a program
	- ![[Pasted image 20260323165337.png]]
	- ![[Pasted image 20260323165358.png]]
	- ![[Pasted image 20260323165412.png]]
- `while`
	- Same logic, it takes the exit status of a command
- Quoting in shell
	- "ls" and ls are the same, everything is a string
-  `seq`
	- used like a for in range
	- `seq 1 4`
		- from 1 to 4 inclusive
-  `case`
	- ![[Pasted image 20260323170931.png]]