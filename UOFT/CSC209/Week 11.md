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
		- 