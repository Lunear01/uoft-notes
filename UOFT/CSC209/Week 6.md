### Useful C features
- `typedef`
	- Kind of like having a customized variable type like `int` `char`, etc
	- ![[Pasted image 20260209135632.png]]
	- Creating aliases to refer the same thing, can make code look cleaner
- `macros`
	- Creating an alias for anything other than a type
	- This is the one that we have been using to declare global variables 
	- Format
		- `#define Variable 1.02`
	- You can also define functions with parameters 
		- `#define func(x) ((x) + 2)`
			- Make sure that there are no spaces in between `func` and `(x)` 
			- Make sure to add parenthesis around `x` within the parameter as it could cause order of operation errors
	- Common errors
		- ![[Pasted image 20260209144126.png]]

### C Preprocessor 
- Processing the code before getting compiled
	- Everything with the `#` such as the macros are processed before compiling
-  The `cpp` (C Preprocessor) goes through the macros defined and replaces everything within the file that uses that macro with `strings` 
	- It also replaces the macros keywords in comments
	- It replaces the **exact** reference, thus if you have one letter difference, it wouldn't get replaced by the defined value
- Macros are fully expanded
	- ![[Pasted image 20260209141657.png]]
- macros with `__something__` are often referring to macros defined within the system
	- Provide help or intro message
	- You can have system wise behavior `gnu/liunx`, `OS/X`,  etc depending on the machine
- You can have  `if` `elif` and `else` within macros to define different set of variables
	- ![[Pasted image 20260209142031.png]]
-  Can be used for debugging 
	- ![[Pasted image 20260209142210.png]]

### System Calls
- Function the request from an operating system
- `exit` 
	- ![[Pasted image 20260209145642.png]]
- ![[Pasted image 20260209145900.png]]
- System calls in a linux machine

### Errors and Errno
- When errors are occurred when performing a system call, it returns -1 along with a number that specifies the type of error
	- ![[Pasted image 20260209152636.png]]
- `perror` 
	- prints the error into the stand output, use when checking system calls
	- ![[Pasted image 20260209155242.png]]
	- f