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
- 