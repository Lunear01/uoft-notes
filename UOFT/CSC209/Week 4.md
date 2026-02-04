## C Language
- Strings
	- Is an array of `char` with a `NULL` at the end to mark the end of a string
		- Example: with NULL being `\0`
			```c
			char str[20];
			string[0] = 'h';
			string[1] = 'i';
			string[2] = '\0';
			
			// Now str is a string, meaning it can be printed using %s
			```
- String Literal vs. String Variable
	- String literal is a fixed string, can't be changed
		- Declared by: 
			- char \*str = "Hello";
	- String variable is an array of characters with `\0` at the end
		- Can be changed by index
		- Declared by: 
			- char str[] = "Hello";
- String declaration in C 
	- Can be declared in the following ways
		```c
			char str[20];
			string[0] = 'h';
			string[1] = 'i';
			string[2] = '\0';
			
			char str[20] = {'h','i','\0'};
			
			char str[20] = "hi";
			
			char str[] = "hi";
			
			// Without defined the memory assigned, C will automatically assign
			// enough memory for the string and the NULL at the end
		```
	- Make sure to include enough space for the string AND the NULL at the end. 
- String Length
	- Using the builtin C library `#include <string.h>`
	- `strlen` to find the length of a string 
- Copying and concatenating strings
	- `strcpy` 
		- ![[2026-01-20-204944_hyprshot.png]]
		- Copying overrides
		- It copies s2 into s1, overriding what's in the start of s1
		- `strcpy` is considered to be an UNSAFE function 
			- Unexpected behavior can happen when the string copies to a variable with less than the space required.
	- `strncpy`
		- The better/safer version of `strcpy`, including an extra parameter `n`
		- ![[Pasted image 20260120205643.png]]
		- `n` is the maximum character that s1 can hold
		- Can also be unsafe if it doesn't end with `\0`
			- Fix it by adding it manually 
	- `strcat`
		- ![[Pasted image 20260120211300.png]]
		- Add the characters of s2 to the end of s1 
		- NOTE: It first looks for the first '\0' it founds and then add S2
			- Important because it can have errors in uninitialized memories
	- `strncat`
		- Safe version of `strcat`
			- ![[Pasted image 20260120211452.png]]
- Searching through strings
	- `strchr`
		- ![[Pasted image 20260120211812.png]]
		- (the string to look in, the character to look for) from left to right
		- Returns the pointer to the character that was found, or NULL if not found 
	- `strstr`
		- ![[Pasted image 20260120212047.png]]
		- Searches the first occurrence of a substring within a string
		- If s2 is found in s1, returns the pointer to the first character of the substring
	- **To find a precise index, perform pointer arithmetic**
- Structs
	- Storing collections of different datatypes 
	- Similar to a class
	- Example usage:
		- ![[Pasted image 20260120213239.png]]
	- Structs when passed into a function as a parameter, it creates a copy of the struct, unlike arrays, which pass the pointer of the first element. 
		- To make it so that functions modifies the original, pass in a pointer of the struct instead
	- Syntax: Changing data inside a struct
		- ![[Pasted image 20260120214134.png]]
		- `->` is the same as `(*p).`